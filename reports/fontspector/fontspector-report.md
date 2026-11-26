## FontSpector report

fontspector version: 1.9.0






## Check results




<details><summary>[12] fonts/ttf/CCRusticCANARY-Regular.ttf</summary>
<div>


<details>
    <summary>⚠️ <b>WARN</b> Check that OS/2 fsSelection WWS bit is set correctly. (opentype/fsselection_wws)</summary>
    <div>








- ⚠️ **WARN** OS/2 fsSelection WWS bit is not set, and the font does not have name IDs 21/22 (WWS Family/Subfamily). If the font's naming is WWS-conformant, the WWS bit should be set. [code: no-wws-without-wws-names]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Check if each glyph has the recommended amount of contours. (contour_count)</summary>
    <div>








- ⚠️ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are
     inferred from the typical amounts of contours observed in a
     large collection of reference font families. The divergences
     listed below may simply indicate a significantly different
     design on some of your glyphs. On the other hand, some of these
     may flag actual bugs in the font such as glyphs mapped to an
     incorrect codepoint. Please consider reviewing the design and
     codepoint assignment of these to make sure they are correct.


    The following glyphs do not have the recommended number of contours:
* uni0D85 (U+0D85): found 1, expected one of: [2, 3, 4]
* uni0D86 (U+0D86): found 2, expected one of: [3, 4, 5]
* uni0D87 (U+0D87): found 2, expected one of: [3, 4, 5]
* uni0D88 (U+0D88): found 2, expected one of: [3, 4, 5]
* uni0D89 (U+0D89): found 1, expected one of: [2, 3, 4]
* uni0D91 (U+0D91): found 20, expected one of: [2, 3]
* uni0D92 (U+0D92): found 21, expected one of: [3, 4, 5]
* uni0D93 (U+0D93): found 21, expected one of: [4, 5, 6]
* uni0D9B (U+0D9B): found 8, expected one of: [2, 3]
* uni0D9E (U+0D9E): found 1, expected one of: [2, 3, 4]
* uni0D9F (U+0D9F): found 4, expected one of: [1, 3, 5]
* uni0DA4 (U+0DA4): found 2, expected one of: [3, 4, 6]
* uni0DA7 (U+0DA7): found 2, expected one of: [1, 3]
* uni0DB5 (U+0DB5): found 12, expected one of: [2, 3]
* uni0DB8 (U+0DB8): found 3, expected one of: [1, 2]
* uni0DC4 (U+0DC4): found 2, expected one of: [1, 3, 4] [code: contour-count]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Does GPOS table have kerning information? (gpos_kerning_info)</summary>
    <div>








- ⚠️ **WARN** GPOS table lacks kerning information. [code: lacks-kern-info]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Ensure indic fonts have the Indian Rupee Sign glyph. (rupee)</summary>
    <div>








- ⚠️ **WARN** Font is missing the Indian Rupee Sign glyph. Please add a glyph for Indian Rupee Sign (₹) at codepoint U+20B9. (Overriden: Sinhala fonts: U+20B9 is optional (Sri Lanka writes රු / Rs)) [code: missing-rupee]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Check font contains no unreachable glyphs (unreachable_glyphs)</summary>
    <div>








- ⚠️ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

* nngasinh.alt1
* viramasinh.alt1 [code: unreachable-glyphs]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Ensure font has overlaps bit set correctly. (overlaps_bit)</summary>
    <div>








- ⚠️ **WARN** The following glyphs have overlaps but the overlaps bit is not set:
* tthIisinh
* uni0D91 (U+0D91)
* uni0D93 (U+0D93)
* uni0D92 (U+0D92)
* uni0D9B (U+0D9B) [code: no-overlaps-bit]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Check font follows the Google Fonts vertical metric schema (googlefonts/vertical_metrics)</summary>
    <div>








- ⚠️ **WARN** We recommend the absolute sum of the hhea metrics should be between 1.2-1.5x of the font's upm. This font has 1.879x (1879) (Overriden: line height is a design choice for Mooniak display faces) [code: bad-hhea-range]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (googlefonts/meta/script_lang_tags)</summary>
    <div>








- ⚠️ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Do any segments have colinear vectors? (outline_colinear_vectors)</summary>
    <div>








- ⚠️ **WARN** The following glyphs have colinear vectors:

* uni0DB3 (U+0DB3): from (318.0, 725.0) to (311.0, 725.0) is colinear with segment from (311.0, 725.0) to (296.0, 726.0)
* rAaesinh: from (577.0, 577.0) to (596.0, 648.0) is colinear with segment from (596.0, 648.0) to (606.0, 684.0)
* parenleft (U+0028): from (64.0, 451.0) to (64.0, 468.0) is colinear with segment from (64.0, 468.0) to (63.0, 507.0)
* parenleft (U+0028): from (64.0, 468.0) to (63.0, 507.0) is colinear with segment from (63.0, 507.0) to (63.0, 523.0)
* parenleft (U+0028): from (64.0, 573.0) to (67.0, 598.0) is colinear with segment from (67.0, 598.0) to (69.0, 621.0) [code: found-colinear-vectors]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Check the direction of the outermost contour in each glyph (outline_direction)</summary>
    <div>








- ⚠️ **WARN** The following glyphs have a counter-clockwise outer contour:

* uni0D91 (U+0D91) has a path with no bounds (probably a single point)
* uni0D91 (U+0D91) has a path with no bounds (probably a single point)
* uni0D91 (U+0D91) has a path with no bounds (probably a single point)
* uni0D91 (U+0D91) has a path with no bounds (probably a single point)
* uni0D91 (U+0D91) has a path with no bounds (probably a single point)
* uni0D91 (U+0D91) has a path with no bounds (probably a single point)
* uni0D92 (U+0D92) has a path with no bounds (probably a single point)
* uni0D92 (U+0D92) has a path with no bounds (probably a single point)
* uni0D92 (U+0D92) has a path with no bounds (probably a single point)
* uni0D92 (U+0D92) has a path with no bounds (probably a single point)
* uni0D92 (U+0D92) has a path with no bounds (probably a single point)
* uni0D92 (U+0D92) has a path with no bounds (probably a single point)
* uni0D93 (U+0D93) has a path with no bounds (probably a single point)
* uni0D93 (U+0D93) has a path with no bounds (probably a single point)
* uni0D93 (U+0D93) has a path with no bounds (probably a single point)
* uni0D93 (U+0D93) has a path with no bounds (probably a single point)
* uni0D93 (U+0D93) has a path with no bounds (probably a single point)
* uni0D93 (U+0D93) has a path with no bounds (probably a single point)
* uni0D9B (U+0D9B) has a path with no bounds (probably a single point)
* uni0D9B (U+0D9B) has a path with no bounds (probably a single point)
* uni0D9B (U+0D9B) has a path with no bounds (probably a single point)
* uni0D9B (U+0D9B) has a path with no bounds (probably a single point)
* uni0DB5 (U+0DB5) has a path with no bounds (probably a single point) [code: ccw-outer-contour]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Do outlines contain any jaggy segments? (outline_jaggy_segments)</summary>
    <div>








- ⚠️ **WARN** The following glyphs have jaggy segments:

* uni0D91 (U+0D91): Quad(QuadBez { p0: (78.5, 604.0), p1: (80.0, 604.0), p2: (87.0, 605.0) })/Quad(QuadBez { p0: (87.0, 605.0), p1: (82.0, 605.0), p2: (77.0, 604.0) }) = 8.130102354156005 degrees
* uni0D91 (U+0D91): Line(Line { p0: (466.0, 257.0), p1: (471.0, 255.0) })/Quad(QuadBez { p0: (471.0, 255.0), p1: (469.0, 256.0), p2: (466.0, 257.0) }) = 4.76364169072622 degrees
* uni0D91 (U+0D91): Quad(QuadBez { p0: (471.0, 255.0), p1: (469.0, 256.0), p2: (466.0, 257.0) })/Line(Line { p0: (466.0, 257.0), p1: (471.0, 255.0) }) = 3.36646066342994 degrees
* uni0D91 (U+0D91): Quad(QuadBez { p0: (475.0, 252.0), p1: (475.0, 252.0), p2: (473.0, 254.0) })/Line(Line { p0: (473.0, 254.0), p1: (475.0, 252.0) }) = 0.0000012074182697257333 degrees
* uni0D91 (U+0D91): Quad(QuadBez { p0: (479.0, 249.0), p1: (479.0, 249.0), p2: (477.0, 251.0) })/Line(Line { p0: (477.0, 251.0), p1: (479.0, 249.0) }) = 0.0000012074182697257333 degrees
* uni0D91 (U+0D91): Quad(QuadBez { p0: (485.0, 241.0), p1: (485.0, 241.0), p2: (484.0, 243.0) })/Line(Line { p0: (484.0, 243.0), p1: (485.0, 241.0) }) = 0.0000012074182697257333 degrees
* uni0D91 (U+0D91): Quad(QuadBez { p0: (487.0, 236.0), p1: (487.0, 237.0), p2: (486.0, 239.0) })/Line(Line { p0: (486.0, 239.0), p1: (487.0, 236.0) }) = 8.130102354156051 degrees
* uni0D92 (U+0D92): Quad(QuadBez { p0: (78.5, 604.0), p1: (80.0, 604.0), p2: (87.0, 605.0) })/Quad(QuadBez { p0: (87.0, 605.0), p1: (82.0, 605.0), p2: (77.0, 604.0) }) = 8.130102354156005 degrees
* uni0D92 (U+0D92): Line(Line { p0: (466.0, 257.0), p1: (471.0, 255.0) })/Quad(QuadBez { p0: (471.0, 255.0), p1: (469.0, 256.0), p2: (466.0, 257.0) }) = 4.76364169072622 degrees
* uni0D92 (U+0D92): Quad(QuadBez { p0: (471.0, 255.0), p1: (469.0, 256.0), p2: (466.0, 257.0) })/Line(Line { p0: (466.0, 257.0), p1: (471.0, 255.0) }) = 3.36646066342994 degrees
* uni0D92 (U+0D92): Quad(QuadBez { p0: (475.0, 252.0), p1: (475.0, 252.0), p2: (473.0, 254.0) })/Line(Line { p0: (473.0, 254.0), p1: (475.0, 252.0) }) = 0.0000012074182697257333 degrees
* uni0D92 (U+0D92): Quad(QuadBez { p0: (479.0, 249.0), p1: (479.0, 249.0), p2: (477.0, 251.0) })/Line(Line { p0: (477.0, 251.0), p1: (479.0, 249.0) }) = 0.0000012074182697257333 degrees
* uni0D92 (U+0D92): Quad(QuadBez { p0: (485.0, 241.0), p1: (485.0, 241.0), p2: (484.0, 243.0) })/Line(Line { p0: (484.0, 243.0), p1: (485.0, 241.0) }) = 0.0000012074182697257333 degrees
* uni0D92 (U+0D92): Quad(QuadBez { p0: (487.0, 236.0), p1: (487.0, 237.0), p2: (486.0, 239.0) })/Line(Line { p0: (486.0, 239.0), p1: (487.0, 236.0) }) = 8.130102354156051 degrees
* uni0D93 (U+0D93): Quad(QuadBez { p0: (576.5, 604.0), p1: (578.0, 604.0), p2: (585.0, 605.0) })/Quad(QuadBez { p0: (585.0, 605.0), p1: (580.0, 605.0), p2: (575.0, 604.0) }) = 8.130102354156005 degrees
* uni0D93 (U+0D93): Line(Line { p0: (964.0, 257.0), p1: (969.0, 255.0) })/Quad(QuadBez { p0: (969.0, 255.0), p1: (967.0, 256.0), p2: (964.0, 257.0) }) = 4.76364169072622 degrees
* uni0D93 (U+0D93): Quad(QuadBez { p0: (969.0, 255.0), p1: (967.0, 256.0), p2: (964.0, 257.0) })/Line(Line { p0: (964.0, 257.0), p1: (969.0, 255.0) }) = 3.36646066342994 degrees
* uni0D93 (U+0D93): Quad(QuadBez { p0: (973.0, 252.0), p1: (973.0, 252.0), p2: (971.0, 254.0) })/Line(Line { p0: (971.0, 254.0), p1: (973.0, 252.0) }) = 0.0000012074182697257333 degrees
* uni0D93 (U+0D93): Quad(QuadBez { p0: (977.0, 249.0), p1: (977.0, 249.0), p2: (975.0, 251.0) })/Line(Line { p0: (975.0, 251.0), p1: (977.0, 249.0) }) = 0.0000012074182697257333 degrees
* uni0D93 (U+0D93): Quad(QuadBez { p0: (983.0, 241.0), p1: (983.0, 241.0), p2: (982.0, 243.0) })/Line(Line { p0: (982.0, 243.0), p1: (983.0, 241.0) }) = 0.0000012074182697257333 degrees
* uni0D93 (U+0D93): Quad(QuadBez { p0: (985.0, 236.0), p1: (985.0, 237.0), p2: (984.0, 239.0) })/Line(Line { p0: (984.0, 239.0), p1: (985.0, 236.0) }) = 8.130102354156051 degrees
* uni0D9B (U+0D9B): Quad(QuadBez { p0: (315.0, 374.5), p1: (322.0, 380.0), p2: (331.0, 381.0) })/Quad(QuadBez { p0: (331.0, 381.0), p1: (321.0, 382.0), p2: (310.5, 383.0) }) = 12.050784883409548 degrees
* uni0D9B (U+0D9B): Quad(QuadBez { p0: (487.5, 848.5), p1: (484.0, 848.0), p2: (480.0, 848.0) })/Quad(QuadBez { p0: (480.0, 848.0), p1: (485.0, 847.0), p2: (491.0, 846.5) }) = 11.309932474020195 degrees
* uni0DB5 (U+0DB5): Line(Line { p0: (494.0, 257.0), p1: (499.0, 255.0) })/Quad(QuadBez { p0: (499.0, 255.0), p1: (497.0, 256.0), p2: (494.0, 257.0) }) = 4.76364169072622 degrees
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (499.0, 255.0), p1: (497.0, 256.0), p2: (494.0, 257.0) })/Line(Line { p0: (494.0, 257.0), p1: (499.0, 255.0) }) = 3.36646066342994 degrees
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (503.0, 252.0), p1: (503.0, 252.0), p2: (501.0, 254.0) })/Line(Line { p0: (501.0, 254.0), p1: (503.0, 252.0) }) = 0.0000012074182697257333 degrees
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (508.0, 249.0), p1: (508.0, 249.0), p2: (506.0, 251.0) })/Line(Line { p0: (506.0, 251.0), p1: (508.0, 249.0) }) = 0.0000012074182697257333 degrees
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (514.0, 241.0), p1: (514.0, 241.0), p2: (512.0, 243.0) })/Line(Line { p0: (512.0, 243.0), p1: (514.0, 241.0) }) = 0.0000012074182697257333 degrees
* uni0DB8 (U+0DB8): Quad(QuadBez { p0: (162.5, 340.0), p1: (160.0, 337.0), p2: (143.0, 335.0) })/Quad(QuadBez { p0: (143.0, 335.0), p1: (161.0, 334.0), p2: (166.0, 333.0) }) = 9.889666927621194 degrees
* uni0DD4 (U+0DD4): Quad(QuadBez { p0: (-123.0, 49.5), p1: (-95.0, 76.0), p2: (-79.0, 113.0) })/Quad(QuadBez { p0: (-79.0, 113.0), p1: (-80.0, 108.0), p2: (-81.0, 102.5) }) = 12.075288583193501 degrees
* uni0DD6 (U+0DD6): Quad(QuadBez { p0: (-123.0, 49.5), p1: (-95.0, 76.0), p2: (-79.0, 113.0) })/Quad(QuadBez { p0: (-79.0, 113.0), p1: (-80.0, 108.0), p2: (-81.0, 102.5) }) = 12.075288583193501 degrees
* uusignsinh.alt1: Quad(QuadBez { p0: (-100.5, -41.5), p1: (-110.0, -41.0), p2: (-111.0, -41.0) })/Quad(QuadBez { p0: (-111.0, -41.0), p1: (-96.0, -42.0), p2: (-79.0, -50.0) }) = 3.8140748342903783 degrees
* jIsinh: Line(Line { p0: (219.0, 772.0), p1: (225.0, 772.0) })/Quad(QuadBez { p0: (225.0, 772.0), p1: (202.0, 777.0), p2: (180.5, 787.5) }) = 12.2647737278924 degrees
* jIisinh: Line(Line { p0: (219.0, 772.0), p1: (225.0, 772.0) })/Quad(QuadBez { p0: (225.0, 772.0), p1: (202.0, 777.0), p2: (180.5, 787.5) }) = 12.2647737278924 degrees
* four (U+0034): Line(Line { p0: (269.0, 645.0), p1: (274.0, 773.0) })/Quad(QuadBez { p0: (274.0, 773.0), p1: (265.0, 742.0), p2: (249.5, 698.0) }) = 13.9522271935892 degrees [code: found-jaggy-segments]
  
  

</div>
</details>





<details>
    <summary>⚠️ <b>WARN</b> Check there are no overlapping path segments (overlapping_path_segments)</summary>
    <div>








- ⚠️ **WARN** The following glyphs have overlapping path segments:

* uni0D91 (U+0D91): Quad(QuadBez { p0: (46.0, 605.0), p1: (46.0, 605.0), p2: (45.5, 605.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (45.5, 605.0), p1: (45.0, 605.0), p2: (45.0, 605.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (47.0, 604.0), p1: (47.0, 604.0), p2: (47.0, 604.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (48.0, 603.0), p1: (48.0, 603.0), p2: (48.0, 603.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (99.0, 354.0), p1: (99.0, 353.0), p2: (99.0, 353.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (471.0, 255.0), p1: (469.0, 256.0), p2: (466.0, 257.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (475.0, 252.0), p1: (475.0, 252.0), p2: (473.0, 254.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (479.0, 249.0), p1: (479.0, 249.0), p2: (477.0, 251.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (483.0, 245.0), p1: (483.0, 246.0), p2: (481.0, 247.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (485.0, 241.0), p1: (485.0, 241.0), p2: (484.0, 243.0) }) has the same coordinates as a previous segment.
* uni0D91 (U+0D91): Quad(QuadBez { p0: (487.0, 236.0), p1: (487.0, 237.0), p2: (486.0, 239.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (46.0, 605.0), p1: (46.0, 605.0), p2: (45.5, 605.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (45.5, 605.0), p1: (45.0, 605.0), p2: (45.0, 605.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (47.0, 604.0), p1: (47.0, 604.0), p2: (47.0, 604.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (48.0, 603.0), p1: (48.0, 603.0), p2: (48.0, 603.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (99.0, 354.0), p1: (99.0, 353.0), p2: (99.0, 353.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (471.0, 255.0), p1: (469.0, 256.0), p2: (466.0, 257.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (475.0, 252.0), p1: (475.0, 252.0), p2: (473.0, 254.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (479.0, 249.0), p1: (479.0, 249.0), p2: (477.0, 251.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (483.0, 245.0), p1: (483.0, 246.0), p2: (481.0, 247.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (485.0, 241.0), p1: (485.0, 241.0), p2: (484.0, 243.0) }) has the same coordinates as a previous segment.
* uni0D92 (U+0D92): Quad(QuadBez { p0: (487.0, 236.0), p1: (487.0, 237.0), p2: (486.0, 239.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (544.0, 605.0), p1: (544.0, 605.0), p2: (543.5, 605.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (543.5, 605.0), p1: (543.0, 605.0), p2: (543.0, 605.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (545.0, 604.0), p1: (545.0, 604.0), p2: (545.0, 604.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (546.0, 603.0), p1: (546.0, 603.0), p2: (546.0, 603.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (597.0, 354.0), p1: (597.0, 353.0), p2: (597.0, 353.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (969.0, 255.0), p1: (967.0, 256.0), p2: (964.0, 257.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (973.0, 252.0), p1: (973.0, 252.0), p2: (971.0, 254.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (977.0, 249.0), p1: (977.0, 249.0), p2: (975.0, 251.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (981.0, 245.0), p1: (981.0, 246.0), p2: (979.0, 247.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (983.0, 241.0), p1: (983.0, 241.0), p2: (982.0, 243.0) }) has the same coordinates as a previous segment.
* uni0D93 (U+0D93): Quad(QuadBez { p0: (985.0, 236.0), p1: (985.0, 237.0), p2: (984.0, 239.0) }) has the same coordinates as a previous segment.
* uni0D9B (U+0D9B): Quad(QuadBez { p0: (497.0, 477.0), p1: (497.0, 477.0), p2: (497.0, 477.0) }) has the same coordinates as a previous segment.
* uni0D9B (U+0D9B): Line(Line { p0: (494.0, 478.0), p1: (493.0, 479.0) }) has the same coordinates as a previous segment.
* uni0D9B (U+0D9B): Line(Line { p0: (496.0, 477.0), p1: (495.0, 477.0) }) has the same coordinates as a previous segment.
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (499.0, 255.0), p1: (497.0, 256.0), p2: (494.0, 257.0) }) has the same coordinates as a previous segment.
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (503.0, 252.0), p1: (503.0, 252.0), p2: (501.0, 254.0) }) has the same coordinates as a previous segment.
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (508.0, 249.0), p1: (508.0, 249.0), p2: (506.0, 251.0) }) has the same coordinates as a previous segment.
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (511.0, 245.0), p1: (511.0, 246.0), p2: (509.0, 247.0) }) has the same coordinates as a previous segment.
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (514.0, 241.0), p1: (514.0, 241.0), p2: (512.0, 243.0) }) has the same coordinates as a previous segment.
* uni0DB5 (U+0DB5): Quad(QuadBez { p0: (515.0, 236.0), p1: (515.0, 237.0), p2: (515.0, 239.0) }) has the same coordinates as a previous segment. [code: overlapping-path-segments]
  
  

</div>
</details>


</div>
</details>


<details><summary>[1] fonts/ttf</summary>
<div>


<details>
    <summary>⚠️ <b>WARN</b> Ensure Fonts have 'ital' STAT axis. (opentype/STAT/ital_axis)</summary>
    <div>








- ⚠️ **WARN** Static font is missing the 'STAT' table. [code: no-stat-table]
  
  

</div>
</details>


</div>
</details>






### Summary

| ⚠️ WARN | ℹ️ INFO | ✅ PASS | ⏩ SKIP | 
| ---|---|---|---|
| 13 | 11 | 82 | 51 | 
| 8% | 7% | 52% | 32% | 



