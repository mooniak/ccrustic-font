# CCRustic: shipping checklist

Status on 18 November 2026, after the ASCII → Unicode port and the move to the Mooniak pipeline
(`dev` branch). Maturity: **beta**. The font sets real Unicode text, but it has no repaya, few
conjuncts, and a few glyphs need the designer's confirmation. Tick items as they're done; keep
this file current with each release.

## 1. Repository and pipeline

- [x] Repo `mooniak/ccrustic-font`, from the Mooniak project template
- [x] Template synced to the latest (`mnik template-sync ccrustic-font`)
- [x] `dev` branch is the working branch; `main` is release-only
- [ ] Push `dev` and make it the GitHub default branch:
      `git push -u origin dev && gh repo edit mooniak/ccrustic-font --default-branch dev`
- [x] `sources/config.yaml` builds static TTF + OTF + WOFF2 from the Glyphs package
- [x] Builds with `mnik build` (canary and release channels)
- [x] Full CI sequence passes locally in a clean clone: build, stamp, test, proof, manifest, pages
- [ ] GitHub Actions build green on `dev`
- [ ] GitHub Pages serves https://src.mooniak.com/ccrustic-font/
      (`gh api -X POST repos/mooniak/ccrustic-font/pages -f 'source[branch]=gh-pages' -f 'source[path]=/'`
      after the first green run)
- [ ] README badges (build, QA pass rate, release, licence) resolve
- [ ] First `canary` pre-release published by CI

## 2. Source and Unicode port

- [x] The 2021 FM ASCII source committed as received (commit `8f7ba36`)
- [x] Ported to Unicode with `ascii_to_unicode.py` (commit `f3b584c`): every glyph recorded
      in `documentation/ascii-unicode-map.tsv`, CCRustic's deviations from FM in
      `documentation/ascii-overrides.tsv`
- [x] Verified: 1216/1216 texts render the same in the ASCII original and the Unicode font
      (`verify_ascii_port.py`; glyph slots, generated syllables, Pandukabhaya's FM test text)
- [x] Glyph names follow LankaGlyphset
- [x] FontForge GDEF removed; spacing signs Mark/Spacing; overprinting signs zero-width with
      mark anchors at their drawn position
- [x] Source renamed to `sources/CCRustic.glyphspackage`
- [ ] Open and save once in Glyphs 3 (normalises the file; check nothing moves)

## 3. Metadata

- [x] Family name `CCRustic`, style Regular
- [x] Copyright `Copyright 2021 The CCRustic Project Authors (https://github.com/mooniak/ccrustic-font)`
- [x] Designer Damith Welikala, manufacturer mooniak, vendor ID `MNIK`
- [x] SIL OFL 1.1 licence + URL in the font; `OFL.txt` header matches
- [x] `fontpackage.json`: free tier, OFL-1.1, maturity beta; `mnik fp check` clean
- [x] `AUTHORS.txt`, `CONTRIBUTORS.txt`, `documentation/ARTICLE.en_us.html`, specimen images
- [ ] Designer to confirm the description, the credit "Ceylon Calligraphy" and the year (2021)
- [ ] Add the designer's email/URL to `fontpackage.json` `designers` if they want it shown

## 4. Designer decisions from the port

- [ ] **`µ` → `nnI-sinh` (ණි).** In FM, ණි lives at `‚` (0x82), which is an empty glyph in this
      font. The drawing on `µ` looks like ණ with an i-loop, so it was read as ණි. Medium confidence
- [ ] **`` ` `` → `nnga-sinh.alt1`.** In FM `` ` `` is a nasal prefix; here it is a second, full ඟ
      next to `Õ` (`nnga-sinh`). Nothing reaches it. Pick one as the ඟ, or make it an ss
      alternate, or delete it
- [ ] **`A` → `virama-sinh.alt1`.** FM's second al-lakuna, nearly the same as `a`. Nothing
      reaches it. Give it a context (for which letters?) or delete it
- [ ] **`©` → `ornament` on U+E000.** A decorative line ornament. Keep it on the private-use
      code point, map it elsewhere, or drop it
- [ ] **`\` → `ndaa._c-sinh` (ඳා) and `Þ` → `daa._c-sinh` (දා)** are in `ss01`, so by default
      ද + ා is the separate sign. Make them the default (move the rules to `psts`) if the
      below-base forms are the intended look
- [ ] **ක්‍රු / ක්‍රූ** use the plain ු/ූ under the rakaransaya; the hook forms (`usign-sinh.alt1`)
      are used only after ක ග ත භ ශ. Check in the proofs

## 5. Drawing (designer)

- [ ] `jha-sinh` ඣ (U+0DA3): not drawn. FM built it from `C` + `O`, and `C` (touching ක්‍)
      isn't in the font either
- [ ] `repha-sinh`, repaya (ර්‍ + consonant). Common in real text (ධර්ම, කර්ම); today it shows
      ර් + consonant
- [ ] Conjuncts: only ක්‍ෂ, ත්‍ව and ද්‍ර exist. ද්‍ව ද්‍ධ න්‍ද න්‍ධ ත්‍ථ (FM `„ Š ‡ JO †`), and ශ්‍රී (`›`),
      show as letter + al-lakuna
- [ ] Missing ligatures FM fonts usually have: ණි ණී on their own slots, ඳි ඳී ඳූ ඳැ, ලූ, දැ,
      ඬ් ඞ් ඡ් ඡි ඡී ඵි ඵී ඣි ඣී (FM `¢ £ ª ƒ Æ ± å Ù þ ý Â Ý Ú ¯ °`)
- [ ] Optional: ඏ ඐ ඦ, candrabindu U+0D81, ෳ, kunddaliya ෴, Lith digits U+0DE6–0DEF
- [ ] Review the generated `dottedCircle` (12 dots sized from ක)
- [ ] Fontspector outline warnings (FontForge-era): jaggy segments, colinear vectors,
      overlapping segments, counter-clockwise outer contours. Fix the real ones
- [ ] Kerning: none. Kern common pairs for display sizes
- [ ] Optional: Latin, only needed for a Google Fonts submission

## 6. OpenType

- [x] Features generated by `ascii_to_unicode.py`: akhn, vatu, pstf, abvs, blws, psts, ss01;
      `abvm`/`mark` from the anchors
- [x] Two-part vowels (ේ ො ෝ ෞ) split Uniscribe-style (display glyphs + pstf), so HarfBuzz and
      Windows both work
- [ ] When glyphs are added, regenerate the features (or add the rules by hand) and re-run
      `overprint_anchors.py` for new bases

## 7. QA (Fontspector, Google Fonts profile)

Local CI run: 4 FAIL, 16 WARN, 94 PASS, 0 ERROR (201 checks).

- [x] Vertical metrics: hhea = typo = win = 900/−300, `USE_TYPO_METRICS`, covers the bounding box
- [x] No-break space, dotted circle (with mark anchors), name ID 9, copyright, licence, ss01 name
- [ ] Accepted for now (shared by the other Sinhala-only Mooniak fonts): `glyph_coverage`,
      `glyphsets/shape_languages`, `render_own_name` (all need Latin), and the GF
      repository-layout check
- [ ] Remaining WARNs: unreachable `virama-sinh.alt1` and `nnga-sinh.alt1` (section 4), no
      kerning, missing ₹ U+20B9 and U+2028/2029, no STAT/meta table (static font), outline
      warnings (section 5)

## 8. Release

- [ ] Designer sign-off on the proofs at https://src.mooniak.com/ccrustic-font/
- [ ] Tag a preview for testers: `v1.001-dev.1` on `dev`
- [ ] Bump the source version to 1.001 (`versionMinor = 1`) before the release
- [ ] Merge `dev` into `main` (no squash) and tag `v1.001` on `main`
- [ ] Set `maturity` to `stable` once repaya and ඣ are drawn
- [ ] Add display images to `fontpackage.json` `directory.display_images`
