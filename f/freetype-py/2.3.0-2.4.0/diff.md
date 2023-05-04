# Comparing `tmp/freetype-py-2.3.0.zip` & `tmp/freetype-py-2.4.0.zip`

## zipinfo {}

```diff
@@ -1,166 +1,172 @@
-Zip file size: 830613 bytes, number of entries: 164
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/freetype_py.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/freetype/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/doc/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/debian/
--rw-r--r--  2.0 unx      409 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/MANIFEST.in
--rw-r--r--  2.0 unx     1143 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/NOTES.txt
--rw-r--r--  2.0 unx     5350 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/README.rst
--rw-r--r--  2.0 unx      718 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/.gitignore
--rw-r--r--  2.0 unx     4460 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/setup.py
--rw-r--r--  2.0 unx      101 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/tox.ini
--rw-r--r--  2.0 unx     6154 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/PKG-INFO
--rw-r--r--  2.0 unx     8048 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/setup-build-freetype.py
--rw-r--r--  2.0 unx      105 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/pyproject.toml
--rw-r--r--  2.0 unx     1585 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/LICENSE.txt
--rw-r--r--  2.0 unx       90 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/setup.cfg
--rw-r--r--  2.0 unx        1 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype_py.egg-info/zip-safe
--rw-r--r--  2.0 unx        9 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype_py.egg-info/top_level.txt
--rw-r--r--  2.0 unx     6154 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype_py.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype_py.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     3685 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype_py.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/
--rw-r--r--  2.0 unx    94542 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/__init__.py
--rw-r--r--  2.0 unx     4522 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_errors.py
--rw-r--r--  2.0 unx    12618 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/raw.py
--rw-r--r--  2.0 unx     5701 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_types.py
--rw-r--r--  2.0 unx    38531 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_structs.py
--rw-r--r--  2.0 unx      825 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_kerning_modes.py
--rw-r--r--  2.0 unx     5634 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/__init__.py
--rw-r--r--  2.0 unx     2276 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_glyph_formats.py
--rw-r--r--  2.0 unx     1984 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_platforms.py
--rw-r--r--  2.0 unx     1578 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_lcd_filters.py
--rw-r--r--  2.0 unx     2216 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_name_ids.py
--rw-r--r--  2.0 unx     1604 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_curve_tags.py
--rw-r--r--  2.0 unx      717 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_style_flags.py
--rw-r--r--  2.0 unx      910 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_stroker_linecaps.py
--rw-r--r--  2.0 unx     9944 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_mac_langids.py
--rw-r--r--  2.0 unx     1169 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_apple_ids.py
--rw-r--r--  2.0 unx     6458 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_load_flags.py
--rw-r--r--  2.0 unx     1131 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_stroker_borders.py
--rw-r--r--  2.0 unx      947 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_open_modes.py
--rw-r--r--  2.0 unx     1001 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_glyph_bbox_modes.py
--rw-r--r--  2.0 unx     2936 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_outline_flags.py
--rw-r--r--  2.0 unx     2438 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_render_modes.py
--rw-r--r--  2.0 unx     1092 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_stroker_linejoins.py
--rw-r--r--  2.0 unx     2564 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_mac_ids.py
--rw-r--r--  2.0 unx      813 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_adobe_ids.py
--rw-r--r--  2.0 unx    23686 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_ms_langids.py
--rw-r--r--  2.0 unx     2456 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_pixel_modes.py
--rw-r--r--  2.0 unx     2490 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_fstypes.py
--rw-r--r--  2.0 unx     2226 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_load_targets.py
--rw-r--r--  2.0 unx     4854 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_face_flags.py
--rw-r--r--  2.0 unx     4019 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/ft_encodings.py
--rw-r--r--  2.0 unx     1525 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/freetype/ft_enums/tt_ms_ids.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/
--rw-r--r--  2.0 unx     1026 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/screenshots.rst
--rw-r--r--  2.0 unx      381 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_adobe_ids.rst
--rw-r--r--  2.0 unx       95 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/bitmap_glyph.rst
--rw-r--r--  2.0 unx     4317 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_mac_langids.rst
--rw-r--r--  2.0 unx     1454 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_platforms.rst
--rw-r--r--  2.0 unx     1040 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/make_enums.py
--rw-r--r--  2.0 unx       89 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/glyph_slot.rst
--rw-r--r--  2.0 unx     1284 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_glyph_formats.rst
--rw-r--r--  2.0 unx     4103 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_load_flags.rst
--rw-r--r--  2.0 unx     7444 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/conf.py
--rw-r--r--  2.0 unx     2635 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_encodings.rst
--rw-r--r--  2.0 unx       81 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/charmap.rst
--rw-r--r--  2.0 unx      601 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/constants.rst
--rw-r--r--  2.0 unx       95 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/size_metrics.rst
--rw-r--r--  2.0 unx       81 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/stroker.rst
--rw-r--r--  2.0 unx     4622 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/Makefile
--rw-r--r--  2.0 unx     1426 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_fstypes.rst
--rw-r--r--  2.0 unx     1654 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_pixel_modes.rst
--rw-r--r--  2.0 unx      446 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_stroker_linecaps.rst
--rw-r--r--  2.0 unx     2185 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_outline_flags.rst
--rw-r--r--  2.0 unx      318 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_style_flags.rst
--rw-r--r--  2.0 unx     1516 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/license.rst
--rw-r--r--  2.0 unx       87 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/sfnt_name.rst
--rw-r--r--  2.0 unx     3794 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_face_flags.rst
--rw-r--r--  2.0 unx      463 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_glyph_bbox_modes.rst
--rw-r--r--  2.0 unx       78 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/bitmap.rst
--rw-r--r--  2.0 unx      731 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_stroker_borders.rst
--rw-r--r--  2.0 unx      485 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/index.rst
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/bitmap_size.rst
--rw-r--r--  2.0 unx       75 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/glyph.rst
--rw-r--r--  2.0 unx      398 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_kerning_modes.rst
--rw-r--r--  2.0 unx      250 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/api.rst
--rw-r--r--  2.0 unx       81 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/outline.rst
--rw-r--r--  2.0 unx     1438 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_load_targets.rst
--rw-r--r--  2.0 unx    10353 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_ms_langids.rst
--rw-r--r--  2.0 unx      473 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_open_modes.rst
--rw-r--r--  2.0 unx     4527 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/make.bat
--rw-r--r--  2.0 unx     1009 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_ms_ids.rst
--rw-r--r--  2.0 unx     1432 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_render_modes.rst
--rw-r--r--  2.0 unx      627 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_stroker_linejoins.rst
--rw-r--r--  2.0 unx     1129 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_mac_ids.rst
--rw-r--r--  2.0 unx      645 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_apple_ids.rst
--rw-r--r--  2.0 unx      147 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/face.rst
--rw-r--r--  2.0 unx      223 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/usage.rst
--rw-r--r--  2.0 unx      934 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/notes.rst
--rw-r--r--  2.0 unx     1104 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/ft_lcd_filters.rst
--rw-r--r--  2.0 unx      915 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/tt_name_ids.rst
--rw-r--r--  2.0 unx       72 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/bbox.rst
--rw-r--r--  2.0 unx   119705 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/wordle.png
--rw-r--r--  2.0 unx    80186 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/opengl.png
--rw-r--r--  2.0 unx    55986 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/S.png
--rw-r--r--  2.0 unx     8697 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/hello-world.png
--rw-r--r--  2.0 unx    98432 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/agg-trick.png
--rw-r--r--  2.0 unx    25701 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/outline.png
--rw-r--r--  2.0 unx    25511 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/doc/_static/G.png
--rw-r--r--  2.0 unx     2601 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/tests/vf_test.py
--rw-r--r--  2.0 unx     1251 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/tests/smoke_test.py
--rw-r--r--  2.0 unx     2222 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/hello-vf.py
--rwxr-xr-x  2.0 unx     2029 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/hello-world-cairo.py
--rw-r--r--  2.0 unx     4486 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/SourceSansVariable-LICENSE.md
--rw-r--r--  2.0 unx     1776 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/hello-world.py
--rw-r--r--  2.0 unx     1887 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/font-info.py
--rw-r--r--  2.0 unx     3765 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-vector-2.py
--rw-r--r--  2.0 unx     3831 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/bitmap_to_surface.py
--rw-r--r--  2.0 unx    12188 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/texture_font.py
--rw-r--r--  2.0 unx     2993 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-color.py
--rw-r--r--  2.0 unx      571 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/emoji-color.py
--rwxr-xr-x  2.0 unx     2997 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-color-cairo.py
--rwxr-xr-x  2.0 unx     6364 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/wordle-cairo.py
--rw-r--r--  2.0 unx     7724 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-metrics.py
--rw-r--r--  2.0 unx     4243 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/ascii.py
--rw-r--r--  2.0 unx     7375 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/subpixel-positioning.py
--rw-r--r--  2.0 unx     2150 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/sfnt-names.py
--rw-r--r--  2.0 unx    65932 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/Vera.ttf
--rwxr-xr-x  2.0 unx     1844 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-outline-cairo.py
--rw-r--r--  2.0 unx     4424 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/opengl.py
--rw-r--r--  2.0 unx     4621 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/wordle.py
--rwxr-xr-x  2.0 unx     3928 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/outline-test.py
--rwxr-xr-x  2.0 unx     4535 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-lcd-cairo.py
--rw-r--r--  2.0 unx     3144 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/example_1.py
--rwxr-xr-x  2.0 unx     2090 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/emoji-color-cairo.py
--rw-r--r--  2.0 unx     2538 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/agg-trick.py
--rwxr-xr-x  2.0 unx     5605 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-vector-2-cairo.py
--rwxr-xr-x  2.0 unx     3207 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/example_1-cairo.py
--rwxr-xr-x  2.0 unx     5743 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-vector-cairo.py
--rw-r--r--  2.0 unx     9578 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/ftdump.py
--rw-r--r--  2.0 unx     1263 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-monochrome.py
--rw-r--r--  2.0 unx     5374 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/shader.py
--rw-r--r--  2.0 unx      987 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-alpha.py
--rw-r--r--  2.0 unx   467920 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/SourceSansVariable-Roman.otf
--rw-r--r--  2.0 unx    49224 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/VeraMono.ttf
--rw-r--r--  2.0 unx     3248 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-vector.py
--rw-r--r--  2.0 unx     1296 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-outline.py
--rw-r--r--  2.0 unx     1312 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-vector-decompose.py
--rwxr-xr-x  2.0 unx     2307 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-mono+alpha-cairo.py
--rw-r--r--  2.0 unx     1032 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/examples/glyph-lcd.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/.github/workflows/
--rw-r--r--  2.0 unx     3205 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/.github/workflows/ci.yml
-drwxr-xr-x  2.0 unx        0 b- stor 22-Apr-25 12:02 freetype-py-2.3.0/debian/source/
--rw-r--r--  2.0 unx      179 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/changelog
--rw-r--r--  2.0 unx        2 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/compat
--rw-r--r--  2.0 unx       70 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/python-freetype-py.lintian-overrides
--rw-r--r--  2.0 unx      513 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/control
--rw-r--r--  2.0 unx     2746 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/copyright
--rwxr-xr-x  2.0 unx      192 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/rules
--rw-r--r--  2.0 unx       12 b- defN 22-Apr-25 12:02 freetype-py-2.3.0/debian/source/format
-164 files, 1494617 bytes uncompressed, 804885 bytes compressed:  46.1%
+Zip file size: 832493 bytes, number of entries: 170
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/debian/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/doc/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/freetype/
+-rw-r--r--  2.0 unx     1585 b- defN 23-May-04 11:28 freetype-py-2.4.0/LICENSE.txt
+-rw-r--r--  2.0 unx       90 b- defN 23-May-04 11:28 freetype-py-2.4.0/setup.cfg
+-rw-r--r--  2.0 unx      105 b- defN 23-May-04 11:28 freetype-py-2.4.0/pyproject.toml
+-rw-r--r--  2.0 unx     4648 b- defN 23-May-04 11:28 freetype-py-2.4.0/setup.py
+-rw-r--r--  2.0 unx     1143 b- defN 23-May-04 11:28 freetype-py-2.4.0/NOTES.txt
+-rw-r--r--  2.0 unx     8040 b- defN 23-May-04 11:28 freetype-py-2.4.0/setup-build-freetype.py
+-rw-r--r--  2.0 unx      101 b- defN 23-May-04 11:28 freetype-py-2.4.0/tox.ini
+-rw-r--r--  2.0 unx     5557 b- defN 23-May-04 11:28 freetype-py-2.4.0/README.rst
+-rw-r--r--  2.0 unx      718 b- defN 23-May-04 11:28 freetype-py-2.4.0/.gitignore
+-rw-r--r--  2.0 unx      409 b- defN 23-May-04 11:28 freetype-py-2.4.0/MANIFEST.in
+-rw-r--r--  2.0 unx     6361 b- defN 23-May-04 11:28 freetype-py-2.4.0/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/.github/workflows/
+-rw-r--r--  2.0 unx     3650 b- defN 23-May-04 11:28 freetype-py-2.4.0/.github/workflows/ci.yml
+-rwxr-xr-x  2.0 unx     6364 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/wordle-cairo.py
+-rw-r--r--  2.0 unx     4243 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/ascii.py
+-rw-r--r--  2.0 unx    12188 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/texture_font.py
+-rwxr-xr-x  2.0 unx     2997 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-color-cairo.py
+-rw-r--r--  2.0 unx     3248 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-vector.py
+-rw-r--r--  2.0 unx     1312 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-vector-decompose.py
+-rw-r--r--  2.0 unx     3144 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/example_1.py
+-rw-r--r--  2.0 unx     5374 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/shader.py
+-rwxr-xr-x  2.0 unx     3207 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/example_1-cairo.py
+-rwxr-xr-x  2.0 unx     3928 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/outline-test.py
+-rw-r--r--  2.0 unx     7724 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-metrics.py
+-rw-r--r--  2.0 unx     3831 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/bitmap_to_surface.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/font-info.py
+-rw-r--r--  2.0 unx     1786 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/hello-world.py
+-rw-r--r--  2.0 unx     2993 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-color.py
+-rwxr-xr-x  2.0 unx     2034 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/hello-world-cairo.py
+-rw-r--r--  2.0 unx     1032 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-lcd.py
+-rw-r--r--  2.0 unx     3765 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-vector-2.py
+-rw-r--r--  2.0 unx     4621 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/wordle.py
+-rw-r--r--  2.0 unx     4486 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/SourceSansVariable-LICENSE.md
+-rw-r--r--  2.0 unx     2236 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/hello-vf.py
+-rwxr-xr-x  2.0 unx     1844 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-outline-cairo.py
+-rwxr-xr-x  2.0 unx     5743 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-vector-cairo.py
+-rw-r--r--  2.0 unx     1263 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-monochrome.py
+-rwxr-xr-x  2.0 unx     2307 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-mono+alpha-cairo.py
+-rw-r--r--  2.0 unx     2538 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/agg-trick.py
+-rw-r--r--  2.0 unx     1296 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-outline.py
+-rw-r--r--  2.0 unx   467920 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/SourceSansVariable-Roman.otf
+-rw-r--r--  2.0 unx     2150 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/sfnt-names.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/emoji-color.py
+-rw-r--r--  2.0 unx    49224 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/VeraMono.ttf
+-rw-r--r--  2.0 unx     4424 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/opengl.py
+-rw-r--r--  2.0 unx     7375 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/subpixel-positioning.py
+-rw-r--r--  2.0 unx     9578 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/ftdump.py
+-rw-r--r--  2.0 unx    65932 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/Vera.ttf
+-rwxr-xr-x  2.0 unx     4535 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-lcd-cairo.py
+-rwxr-xr-x  2.0 unx     5605 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-vector-2-cairo.py
+-rw-r--r--  2.0 unx      987 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/glyph-alpha.py
+-rwxr-xr-x  2.0 unx     2090 b- defN 23-May-04 11:28 freetype-py-2.4.0/examples/emoji-color-cairo.py
+-rw-r--r--  2.0 unx      111 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3873 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/zip-safe
+-rw-r--r--  2.0 unx     6361 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype_py.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/debian/source/
+-rw-r--r--  2.0 unx      513 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/control
+-rw-r--r--  2.0 unx        2 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/compat
+-rw-r--r--  2.0 unx       70 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/python-freetype-py.lintian-overrides
+-rw-r--r--  2.0 unx     2746 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/copyright
+-rwxr-xr-x  2.0 unx      192 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/rules
+-rw-r--r--  2.0 unx      179 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/changelog
+-rw-r--r--  2.0 unx       12 b- defN 23-May-04 11:28 freetype-py-2.4.0/debian/source/format
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-04 11:28 freetype-py-2.4.0/tests/vf_test.py
+-rw-r--r--  2.0 unx     1251 b- defN 23-May-04 11:28 freetype-py-2.4.0/tests/smoke_test.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/doc/_static/
+-rw-r--r--  2.0 unx     1040 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/make_enums.py
+-rw-r--r--  2.0 unx      485 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/index.rst
+-rw-r--r--  2.0 unx      627 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_stroker_linejoins.rst
+-rw-r--r--  2.0 unx       95 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/size_metrics.rst
+-rw-r--r--  2.0 unx     1284 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_glyph_formats.rst
+-rw-r--r--  2.0 unx      446 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_stroker_linecaps.rst
+-rw-r--r--  2.0 unx       78 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/bitmap.rst
+-rw-r--r--  2.0 unx      731 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_stroker_borders.rst
+-rw-r--r--  2.0 unx     1432 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_render_modes.rst
+-rw-r--r--  2.0 unx     1654 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_pixel_modes.rst
+-rw-r--r--  2.0 unx     1438 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_load_targets.rst
+-rw-r--r--  2.0 unx       81 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/outline.rst
+-rw-r--r--  2.0 unx      934 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/notes.rst
+-rw-r--r--  2.0 unx      645 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_apple_ids.rst
+-rw-r--r--  2.0 unx     1426 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_fstypes.rst
+-rw-r--r--  2.0 unx       95 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/bitmap_glyph.rst
+-rw-r--r--  2.0 unx     2635 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_encodings.rst
+-rw-r--r--  2.0 unx      381 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_adobe_ids.rst
+-rw-r--r--  2.0 unx      223 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/usage.rst
+-rw-r--r--  2.0 unx     1454 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_platforms.rst
+-rw-r--r--  2.0 unx       87 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/sfnt_name.rst
+-rw-r--r--  2.0 unx      473 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_open_modes.rst
+-rw-r--r--  2.0 unx      318 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_style_flags.rst
+-rw-r--r--  2.0 unx     7444 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/conf.py
+-rw-r--r--  2.0 unx    10353 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_ms_langids.rst
+-rw-r--r--  2.0 unx      398 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_kerning_modes.rst
+-rw-r--r--  2.0 unx     1009 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_ms_ids.rst
+-rw-r--r--  2.0 unx      601 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/constants.rst
+-rw-r--r--  2.0 unx     3794 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_face_flags.rst
+-rw-r--r--  2.0 unx      463 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_glyph_bbox_modes.rst
+-rw-r--r--  2.0 unx       81 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/stroker.rst
+-rw-r--r--  2.0 unx     4622 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/Makefile
+-rw-r--r--  2.0 unx       81 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/charmap.rst
+-rw-r--r--  2.0 unx       89 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/glyph_slot.rst
+-rw-r--r--  2.0 unx     1104 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_lcd_filters.rst
+-rw-r--r--  2.0 unx      250 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/api.rst
+-rw-r--r--  2.0 unx     4527 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/make.bat
+-rw-r--r--  2.0 unx     4317 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_mac_langids.rst
+-rw-r--r--  2.0 unx     2185 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_outline_flags.rst
+-rw-r--r--  2.0 unx       75 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/glyph.rst
+-rw-r--r--  2.0 unx       72 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/bbox.rst
+-rw-r--r--  2.0 unx      915 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_name_ids.rst
+-rw-r--r--  2.0 unx     4103 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/ft_load_flags.rst
+-rw-r--r--  2.0 unx     1516 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/license.rst
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/bitmap_size.rst
+-rw-r--r--  2.0 unx     1026 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/screenshots.rst
+-rw-r--r--  2.0 unx     1129 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/tt_mac_ids.rst
+-rw-r--r--  2.0 unx      147 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/face.rst
+-rw-r--r--  2.0 unx    55986 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/S.png
+-rw-r--r--  2.0 unx    25701 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/outline.png
+-rw-r--r--  2.0 unx    98432 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/agg-trick.png
+-rw-r--r--  2.0 unx    80186 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/opengl.png
+-rw-r--r--  2.0 unx   119705 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/wordle.png
+-rw-r--r--  2.0 unx    25511 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/G.png
+-rw-r--r--  2.0 unx     8697 b- defN 23-May-04 11:28 freetype-py-2.4.0/doc/_static/hello-world.png
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 11:28 freetype-py-2.4.0/freetype/__pyinstaller/
+-rw-r--r--  2.0 unx    94490 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/__init__.py
+-rw-r--r--  2.0 unx    38531 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_structs.py
+-rw-r--r--  2.0 unx     5701 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_types.py
+-rw-r--r--  2.0 unx    12618 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/raw.py
+-rw-r--r--  2.0 unx     4522 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_errors.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_stroker_linejoins.py
+-rw-r--r--  2.0 unx     9944 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_mac_langids.py
+-rw-r--r--  2.0 unx     4019 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_encodings.py
+-rw-r--r--  2.0 unx     1001 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_glyph_bbox_modes.py
+-rw-r--r--  2.0 unx     2936 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_outline_flags.py
+-rw-r--r--  2.0 unx     1984 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_platforms.py
+-rw-r--r--  2.0 unx      825 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_kerning_modes.py
+-rw-r--r--  2.0 unx     6458 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_load_flags.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_apple_ids.py
+-rw-r--r--  2.0 unx     2490 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_fstypes.py
+-rw-r--r--  2.0 unx     4854 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_face_flags.py
+-rw-r--r--  2.0 unx     5634 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_style_flags.py
+-rw-r--r--  2.0 unx     2216 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_name_ids.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_stroker_borders.py
+-rw-r--r--  2.0 unx     1578 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_lcd_filters.py
+-rw-r--r--  2.0 unx     1525 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_ms_ids.py
+-rw-r--r--  2.0 unx     1604 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_curve_tags.py
+-rw-r--r--  2.0 unx     2276 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_glyph_formats.py
+-rw-r--r--  2.0 unx      947 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_open_modes.py
+-rw-r--r--  2.0 unx      813 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_adobe_ids.py
+-rw-r--r--  2.0 unx     2564 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_mac_ids.py
+-rw-r--r--  2.0 unx    23686 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/tt_ms_langids.py
+-rw-r--r--  2.0 unx     2456 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_pixel_modes.py
+-rw-r--r--  2.0 unx     2226 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_load_targets.py
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_render_modes.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/ft_enums/ft_stroker_linecaps.py
+-rw-r--r--  2.0 unx       41 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/__pyinstaller/conftest.py
+-rw-r--r--  2.0 unx      119 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/__pyinstaller/test_freetype.py
+-rw-r--r--  2.0 unx      137 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/__pyinstaller/__init__.py
+-rw-r--r--  2.0 unx      103 b- defN 23-May-04 11:28 freetype-py-2.4.0/freetype/__pyinstaller/hook-freetype.py
+170 files, 1496539 bytes uncompressed, 805681 bytes compressed:  46.2%
```

## zipnote {}

```diff
@@ -1,493 +1,511 @@
-Filename: freetype-py-2.3.0/
+Filename: freetype-py-2.4.0/
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype_py.egg-info/
+Filename: freetype-py-2.4.0/.github/
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/
+Filename: freetype-py-2.4.0/examples/
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/
+Filename: freetype-py-2.4.0/freetype_py.egg-info/
 Comment: 
 
-Filename: freetype-py-2.3.0/tests/
+Filename: freetype-py-2.4.0/debian/
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/
+Filename: freetype-py-2.4.0/tests/
 Comment: 
 
-Filename: freetype-py-2.3.0/.github/
+Filename: freetype-py-2.4.0/doc/
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/
+Filename: freetype-py-2.4.0/freetype/
 Comment: 
 
-Filename: freetype-py-2.3.0/MANIFEST.in
+Filename: freetype-py-2.4.0/LICENSE.txt
 Comment: 
 
-Filename: freetype-py-2.3.0/NOTES.txt
+Filename: freetype-py-2.4.0/setup.cfg
 Comment: 
 
-Filename: freetype-py-2.3.0/README.rst
+Filename: freetype-py-2.4.0/pyproject.toml
 Comment: 
 
-Filename: freetype-py-2.3.0/.gitignore
+Filename: freetype-py-2.4.0/setup.py
 Comment: 
 
-Filename: freetype-py-2.3.0/setup.py
+Filename: freetype-py-2.4.0/NOTES.txt
 Comment: 
 
-Filename: freetype-py-2.3.0/tox.ini
+Filename: freetype-py-2.4.0/setup-build-freetype.py
 Comment: 
 
-Filename: freetype-py-2.3.0/PKG-INFO
+Filename: freetype-py-2.4.0/tox.ini
 Comment: 
 
-Filename: freetype-py-2.3.0/setup-build-freetype.py
+Filename: freetype-py-2.4.0/README.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/pyproject.toml
+Filename: freetype-py-2.4.0/.gitignore
 Comment: 
 
-Filename: freetype-py-2.3.0/LICENSE.txt
+Filename: freetype-py-2.4.0/MANIFEST.in
 Comment: 
 
-Filename: freetype-py-2.3.0/setup.cfg
+Filename: freetype-py-2.4.0/PKG-INFO
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype_py.egg-info/zip-safe
+Filename: freetype-py-2.4.0/.github/workflows/
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype_py.egg-info/top_level.txt
+Filename: freetype-py-2.4.0/.github/workflows/ci.yml
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype_py.egg-info/PKG-INFO
+Filename: freetype-py-2.4.0/examples/wordle-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype_py.egg-info/dependency_links.txt
+Filename: freetype-py-2.4.0/examples/ascii.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype_py.egg-info/SOURCES.txt
+Filename: freetype-py-2.4.0/examples/texture_font.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/
+Filename: freetype-py-2.4.0/examples/glyph-color-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/__init__.py
+Filename: freetype-py-2.4.0/examples/glyph-vector.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_errors.py
+Filename: freetype-py-2.4.0/examples/glyph-vector-decompose.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/raw.py
+Filename: freetype-py-2.4.0/examples/example_1.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_types.py
+Filename: freetype-py-2.4.0/examples/shader.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_structs.py
+Filename: freetype-py-2.4.0/examples/example_1-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_kerning_modes.py
+Filename: freetype-py-2.4.0/examples/outline-test.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/__init__.py
+Filename: freetype-py-2.4.0/examples/glyph-metrics.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_glyph_formats.py
+Filename: freetype-py-2.4.0/examples/bitmap_to_surface.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_platforms.py
+Filename: freetype-py-2.4.0/examples/font-info.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_lcd_filters.py
+Filename: freetype-py-2.4.0/examples/hello-world.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_name_ids.py
+Filename: freetype-py-2.4.0/examples/glyph-color.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_curve_tags.py
+Filename: freetype-py-2.4.0/examples/hello-world-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_style_flags.py
+Filename: freetype-py-2.4.0/examples/glyph-lcd.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_stroker_linecaps.py
+Filename: freetype-py-2.4.0/examples/glyph-vector-2.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_mac_langids.py
+Filename: freetype-py-2.4.0/examples/wordle.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_apple_ids.py
+Filename: freetype-py-2.4.0/examples/SourceSansVariable-LICENSE.md
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_load_flags.py
+Filename: freetype-py-2.4.0/examples/hello-vf.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_stroker_borders.py
+Filename: freetype-py-2.4.0/examples/glyph-outline-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_open_modes.py
+Filename: freetype-py-2.4.0/examples/glyph-vector-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_glyph_bbox_modes.py
+Filename: freetype-py-2.4.0/examples/glyph-monochrome.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_outline_flags.py
+Filename: freetype-py-2.4.0/examples/glyph-mono+alpha-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_render_modes.py
+Filename: freetype-py-2.4.0/examples/agg-trick.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_stroker_linejoins.py
+Filename: freetype-py-2.4.0/examples/glyph-outline.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_mac_ids.py
+Filename: freetype-py-2.4.0/examples/SourceSansVariable-Roman.otf
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_adobe_ids.py
+Filename: freetype-py-2.4.0/examples/sfnt-names.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_ms_langids.py
+Filename: freetype-py-2.4.0/examples/emoji-color.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_pixel_modes.py
+Filename: freetype-py-2.4.0/examples/VeraMono.ttf
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_fstypes.py
+Filename: freetype-py-2.4.0/examples/opengl.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_load_targets.py
+Filename: freetype-py-2.4.0/examples/subpixel-positioning.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_face_flags.py
+Filename: freetype-py-2.4.0/examples/ftdump.py
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/ft_encodings.py
+Filename: freetype-py-2.4.0/examples/Vera.ttf
 Comment: 
 
-Filename: freetype-py-2.3.0/freetype/ft_enums/tt_ms_ids.py
+Filename: freetype-py-2.4.0/examples/glyph-lcd-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/
+Filename: freetype-py-2.4.0/examples/glyph-vector-2-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/screenshots.rst
+Filename: freetype-py-2.4.0/examples/glyph-alpha.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_adobe_ids.rst
+Filename: freetype-py-2.4.0/examples/emoji-color-cairo.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/bitmap_glyph.rst
+Filename: freetype-py-2.4.0/freetype_py.egg-info/entry_points.txt
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_mac_langids.rst
+Filename: freetype-py-2.4.0/freetype_py.egg-info/top_level.txt
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_platforms.rst
+Filename: freetype-py-2.4.0/freetype_py.egg-info/SOURCES.txt
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/make_enums.py
+Filename: freetype-py-2.4.0/freetype_py.egg-info/zip-safe
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/glyph_slot.rst
+Filename: freetype-py-2.4.0/freetype_py.egg-info/PKG-INFO
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_glyph_formats.rst
+Filename: freetype-py-2.4.0/freetype_py.egg-info/dependency_links.txt
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_load_flags.rst
+Filename: freetype-py-2.4.0/debian/source/
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/conf.py
+Filename: freetype-py-2.4.0/debian/control
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_encodings.rst
+Filename: freetype-py-2.4.0/debian/compat
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/charmap.rst
+Filename: freetype-py-2.4.0/debian/python-freetype-py.lintian-overrides
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/constants.rst
+Filename: freetype-py-2.4.0/debian/copyright
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/size_metrics.rst
+Filename: freetype-py-2.4.0/debian/rules
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/stroker.rst
+Filename: freetype-py-2.4.0/debian/changelog
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/Makefile
+Filename: freetype-py-2.4.0/debian/source/format
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_fstypes.rst
+Filename: freetype-py-2.4.0/tests/vf_test.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_pixel_modes.rst
+Filename: freetype-py-2.4.0/tests/smoke_test.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_stroker_linecaps.rst
+Filename: freetype-py-2.4.0/doc/_static/
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_outline_flags.rst
+Filename: freetype-py-2.4.0/doc/make_enums.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_style_flags.rst
+Filename: freetype-py-2.4.0/doc/index.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/license.rst
+Filename: freetype-py-2.4.0/doc/ft_stroker_linejoins.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/sfnt_name.rst
+Filename: freetype-py-2.4.0/doc/size_metrics.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_face_flags.rst
+Filename: freetype-py-2.4.0/doc/ft_glyph_formats.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_glyph_bbox_modes.rst
+Filename: freetype-py-2.4.0/doc/ft_stroker_linecaps.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/bitmap.rst
+Filename: freetype-py-2.4.0/doc/bitmap.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_stroker_borders.rst
+Filename: freetype-py-2.4.0/doc/ft_stroker_borders.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/index.rst
+Filename: freetype-py-2.4.0/doc/ft_render_modes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/bitmap_size.rst
+Filename: freetype-py-2.4.0/doc/ft_pixel_modes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/glyph.rst
+Filename: freetype-py-2.4.0/doc/ft_load_targets.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_kerning_modes.rst
+Filename: freetype-py-2.4.0/doc/outline.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/api.rst
+Filename: freetype-py-2.4.0/doc/notes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/outline.rst
+Filename: freetype-py-2.4.0/doc/tt_apple_ids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_load_targets.rst
+Filename: freetype-py-2.4.0/doc/ft_fstypes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_ms_langids.rst
+Filename: freetype-py-2.4.0/doc/bitmap_glyph.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_open_modes.rst
+Filename: freetype-py-2.4.0/doc/ft_encodings.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/make.bat
+Filename: freetype-py-2.4.0/doc/tt_adobe_ids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_ms_ids.rst
+Filename: freetype-py-2.4.0/doc/usage.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_render_modes.rst
+Filename: freetype-py-2.4.0/doc/tt_platforms.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_stroker_linejoins.rst
+Filename: freetype-py-2.4.0/doc/sfnt_name.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_mac_ids.rst
+Filename: freetype-py-2.4.0/doc/ft_open_modes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_apple_ids.rst
+Filename: freetype-py-2.4.0/doc/ft_style_flags.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/face.rst
+Filename: freetype-py-2.4.0/doc/conf.py
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/usage.rst
+Filename: freetype-py-2.4.0/doc/tt_ms_langids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/notes.rst
+Filename: freetype-py-2.4.0/doc/ft_kerning_modes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/ft_lcd_filters.rst
+Filename: freetype-py-2.4.0/doc/tt_ms_ids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/tt_name_ids.rst
+Filename: freetype-py-2.4.0/doc/constants.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/bbox.rst
+Filename: freetype-py-2.4.0/doc/ft_face_flags.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/wordle.png
+Filename: freetype-py-2.4.0/doc/ft_glyph_bbox_modes.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/opengl.png
+Filename: freetype-py-2.4.0/doc/stroker.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/S.png
+Filename: freetype-py-2.4.0/doc/Makefile
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/hello-world.png
+Filename: freetype-py-2.4.0/doc/charmap.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/agg-trick.png
+Filename: freetype-py-2.4.0/doc/glyph_slot.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/outline.png
+Filename: freetype-py-2.4.0/doc/ft_lcd_filters.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/doc/_static/G.png
+Filename: freetype-py-2.4.0/doc/api.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/tests/vf_test.py
+Filename: freetype-py-2.4.0/doc/make.bat
 Comment: 
 
-Filename: freetype-py-2.3.0/tests/smoke_test.py
+Filename: freetype-py-2.4.0/doc/tt_mac_langids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/hello-vf.py
+Filename: freetype-py-2.4.0/doc/ft_outline_flags.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/hello-world-cairo.py
+Filename: freetype-py-2.4.0/doc/glyph.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/SourceSansVariable-LICENSE.md
+Filename: freetype-py-2.4.0/doc/bbox.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/hello-world.py
+Filename: freetype-py-2.4.0/doc/tt_name_ids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/font-info.py
+Filename: freetype-py-2.4.0/doc/ft_load_flags.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-vector-2.py
+Filename: freetype-py-2.4.0/doc/license.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/bitmap_to_surface.py
+Filename: freetype-py-2.4.0/doc/bitmap_size.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/texture_font.py
+Filename: freetype-py-2.4.0/doc/screenshots.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-color.py
+Filename: freetype-py-2.4.0/doc/tt_mac_ids.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/emoji-color.py
+Filename: freetype-py-2.4.0/doc/face.rst
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-color-cairo.py
+Filename: freetype-py-2.4.0/doc/_static/S.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/wordle-cairo.py
+Filename: freetype-py-2.4.0/doc/_static/outline.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-metrics.py
+Filename: freetype-py-2.4.0/doc/_static/agg-trick.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/ascii.py
+Filename: freetype-py-2.4.0/doc/_static/opengl.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/subpixel-positioning.py
+Filename: freetype-py-2.4.0/doc/_static/wordle.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/sfnt-names.py
+Filename: freetype-py-2.4.0/doc/_static/G.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/Vera.ttf
+Filename: freetype-py-2.4.0/doc/_static/hello-world.png
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-outline-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/opengl.py
+Filename: freetype-py-2.4.0/freetype/__pyinstaller/
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/wordle.py
+Filename: freetype-py-2.4.0/freetype/__init__.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/outline-test.py
+Filename: freetype-py-2.4.0/freetype/ft_structs.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-lcd-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_types.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/example_1.py
+Filename: freetype-py-2.4.0/freetype/raw.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/emoji-color-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_errors.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/agg-trick.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_stroker_linejoins.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-vector-2-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_mac_langids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/example_1-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_encodings.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-vector-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_glyph_bbox_modes.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/ftdump.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_outline_flags.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-monochrome.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_platforms.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/shader.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_kerning_modes.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-alpha.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_load_flags.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/SourceSansVariable-Roman.otf
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_apple_ids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/VeraMono.ttf
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_fstypes.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-vector.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_face_flags.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-outline.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/__init__.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-vector-decompose.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_style_flags.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-mono+alpha-cairo.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_name_ids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/examples/glyph-lcd.py
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_stroker_borders.py
 Comment: 
 
-Filename: freetype-py-2.3.0/.github/workflows/
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_lcd_filters.py
 Comment: 
 
-Filename: freetype-py-2.3.0/.github/workflows/ci.yml
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_ms_ids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/source/
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_curve_tags.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/changelog
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_glyph_formats.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/compat
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_open_modes.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/python-freetype-py.lintian-overrides
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_adobe_ids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/control
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_mac_ids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/copyright
+Filename: freetype-py-2.4.0/freetype/ft_enums/tt_ms_langids.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/rules
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_pixel_modes.py
 Comment: 
 
-Filename: freetype-py-2.3.0/debian/source/format
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_load_targets.py
+Comment: 
+
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_render_modes.py
+Comment: 
+
+Filename: freetype-py-2.4.0/freetype/ft_enums/ft_stroker_linecaps.py
+Comment: 
+
+Filename: freetype-py-2.4.0/freetype/__pyinstaller/conftest.py
+Comment: 
+
+Filename: freetype-py-2.4.0/freetype/__pyinstaller/test_freetype.py
+Comment: 
+
+Filename: freetype-py-2.4.0/freetype/__pyinstaller/__init__.py
+Comment: 
+
+Filename: freetype-py-2.4.0/freetype/__pyinstaller/hook-freetype.py
 Comment: 
 
 Zip file comment:
```

## Comparing `freetype-py-2.3.0/NOTES.txt` & `freetype-py-2.4.0/NOTES.txt`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/README.rst` & `freetype-py-2.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -130,7 +130,14 @@
 The screenshot below comes from the agg-trick.py example showing an
 implementation of ideas from the `Texts Rasterization Exposures
 <http://agg.sourceforge.net/antigrain.com/research/font_rasterization/>`_ by
 Maxim Shemarev.
 
 .. image:: https://raw.githubusercontent.com/rougier/freetype-py/master/doc/_static/agg-trick.png
 
+
+Freezing apps
+=============
+
+Freetype implements a hook for PyInstaller to help simplify the freezing process
+(it e.g. ensures that the freetype DLL is included). This hook requires
+PyInstaller version 4+.
```

## Comparing `freetype-py-2.3.0/.gitignore` & `freetype-py-2.4.0/.gitignore`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/setup.py` & `freetype-py-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,8 +124,14 @@
         'Operating System :: POSIX',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
         'Topic :: Multimedia :: Graphics',
     ],
     keywords=['freetype', 'font'],
     setup_requires=['setuptools_scm'],
+    entry_points={
+        "pyinstaller40": [
+            "hook-dirs = freetype.__pyinstaller:get_hook_dirs",
+            "tests = freetype.__pyinstaller:get_test_dirs",
+        ],
+    },
 )
```

## Comparing `freetype-py-2.3.0/PKG-INFO` & `freetype-py-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freetype-py
-Version: 2.3.0
+Version: 2.4.0
 Summary: Freetype python bindings
 Home-page: https://github.com/rougier/freetype-py
 Author: Nicolas P. Rougier
 Author-email: Nicolas.Rougier@inria.fr
 License: UNKNOWN
 Keywords: freetype,font
 Platform: UNKNOWN
@@ -155,8 +155,15 @@
 implementation of ideas from the `Texts Rasterization Exposures
 <http://agg.sourceforge.net/antigrain.com/research/font_rasterization/>`_ by
 Maxim Shemarev.
 
 .. image:: https://raw.githubusercontent.com/rougier/freetype-py/master/doc/_static/agg-trick.png
 
 
+Freezing apps
+=============
+
+Freetype implements a hook for PyInstaller to help simplify the freezing process
+(it e.g. ensures that the freetype DLL is included). This hook requires
+PyInstaller version 4+.
+
```

## Comparing `freetype-py-2.3.0/setup-build-freetype.py` & `freetype-py-2.4.0/setup-build-freetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 import urllib.request
 from os import path
 import platform
 
 # Needed for the GitHub Actions macOS CI runner, which appears to come without CAs.
 import certifi
 
-FREETYPE_HOST = "https://download.savannah.gnu.org/releases/freetype/"
-FREETYPE_TARBALL = "freetype-2.12.0.tar.xz"
+FREETYPE_HOST = "https://mirrors.sarata.com/non-gnu/freetype/"
+FREETYPE_TARBALL = "freetype-2.13.0.tar.xz"
 FREETYPE_URL = FREETYPE_HOST + FREETYPE_TARBALL
-FREETYPE_SHA256 = "ef5c336aacc1a079ff9262d6308d6c2a066dd4d2a905301c4adda9b354399033"
-HARFBUZZ_HOST = "https://github.com/harfbuzz/harfbuzz/releases/download/4.2.1/"
-HARFBUZZ_TARBALL = "harfbuzz-4.2.1.tar.xz"
+FREETYPE_SHA256 = "5ee23abd047636c24b2d43c6625dcafc66661d1aca64dec9e0d05df29592624c"
+HARFBUZZ_HOST = "https://github.com/harfbuzz/harfbuzz/releases/download/7.2.0/"
+HARFBUZZ_TARBALL = "harfbuzz-7.2.0.tar.xz"
 HARFBUZZ_URL = HARFBUZZ_HOST + HARFBUZZ_TARBALL
-HARFBUZZ_SHA256 = "bd17916513829aeff961359a5ccebba6de2f4bf37a91faee3ac29c120e3d7ee1"
+HARFBUZZ_SHA256 = "fc5560c807eae0efd5f95b5aa4c65800c7a8eed6642008a6b1e7e3ffff7873cc"
 
 root_dir = "."
 build_dir = path.join(root_dir, "build")
 # CMake requires an absolute path to a prefix.
 prefix_dir = path.abspath(path.join(build_dir, "local"))
 lib_dir = path.join(prefix_dir, "lib")
 build_dir_ft = path.join(build_dir, FREETYPE_TARBALL.split(".tar")[0], "build")
```

## Comparing `freetype-py-2.3.0/LICENSE.txt` & `freetype-py-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype_py.egg-info/PKG-INFO` & `freetype-py-2.4.0/freetype_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freetype-py
-Version: 2.3.0
+Version: 2.4.0
 Summary: Freetype python bindings
 Home-page: https://github.com/rougier/freetype-py
 Author: Nicolas P. Rougier
 Author-email: Nicolas.Rougier@inria.fr
 License: UNKNOWN
 Keywords: freetype,font
 Platform: UNKNOWN
@@ -155,8 +155,15 @@
 implementation of ideas from the `Texts Rasterization Exposures
 <http://agg.sourceforge.net/antigrain.com/research/font_rasterization/>`_ by
 Maxim Shemarev.
 
 .. image:: https://raw.githubusercontent.com/rougier/freetype-py/master/doc/_static/agg-trick.png
 
 
+Freezing apps
+=============
+
+Freetype implements a hook for PyInstaller to help simplify the freezing process
+(it e.g. ensures that the freetype DLL is included). This hook requires
+PyInstaller version 4+.
+
```

## Comparing `freetype-py-2.3.0/freetype_py.egg-info/SOURCES.txt` & `freetype-py-2.4.0/freetype_py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 examples/wordle-cairo.py
 examples/wordle.py
 freetype/__init__.py
 freetype/ft_errors.py
 freetype/ft_structs.py
 freetype/ft_types.py
 freetype/raw.py
+freetype/__pyinstaller/__init__.py
+freetype/__pyinstaller/conftest.py
+freetype/__pyinstaller/hook-freetype.py
+freetype/__pyinstaller/test_freetype.py
 freetype/ft_enums/__init__.py
 freetype/ft_enums/ft_curve_tags.py
 freetype/ft_enums/ft_encodings.py
 freetype/ft_enums/ft_face_flags.py
 freetype/ft_enums/ft_fstypes.py
 freetype/ft_enums/ft_glyph_bbox_modes.py
 freetype/ft_enums/ft_glyph_formats.py
@@ -141,11 +145,12 @@
 freetype/ft_enums/tt_ms_ids.py
 freetype/ft_enums/tt_ms_langids.py
 freetype/ft_enums/tt_name_ids.py
 freetype/ft_enums/tt_platforms.py
 freetype_py.egg-info/PKG-INFO
 freetype_py.egg-info/SOURCES.txt
 freetype_py.egg-info/dependency_links.txt
+freetype_py.egg-info/entry_points.txt
 freetype_py.egg-info/top_level.txt
 freetype_py.egg-info/zip-safe
 tests/smoke_test.py
 tests/vf_test.py
```

## Comparing `freetype-py-2.3.0/freetype/__init__.py` & `freetype-py-2.4.0/freetype/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -895,16 +895,15 @@
           To get the bbox in pixel coordinates, set 'bbox_mode' to
           FT_GLYPH_BBOX_TRUNCATE.
 
           To get the bbox in grid-fitted pixel coordinates, set 'bbox_mode' to
           FT_GLYPH_BBOX_PIXELS.
         '''
         bbox = FT_BBox()
-        error = FT_Glyph_Get_CBox(byref(self._FT_Glyph.contents), bbox_mode, byref(bbox))
-        if error: raise FT_Exception(error)
+        FT_Glyph_Get_CBox(byref(self._FT_Glyph.contents), bbox_mode, byref(bbox))
         return BBox(bbox)
 
 
 
 # -----------------------------------------------------------------------------
 class BitmapGlyph( object ):
     '''
```

## Comparing `freetype-py-2.3.0/freetype/ft_errors.py` & `freetype-py-2.4.0/freetype/ft_errors.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/raw.py` & `freetype-py-2.4.0/freetype/raw.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_types.py` & `freetype-py-2.4.0/freetype/ft_types.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_structs.py` & `freetype-py-2.4.0/freetype/ft_structs.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_kerning_modes.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_kerning_modes.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/__init__.py` & `freetype-py-2.4.0/freetype/ft_enums/__init__.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_glyph_formats.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_glyph_formats.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_platforms.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_platforms.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_lcd_filters.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_lcd_filters.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_name_ids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_name_ids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_curve_tags.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_curve_tags.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_style_flags.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_style_flags.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_stroker_linecaps.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_stroker_linecaps.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_mac_langids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_mac_langids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_apple_ids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_apple_ids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_load_flags.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_load_flags.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_stroker_borders.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_stroker_borders.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_open_modes.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_open_modes.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_glyph_bbox_modes.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_glyph_bbox_modes.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_outline_flags.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_outline_flags.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_render_modes.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_render_modes.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_stroker_linejoins.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_stroker_linejoins.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_mac_ids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_mac_ids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_adobe_ids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_adobe_ids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_ms_langids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_ms_langids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_pixel_modes.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_pixel_modes.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_fstypes.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_fstypes.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_load_targets.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_load_targets.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_face_flags.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_face_flags.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/ft_encodings.py` & `freetype-py-2.4.0/freetype/ft_enums/ft_encodings.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/freetype/ft_enums/tt_ms_ids.py` & `freetype-py-2.4.0/freetype/ft_enums/tt_ms_ids.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/screenshots.rst` & `freetype-py-2.4.0/doc/screenshots.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_mac_langids.rst` & `freetype-py-2.4.0/doc/tt_mac_langids.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_platforms.rst` & `freetype-py-2.4.0/doc/tt_platforms.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/make_enums.py` & `freetype-py-2.4.0/doc/make_enums.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_glyph_formats.rst` & `freetype-py-2.4.0/doc/ft_glyph_formats.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_load_flags.rst` & `freetype-py-2.4.0/doc/ft_load_flags.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/conf.py` & `freetype-py-2.4.0/doc/conf.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_encodings.rst` & `freetype-py-2.4.0/doc/ft_encodings.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/constants.rst` & `freetype-py-2.4.0/doc/constants.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/Makefile` & `freetype-py-2.4.0/doc/Makefile`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_fstypes.rst` & `freetype-py-2.4.0/doc/ft_fstypes.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_pixel_modes.rst` & `freetype-py-2.4.0/doc/ft_pixel_modes.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_outline_flags.rst` & `freetype-py-2.4.0/doc/ft_outline_flags.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/license.rst` & `freetype-py-2.4.0/doc/license.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_face_flags.rst` & `freetype-py-2.4.0/doc/ft_face_flags.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_stroker_borders.rst` & `freetype-py-2.4.0/doc/ft_stroker_borders.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_load_targets.rst` & `freetype-py-2.4.0/doc/ft_load_targets.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_ms_langids.rst` & `freetype-py-2.4.0/doc/tt_ms_langids.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/make.bat` & `freetype-py-2.4.0/doc/make.bat`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_ms_ids.rst` & `freetype-py-2.4.0/doc/tt_ms_ids.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_render_modes.rst` & `freetype-py-2.4.0/doc/ft_render_modes.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_stroker_linejoins.rst` & `freetype-py-2.4.0/doc/ft_stroker_linejoins.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_mac_ids.rst` & `freetype-py-2.4.0/doc/tt_mac_ids.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_apple_ids.rst` & `freetype-py-2.4.0/doc/tt_apple_ids.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/notes.rst` & `freetype-py-2.4.0/doc/notes.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/ft_lcd_filters.rst` & `freetype-py-2.4.0/doc/ft_lcd_filters.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/tt_name_ids.rst` & `freetype-py-2.4.0/doc/tt_name_ids.rst`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/wordle.png` & `freetype-py-2.4.0/doc/_static/wordle.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/opengl.png` & `freetype-py-2.4.0/doc/_static/opengl.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/S.png` & `freetype-py-2.4.0/doc/_static/S.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/hello-world.png` & `freetype-py-2.4.0/doc/_static/hello-world.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/agg-trick.png` & `freetype-py-2.4.0/doc/_static/agg-trick.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/outline.png` & `freetype-py-2.4.0/doc/_static/outline.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/doc/_static/G.png` & `freetype-py-2.4.0/doc/_static/G.png`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/tests/vf_test.py` & `freetype-py-2.4.0/tests/vf_test.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/tests/smoke_test.py` & `freetype-py-2.4.0/tests/smoke_test.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/hello-vf.py` & `freetype-py-2.4.0/examples/hello-vf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
 #
-#  FreeType high-level python API - Copyright 2011-2015 Nicolas P. Rougier
+#  Variable Font example - Copyright 2020 Josh Hadley, based on hello-world.py
 #  Distributed under the terms of the new BSD license.
 #
 # -----------------------------------------------------------------------------
 from freetype import *
 
 if __name__ == '__main__':
     import numpy
@@ -46,15 +46,15 @@
             bitmap = slot.bitmap
             top = slot.bitmap_top
             left = slot.bitmap_left
             w,h = bitmap.width, bitmap.rows
             y = (height - baseline - top) - (i * 48)
             kerning = face.get_kerning(previous, c)
             x += (kerning.x >> 6)
-            Z[y:y+h,x:x+w] += numpy.array(bitmap.buffer, dtype='ubyte').reshape(h,w)
+            Z[y:y+h,x+left:x+left+w] += numpy.array(bitmap.buffer, dtype='ubyte').reshape(h,w)
             x += (slot.advance.x >> 6)
             previous = c
 
     plt.figure(figsize=(10, 10*Z.shape[0]/float(Z.shape[1])))
     plt.imshow(Z, interpolation='nearest', origin='upper', cmap=plt.cm.gray)
     plt.xticks([]), plt.yticks([])
     plt.show()
```

## Comparing `freetype-py-2.3.0/examples/hello-world-cairo.py` & `freetype-py-2.4.0/examples/hello-world-cairo.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,14 @@
         w,h = bitmap.width, bitmap.rows
         y = height-baseline-top
         kerning = face.get_kerning(previous, c)
         x += (kerning.x >> 6)
         # cairo does not like zero-width bitmap from the space character!
         if (bitmap.width > 0):
             glyph_surface = make_image_surface(face.glyph.bitmap)
-            ctx.set_source_surface(glyph_surface, x, y)
+            ctx.set_source_surface(glyph_surface, x+left, y)
             ctx.paint()
         x += (slot.advance.x >> 6)
         previous = c
     Z.flush()
     Z.write_to_png("hello-world-cairo.png")
     Image.open("hello-world-cairo.png").show()
```

## Comparing `freetype-py-2.3.0/examples/SourceSansVariable-LICENSE.md` & `freetype-py-2.4.0/examples/SourceSansVariable-LICENSE.md`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/hello-world.py` & `freetype-py-2.4.0/examples/hello-world.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         bitmap = slot.bitmap
         top = slot.bitmap_top
         left = slot.bitmap_left
         w,h = bitmap.width, bitmap.rows
         y = height-baseline-top
         kerning = face.get_kerning(previous, c)
         x += (kerning.x >> 6)
-        Z[y:y+h,x:x+w] += numpy.array(bitmap.buffer, dtype='ubyte').reshape(h,w)
+        Z[y:y+h,x+left:x+left+w] += numpy.array(bitmap.buffer, dtype='ubyte').reshape(h,w)
         x += (slot.advance.x >> 6)
         previous = c
 
     plt.figure(figsize=(10, 10*Z.shape[0]/float(Z.shape[1])))
     plt.imshow(Z, interpolation='nearest', origin='upper', cmap=plt.cm.gray)
     plt.xticks([]), plt.yticks([])
     plt.show()
```

## Comparing `freetype-py-2.3.0/examples/font-info.py` & `freetype-py-2.4.0/examples/font-info.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-vector-2.py` & `freetype-py-2.4.0/examples/glyph-vector-2.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/bitmap_to_surface.py` & `freetype-py-2.4.0/examples/bitmap_to_surface.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/texture_font.py` & `freetype-py-2.4.0/examples/texture_font.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-color.py` & `freetype-py-2.4.0/examples/glyph-color.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/emoji-color.py` & `freetype-py-2.4.0/examples/emoji-color.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-color-cairo.py` & `freetype-py-2.4.0/examples/glyph-color-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/wordle-cairo.py` & `freetype-py-2.4.0/examples/wordle-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-metrics.py` & `freetype-py-2.4.0/examples/glyph-metrics.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/ascii.py` & `freetype-py-2.4.0/examples/ascii.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/subpixel-positioning.py` & `freetype-py-2.4.0/examples/subpixel-positioning.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/sfnt-names.py` & `freetype-py-2.4.0/examples/sfnt-names.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/Vera.ttf` & `freetype-py-2.4.0/examples/Vera.ttf`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-outline-cairo.py` & `freetype-py-2.4.0/examples/glyph-outline-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/opengl.py` & `freetype-py-2.4.0/examples/opengl.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/wordle.py` & `freetype-py-2.4.0/examples/wordle.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/outline-test.py` & `freetype-py-2.4.0/examples/outline-test.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-lcd-cairo.py` & `freetype-py-2.4.0/examples/glyph-lcd-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/example_1.py` & `freetype-py-2.4.0/examples/example_1.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/emoji-color-cairo.py` & `freetype-py-2.4.0/examples/emoji-color-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/agg-trick.py` & `freetype-py-2.4.0/examples/agg-trick.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-vector-2-cairo.py` & `freetype-py-2.4.0/examples/glyph-vector-2-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/example_1-cairo.py` & `freetype-py-2.4.0/examples/example_1-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-vector-cairo.py` & `freetype-py-2.4.0/examples/glyph-vector-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/ftdump.py` & `freetype-py-2.4.0/examples/ftdump.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-monochrome.py` & `freetype-py-2.4.0/examples/glyph-monochrome.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/shader.py` & `freetype-py-2.4.0/examples/shader.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-alpha.py` & `freetype-py-2.4.0/examples/glyph-alpha.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/SourceSansVariable-Roman.otf` & `freetype-py-2.4.0/examples/SourceSansVariable-Roman.otf`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/VeraMono.ttf` & `freetype-py-2.4.0/examples/VeraMono.ttf`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-vector.py` & `freetype-py-2.4.0/examples/glyph-vector.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-outline.py` & `freetype-py-2.4.0/examples/glyph-outline.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-vector-decompose.py` & `freetype-py-2.4.0/examples/glyph-vector-decompose.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-mono+alpha-cairo.py` & `freetype-py-2.4.0/examples/glyph-mono+alpha-cairo.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/examples/glyph-lcd.py` & `freetype-py-2.4.0/examples/glyph-lcd.py`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/.github/workflows/ci.yml` & `freetype-py-2.4.0/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -41,65 +41,80 @@
         - os: 'ubuntu-latest'
           cibw_build: "cp37-musllinux*"
           cibw_archs_linux: 'aarch64'
           cibw_archs_macos: "auto64"
           name: '(musllinux aarch64)'
           qemu: true
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0  # unshallow fetch for setuptools-scm
 
     - name: Set up QEMU
       if: matrix.qemu
-      uses: docker/setup-qemu-action@v1
+      uses: docker/setup-qemu-action@v2
       with:
         platforms: all
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.4.0
+      uses: pypa/cibuildwheel@v2.12.3
       env:
         CIBW_BUILD: ${{ matrix.cibw_build }}
         CIBW_ARCHS: "auto64"
         CIBW_ARCHS_MACOS: ${{ matrix.cibw_archs_macos }}
         CIBW_ARCHS_LINUX: ${{ matrix.cibw_archs_linux }}
         CIBW_ENVIRONMENT: "FREETYPEPY_BUNDLE_FT=yes PYTHON_ARCH=64"
         CIBW_MANYLINUX_X86_64_IMAGE: manylinux2010
         CIBW_MANYLINUX_AARCH64_IMAGE: manylinux2014
         CIBW_TEST_COMMAND: "pytest {project}/tests"
         CIBW_TEST_REQUIRES: "pytest"
       with:
         output-dir: dist
 
     - name: Upload distributions
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         path: dist
         name: dist
 
   publish:
     name: Publish release to Pypi
     runs-on: ubuntu-latest
     needs: [build]
     if: success() && github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0  # unshallow fetch for setuptools-scm
     - name: Set up Python 3.9
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.9'
     - name: Download assets
-      uses: actions/download-artifact@v1.0.0
+      uses: actions/download-artifact@v3
       with:
         name: dist
     - name: Build sdist
       run: |
         python setup.py sdist
     - name: Publish package to PyPI
       run: |
         pip install twine
         twine upload dist/*
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
+
+  test-pyinstaller:
+    name: Test pyinstaller hook
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python 3.9
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.9'
+    - name: Test pyinstaller hook
+      run: |
+        pip install pytest psutil pyinstaller>=4
+        FREETYPEPY_BUNDLE_FT=yes PYTHON_ARCH=64 pip install -e .
+        pytest -v freetype/__pyinstaller
```

## Comparing `freetype-py-2.3.0/debian/control` & `freetype-py-2.4.0/debian/control`

 * *Files identical despite different names*

## Comparing `freetype-py-2.3.0/debian/copyright` & `freetype-py-2.4.0/debian/copyright`

 * *Files identical despite different names*

