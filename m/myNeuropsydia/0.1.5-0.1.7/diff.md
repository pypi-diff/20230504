# Comparing `tmp/myNeuropsydia-0.1.5.tar.gz` & `tmp/myNeuropsydia-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myNeuropsydia-0.1.5.tar", last modified: Thu May  4 18:18:18 2023, max compression
+gzip compressed data, was "myNeuropsydia-0.1.7.tar", last modified: Thu May  4 18:30:18 2023, max compression
```

## Comparing `myNeuropsydia-0.1.5.tar` & `myNeuropsydia-0.1.7.tar`

### file list

```diff
@@ -1,447 +1,259 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.952025 myNeuropsydia-0.1.5/
--rw-rw-rw-   0        0        0      229 2023-05-04 18:18:18.950025 myNeuropsydia-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:17.844026 myNeuropsydia-0.1.5/myNeuropsydia/
--rw-rw-rw-   0        0        0      330 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.5/myNeuropsydia/__init__.py
--rw-rw-rw-   0        0        0     8399 2023-05-04 09:12:53.000000 myNeuropsydia-0.1.5/myNeuropsydia/ask.py
--rw-rw-rw-   0        0        0    27514 2023-05-04 16:37:28.000000 myNeuropsydia-0.1.5/myNeuropsydia/choice.py
--rw-rw-rw-   0        0        0    27810 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.5/myNeuropsydia/core.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:17.858021 myNeuropsydia-0.1.5/myNeuropsydia/files/
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:17.906021 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/__init__.py
--rw-rw-rw-   0        0        0    51416 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/absorption_desk.png
--rw-rw-rw-   0        0        0    59438 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/absorption_man.png
--rw-rw-rw-   0        0        0   288270 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_absorption.png
--rw-rw-rw-   0        0        0   302887 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_absorption_validated.png
--rw-rw-rw-   0        0        0    47525 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_blue.png
--rw-rw-rw-   0        0        0    49880 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_blue_validated.png
--rw-rw-rw-   0        0        0    43309 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_green.png
--rw-rw-rw-   0        0        0    50122 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_green_validated.png
--rw-rw-rw-   0        0        0    45849 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_orange.png
--rw-rw-rw-   0        0        0    48981 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_orange_validated.png
--rw-rw-rw-   0        0        0    47882 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_purple.png
--rw-rw-rw-   0        0        0    51182 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_purple_validated.png
--rw-rw-rw-   0        0        0    47248 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_red.png
--rw-rw-rw-   0        0        0    44401 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_red_validated.png
--rw-rw-rw-   0        0        0    34927 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_teal.png
--rw-rw-rw-   0        0        0    48362 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_teal_validated.png
--rw-rw-rw-   0        0        0    48420 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_yellow.png
--rw-rw-rw-   0        0        0    47363 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_yellow_validated.png
--rw-rw-rw-   0        0        0    18704 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/binary/scale_point.png
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:17.931023 myNeuropsydia-0.1.5/myNeuropsydia/files/font/
--rw-rw-rw-   0        0        0   105048 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/LiberationMono-Bold.ttf
--rw-rw-rw-   0        0        0   108168 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/LiberationMono-Regular.ttf
--rw-rw-rw-   0        0        0   164936 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoBlack.ttf
--rw-rw-rw-   0        0        0   163448 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoBold.ttf
--rw-rw-rw-   0        0        0   162636 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoLight.ttf
--rw-rw-rw-   0        0        0   158604 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoRegular.ttf
--rw-rw-rw-   0        0        0    35596 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/Timeless-Bold.ttf
--rw-rw-rw-   0        0        0    61212 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/Timeless.ttf
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:17.963032 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/
--rw-rw-rw-   0        0        0   169046 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/N.png
--rw-rw-rw-   0        0        0   843848 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png
--rw-rw-rw-   0        0        0   248442 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png
--rw-rw-rw-   0        0        0  4359723 2022-05-03 22:36:13.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png
--rw-rw-rw-   0        0        0    70561 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Python.png
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/__init__.py
--rw-rw-rw-   0        0        0     1611 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/icon.png
--rw-rw-rw-   0        0        0   827647 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/files/logo/neuropsydia_banner.png
--rw-rw-rw-   0        0        0     2792 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.5/myNeuropsydia/fill_form.py
--rw-rw-rw-   0        0        0    13763 2023-05-04 17:04:02.000000 myNeuropsydia-0.1.5/myNeuropsydia/image.py
--rw-rw-rw-   0        0        0     3663 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/io.py
--rw-rw-rw-   0        0        0    13684 2023-05-04 16:11:01.000000 myNeuropsydia-0.1.5/myNeuropsydia/meta.py
--rw-rw-rw-   0        0        0    14412 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.5/myNeuropsydia/miscellaneous.py
--rw-rw-rw-   0        0        0      413 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/path.py
--rw-rw-rw-   0        0        0     2801 2023-05-04 09:09:54.000000 myNeuropsydia-0.1.5/myNeuropsydia/procedures.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.022036 myNeuropsydia-0.1.5/myNeuropsydia/pygame/
--rw-rw-rw-   0        0        0    10287 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.029021 myNeuropsydia-0.1.5/myNeuropsydia/pygame/__pyinstaller/
--rw-rw-rw-   0        0        0       72 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0     1367 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/__pyinstaller/hook-pygame.py
--rw-rw-rw-   0        0        0     4386 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/_camera_opencv.py
--rw-rw-rw-   0        0        0     3402 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/_camera_vidcapture.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.034023 myNeuropsydia-0.1.5/myNeuropsydia/pygame/_sdl2/
--rw-rw-rw-   0        0        0      248 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/_sdl2/__init__.py
--rw-rw-rw-   0        0        0     4496 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/camera.py
--rw-rw-rw-   0        0        0    25773 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/colordict.py
--rw-rw-rw-   0        0        0    18203 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/cursors.py
--rw-rw-rw-   0        0        0    18687 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/draw_py.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.247035 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/
--rw-rw-rw-   0        0        0        0 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/__init__.py
--rw-rw-rw-   0        0        0     1034 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/aacircle.py
--rw-rw-rw-   0        0        0    12055 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/aliens.py
--rw-rw-rw-   0        0        0     3633 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/arraydemo.py
--rw-rw-rw-   0        0        0     1563 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/audiocapture.py
--rw-rw-rw-   0        0        0     3425 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/blend_fill.py
--rw-rw-rw-   0        0        0     6345 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/blit_blends.py
--rw-rw-rw-   0        0        0     3028 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/camera.py
--rw-rw-rw-   0        0        0     5910 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/chimp.py
--rw-rw-rw-   0        0        0     2873 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/cursors.py
--rw-rw-rw-   0        0        0     2240 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/dropevent.py
--rw-rw-rw-   0        0        0     5938 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/eventlist.py
--rw-rw-rw-   0        0        0     9841 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/font_viewer.py
--rw-rw-rw-   0        0        0     2080 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/fonty.py
--rw-rw-rw-   0        0        0     3656 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/freetype_misc.py
--rw-rw-rw-   0        0        0    16860 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/glcube.py
--rw-rw-rw-   0        0        0     1301 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/headless_no_windows_needed.py
--rw-rw-rw-   0        0        0     5333 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/joystick.py
--rw-rw-rw-   0        0        0     2541 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/liquid.py
--rw-rw-rw-   0        0        0     5811 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/mask.py
--rw-rw-rw-   0        0        0    29414 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/midi.py
--rw-rw-rw-   0        0        0     1824 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/moveit.py
--rw-rw-rw-   0        0        0     8999 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/music_drop_fade.py
--rw-rw-rw-   0        0        0     3450 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/pixelarray.py
--rw-rw-rw-   0        0        0     5223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/playmus.py
--rw-rw-rw-   0        0        0     2492 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/prevent_display_stretching.py
--rw-rw-rw-   0        0        0     1046 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/resizing_new.py
--rw-rw-rw-   0        0        0     4866 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/scaletest.py
--rw-rw-rw-   0        0        0     3056 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/scrap_clipboard.py
--rw-rw-rw-   0        0        0     6578 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/scroll.py
--rw-rw-rw-   0        0        0     1801 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/setmodescale.py
--rw-rw-rw-   0        0        0     1172 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/sound.py
--rw-rw-rw-   0        0        0     5797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/sound_array_demos.py
--rw-rw-rw-   0        0        0     2516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/sprite_texture.py
--rw-rw-rw-   0        0        0     2762 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/stars.py
--rw-rw-rw-   0        0        0     7001 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/testsprite.py
--rw-rw-rw-   0        0        0     5394 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/textinput.py
--rw-rw-rw-   0        0        0     3277 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/vgrade.py
--rw-rw-rw-   0        0        0     4452 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/video.py
--rw-rw-rw-   0        0        0     1694 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/fastevent.py
--rw-rw-rw-   0        0        0     2216 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/freetype.py
--rw-rw-rw-   0        0        0     6145 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/ftfont.py
--rw-rw-rw-   0        0        0    11638 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/locals.py
--rw-rw-rw-   0        0        0      399 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/macosx.py
--rw-rw-rw-   0        0        0    24398 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/midi.py
--rw-rw-rw-   0        0        0     2445 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/pkgdata.py
--rw-rw-rw-   0        0        0     4083 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/sndarray.py
--rw-rw-rw-   0        0        0    61450 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/sprite.py
--rw-rw-rw-   0        0        0    14424 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/surfarray.py
--rw-rw-rw-   0        0        0    16053 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/sysfont.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.402040 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/
--rw-rw-rw-   0        0        0     1251 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/__main__.py
--rw-rw-rw-   0        0        0    22634 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/base_test.py
--rw-rw-rw-   0        0        0     4740 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/blit_test.py
--rw-rw-rw-   0        0        0    16511 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/bufferproxy_test.py
--rw-rw-rw-   0        0        0       70 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/camera_test.py
--rw-rw-rw-   0        0        0    47441 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/color_test.py
--rw-rw-rw-   0        0        0     9516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/constants_test.py
--rw-rw-rw-   0        0        0    10834 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/controller_test.py
--rw-rw-rw-   0        0        0     7700 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/cursors_test.py
--rw-rw-rw-   0        0        0    29009 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/display_test.py
--rw-rw-rw-   0        0        0     1091 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/docs_test.py
--rw-rw-rw-   0        0        0   237007 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/draw_test.py
--rw-rw-rw-   0        0        0    28625 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/event_test.py
--rw-rw-rw-   0        0        0    22605 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/font_test.py
--rw-rw-rw-   0        0        0      182 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/freetype_tags.py
--rw-rw-rw-   0        0        0    64428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/freetype_test.py
--rw-rw-rw-   0        0        0      180 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/ftfont_tags.py
--rw-rw-rw-   0        0        0      523 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/ftfont_test.py
--rw-rw-rw-   0        0        0    32375 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/gfxdraw_test.py
--rw-rw-rw-   0        0        0     1198 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/image__save_gl_surface_test.py
--rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/image_tags.py
--rw-rw-rw-   0        0        0    37989 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/image_test.py
--rw-rw-rw-   0        0        0      135 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/imageext_tags.py
--rw-rw-rw-   0        0        0     2889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/imageext_test.py
--rw-rw-rw-   0        0        0     6168 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/joystick_test.py
--rw-rw-rw-   0        0        0     4171 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/key_test.py
--rw-rw-rw-   0        0        0   246451 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mask_test.py
--rw-rw-rw-   0        0        0    87928 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/math_test.py
--rw-rw-rw-   0        0        0    16914 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/midi_test.py
--rw-rw-rw-   0        0        0      138 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mixer_music_tags.py
--rw-rw-rw-   0        0        0    13312 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mixer_music_test.py
--rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mixer_tags.py
--rw-rw-rw-   0        0        0    43923 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mixer_test.py
--rw-rw-rw-   0        0        0    13149 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mouse_test.py
--rw-rw-rw-   0        0        0    62428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/pixelarray_test.py
--rw-rw-rw-   0        0        0    25561 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/pixelcopy_test.py
--rw-rw-rw-   0        0        0    75529 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/rect_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.406022 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.425024 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_3_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_4_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_5_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_6_test.py
--rw-rw-rw-   0        0        0      797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/no_assertions__ret_code_of_1__test.py
--rw-rw-rw-   0        0        0      545 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/zero_tests_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.436018 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/fake_2_test.py
--rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/incomplete_todo_test.py
--rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/magic_tag_test.py
--rw-rw-rw-   0        0        0      715 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/sleep_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.444031 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/fake_2_test.py
--rw-rw-rw-   0        0        0      925 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/invisible_tag_test.py
--rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/magic_tag_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.452030 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_4_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.458031 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/__init__.py
--rw-rw-rw-   0        0        0      889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_3_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.464044 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/__init__.py
--rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_3_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.470042 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/__init__.py
--rw-rw-rw-   0        0        0      906 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_1_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_2_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.478027 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_2_test.py
--rw-rw-rw-   0        0        0      954 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_4_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.486033 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_2_test.py
--rw-rw-rw-   0        0        0     1012 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_4_test.py
--rw-rw-rw-   0        0        0     4342 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/run_tests__test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.491041 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/timeout/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/timeout/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/timeout/fake_2_test.py
--rw-rw-rw-   0        0        0      716 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/timeout/sleep_test.py
--rw-rw-rw-   0        0        0     4323 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/rwobject_test.py
--rw-rw-rw-   0        0        0      671 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/scrap_tags.py
--rw-rw-rw-   0        0        0     9160 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/scrap_test.py
--rw-rw-rw-   0        0        0      190 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sndarray_tags.py
--rw-rw-rw-   0        0        0     6297 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sndarray_test.py
--rw-rw-rw-   0        0        0    46638 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sprite_test.py
--rw-rw-rw-   0        0        0   163734 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surface_test.py
--rw-rw-rw-   0        0        0      260 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surfarray_tags.py
--rw-rw-rw-   0        0        0    25768 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surfarray_test.py
--rw-rw-rw-   0        0        0     4728 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surflock_test.py
--rw-rw-rw-   0        0        0     1463 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sysfont_test.py
--rw-rw-rw-   0        0        0       21 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_test_.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.509034 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/
--rw-rw-rw-   0        0        0     5371 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0    14843 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/arrinter.py
--rw-rw-rw-   0        0        0     9128 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/async_sub.py
--rw-rw-rw-   0        0        0    23706 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/buftools.py
--rw-rw-rw-   0        0        0      495 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/endian.py
--rw-rw-rw-   0        0        0   152382 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/png.py
--rw-rw-rw-   0        0        0    12049 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/run_tests.py
--rw-rw-rw-   0        0        0     2483 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/test_machinery.py
--rw-rw-rw-   0        0        0     9434 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/test_runner.py
--rw-rw-rw-   0        0        0     7842 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/threads_test.py
--rw-rw-rw-   0        0        0    15336 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/time_test.py
--rw-rw-rw-   0        0        0     3223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/touch_test.py
--rw-rw-rw-   0        0        0    49044 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/transform_test.py
--rw-rw-rw-   0        0        0     1536 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/version_test.py
--rw-rw-rw-   0        0        0      696 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/video_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.511040 myNeuropsydia-0.1.5/myNeuropsydia/pygame/threads/
--rw-rw-rw-   0        0        0     8074 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/threads/__init__.py
--rw-rw-rw-   0        0        0     2526 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/myNeuropsydia/pygame/version.py
--rw-rw-rw-   0        0        0    16381 2023-05-04 09:09:54.000000 myNeuropsydia-0.1.5/myNeuropsydia/scale.py
--rw-rw-rw-   0        0        0     8770 2023-05-04 10:29:19.000000 myNeuropsydia-0.1.5/myNeuropsydia/start.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.515030 myNeuropsydia-0.1.5/myNeuropsydia/tests/
--rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/tests/__init__.py
--rw-rw-rw-   0        0        0      218 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.5/myNeuropsydia/tests/test_color.py
--rw-rw-rw-   0        0        0     8526 2023-05-04 10:24:43.000000 myNeuropsydia-0.1.5/myNeuropsydia/write.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:17.856029 myNeuropsydia-0.1.5/myNeuropsydia.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-04 18:18:17.000000 myNeuropsydia-0.1.5/myNeuropsydia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16616 2023-05-04 18:18:17.000000 myNeuropsydia-0.1.5/myNeuropsydia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       62 2023-05-04 18:18:17.000000 myNeuropsydia-0.1.5/myNeuropsydia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-04 18:18:17.000000 myNeuropsydia-0.1.5/myNeuropsydia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-04 18:18:17.000000 myNeuropsydia-0.1.5/myNeuropsydia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.557018 myNeuropsydia-0.1.5/pygame/
--rw-rw-rw-   0        0        0    10287 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.561024 myNeuropsydia-0.1.5/pygame/__pyinstaller/
--rw-rw-rw-   0        0        0       72 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0     1367 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/__pyinstaller/hook-pygame.py
--rw-rw-rw-   0        0        0     4386 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/_camera_opencv.py
--rw-rw-rw-   0        0        0     3402 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/_camera_vidcapture.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.563029 myNeuropsydia-0.1.5/pygame/_sdl2/
--rw-rw-rw-   0        0        0      248 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/_sdl2/__init__.py
--rw-rw-rw-   0        0        0     4496 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/camera.py
--rw-rw-rw-   0        0        0    25773 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/colordict.py
--rw-rw-rw-   0        0        0    18203 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/cursors.py
--rw-rw-rw-   0        0        0    18687 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/draw_py.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.682031 myNeuropsydia-0.1.5/pygame/examples/
--rw-rw-rw-   0        0        0        0 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/__init__.py
--rw-rw-rw-   0        0        0     1034 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/aacircle.py
--rw-rw-rw-   0        0        0    12055 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/aliens.py
--rw-rw-rw-   0        0        0     3633 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/arraydemo.py
--rw-rw-rw-   0        0        0     1563 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/audiocapture.py
--rw-rw-rw-   0        0        0     3425 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/blend_fill.py
--rw-rw-rw-   0        0        0     6345 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/blit_blends.py
--rw-rw-rw-   0        0        0     3028 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/camera.py
--rw-rw-rw-   0        0        0     5910 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/chimp.py
--rw-rw-rw-   0        0        0     2873 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/cursors.py
--rw-rw-rw-   0        0        0     2240 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/dropevent.py
--rw-rw-rw-   0        0        0     5938 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/eventlist.py
--rw-rw-rw-   0        0        0     9841 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/font_viewer.py
--rw-rw-rw-   0        0        0     2080 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/fonty.py
--rw-rw-rw-   0        0        0     3656 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/freetype_misc.py
--rw-rw-rw-   0        0        0    16860 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/glcube.py
--rw-rw-rw-   0        0        0     1301 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/headless_no_windows_needed.py
--rw-rw-rw-   0        0        0     5333 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/joystick.py
--rw-rw-rw-   0        0        0     2541 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/liquid.py
--rw-rw-rw-   0        0        0     5811 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/mask.py
--rw-rw-rw-   0        0        0    29414 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/midi.py
--rw-rw-rw-   0        0        0     1824 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/moveit.py
--rw-rw-rw-   0        0        0     8999 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/music_drop_fade.py
--rw-rw-rw-   0        0        0     3450 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/pixelarray.py
--rw-rw-rw-   0        0        0     5223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/playmus.py
--rw-rw-rw-   0        0        0     2492 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/prevent_display_stretching.py
--rw-rw-rw-   0        0        0     1046 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/resizing_new.py
--rw-rw-rw-   0        0        0     4866 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/scaletest.py
--rw-rw-rw-   0        0        0     3056 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/scrap_clipboard.py
--rw-rw-rw-   0        0        0     6578 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/scroll.py
--rw-rw-rw-   0        0        0     1801 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/setmodescale.py
--rw-rw-rw-   0        0        0     1172 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/sound.py
--rw-rw-rw-   0        0        0     5797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/sound_array_demos.py
--rw-rw-rw-   0        0        0     2516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/sprite_texture.py
--rw-rw-rw-   0        0        0     2762 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/stars.py
--rw-rw-rw-   0        0        0     7001 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/testsprite.py
--rw-rw-rw-   0        0        0     5394 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/textinput.py
--rw-rw-rw-   0        0        0     3277 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/vgrade.py
--rw-rw-rw-   0        0        0     4452 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/examples/video.py
--rw-rw-rw-   0        0        0     1694 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/fastevent.py
--rw-rw-rw-   0        0        0     2216 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/freetype.py
--rw-rw-rw-   0        0        0     6145 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/ftfont.py
--rw-rw-rw-   0        0        0    11638 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/locals.py
--rw-rw-rw-   0        0        0      399 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/macosx.py
--rw-rw-rw-   0        0        0    24398 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/midi.py
--rw-rw-rw-   0        0        0     2445 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/pkgdata.py
--rw-rw-rw-   0        0        0     4083 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/sndarray.py
--rw-rw-rw-   0        0        0    61450 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/sprite.py
--rw-rw-rw-   0        0        0    14424 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/surfarray.py
--rw-rw-rw-   0        0        0    16053 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/sysfont.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.819024 myNeuropsydia-0.1.5/pygame/tests/
--rw-rw-rw-   0        0        0     1251 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/__main__.py
--rw-rw-rw-   0        0        0    22634 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/base_test.py
--rw-rw-rw-   0        0        0     4740 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/blit_test.py
--rw-rw-rw-   0        0        0    16511 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/bufferproxy_test.py
--rw-rw-rw-   0        0        0       70 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/camera_test.py
--rw-rw-rw-   0        0        0    47441 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/color_test.py
--rw-rw-rw-   0        0        0     9516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/constants_test.py
--rw-rw-rw-   0        0        0    10834 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/controller_test.py
--rw-rw-rw-   0        0        0     7700 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/cursors_test.py
--rw-rw-rw-   0        0        0    29009 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/display_test.py
--rw-rw-rw-   0        0        0     1091 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/docs_test.py
--rw-rw-rw-   0        0        0   237007 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/draw_test.py
--rw-rw-rw-   0        0        0    28625 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/event_test.py
--rw-rw-rw-   0        0        0    22605 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/font_test.py
--rw-rw-rw-   0        0        0      182 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/freetype_tags.py
--rw-rw-rw-   0        0        0    64428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/freetype_test.py
--rw-rw-rw-   0        0        0      180 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/ftfont_tags.py
--rw-rw-rw-   0        0        0      523 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/ftfont_test.py
--rw-rw-rw-   0        0        0    32375 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/gfxdraw_test.py
--rw-rw-rw-   0        0        0     1198 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/image__save_gl_surface_test.py
--rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/image_tags.py
--rw-rw-rw-   0        0        0    37989 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/image_test.py
--rw-rw-rw-   0        0        0      135 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/imageext_tags.py
--rw-rw-rw-   0        0        0     2889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/imageext_test.py
--rw-rw-rw-   0        0        0     6168 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/joystick_test.py
--rw-rw-rw-   0        0        0     4171 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/key_test.py
--rw-rw-rw-   0        0        0   246451 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/mask_test.py
--rw-rw-rw-   0        0        0    87928 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/math_test.py
--rw-rw-rw-   0        0        0    16914 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/midi_test.py
--rw-rw-rw-   0        0        0      138 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/mixer_music_tags.py
--rw-rw-rw-   0        0        0    13312 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/mixer_music_test.py
--rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/mixer_tags.py
--rw-rw-rw-   0        0        0    43923 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/mixer_test.py
--rw-rw-rw-   0        0        0    13149 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/mouse_test.py
--rw-rw-rw-   0        0        0    62428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/pixelarray_test.py
--rw-rw-rw-   0        0        0    25561 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/pixelcopy_test.py
--rw-rw-rw-   0        0        0    75529 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/rect_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.822032 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.843020 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/fake_3_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/fake_4_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/fake_5_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/fake_6_test.py
--rw-rw-rw-   0        0        0      797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/no_assertions__ret_code_of_1__test.py
--rw-rw-rw-   0        0        0      545 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/all_ok/zero_tests_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.853032 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/everything/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/everything/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/everything/fake_2_test.py
--rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/everything/incomplete_todo_test.py
--rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/everything/magic_tag_test.py
--rw-rw-rw-   0        0        0      715 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/everything/sleep_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.863018 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/exclude/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/exclude/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/exclude/fake_2_test.py
--rw-rw-rw-   0        0        0      925 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/exclude/invisible_tag_test.py
--rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/exclude/magic_tag_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.873021 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/failures1/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/failures1/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/failures1/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/failures1/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/failures1/fake_4_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.880029 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete/__init__.py
--rw-rw-rw-   0        0        0      889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete/fake_3_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.887025 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete_todo/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete_todo/__init__.py
--rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete_todo/fake_2_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/incomplete_todo/fake_3_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.895024 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/infinite_loop/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/infinite_loop/__init__.py
--rw-rw-rw-   0        0        0      906 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/infinite_loop/fake_1_test.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/infinite_loop/fake_2_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.906024 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stderr/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stderr/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stderr/fake_2_test.py
--rw-rw-rw-   0        0        0      954 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stderr/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stderr/fake_4_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.916023 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stdout/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stdout/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stdout/fake_2_test.py
--rw-rw-rw-   0        0        0     1012 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stdout/fake_3_test.py
--rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/print_stdout/fake_4_test.py
--rw-rw-rw-   0        0        0     4342 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/run_tests__test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.923033 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/timeout/
--rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/timeout/__init__.py
--rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/timeout/fake_2_test.py
--rw-rw-rw-   0        0        0      716 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/run_tests__tests/timeout/sleep_test.py
--rw-rw-rw-   0        0        0     4323 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/rwobject_test.py
--rw-rw-rw-   0        0        0      671 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/scrap_tags.py
--rw-rw-rw-   0        0        0     9160 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/scrap_test.py
--rw-rw-rw-   0        0        0      190 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/sndarray_tags.py
--rw-rw-rw-   0        0        0     6297 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/sndarray_test.py
--rw-rw-rw-   0        0        0    46638 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/sprite_test.py
--rw-rw-rw-   0        0        0   163734 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/surface_test.py
--rw-rw-rw-   0        0        0      260 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/surfarray_tags.py
--rw-rw-rw-   0        0        0    25768 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/surfarray_test.py
--rw-rw-rw-   0        0        0     4728 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/surflock_test.py
--rw-rw-rw-   0        0        0     1463 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/sysfont_test.py
--rw-rw-rw-   0        0        0       21 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_test_.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.945024 myNeuropsydia-0.1.5/pygame/tests/test_utils/
--rw-rw-rw-   0        0        0     5371 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0    14843 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/arrinter.py
--rw-rw-rw-   0        0        0     9128 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/async_sub.py
--rw-rw-rw-   0        0        0    23706 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/buftools.py
--rw-rw-rw-   0        0        0      495 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/endian.py
--rw-rw-rw-   0        0        0   152382 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/png.py
--rw-rw-rw-   0        0        0    12049 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/run_tests.py
--rw-rw-rw-   0        0        0     2483 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/test_machinery.py
--rw-rw-rw-   0        0        0     9434 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/test_utils/test_runner.py
--rw-rw-rw-   0        0        0     7842 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/threads_test.py
--rw-rw-rw-   0        0        0    15336 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/time_test.py
--rw-rw-rw-   0        0        0     3223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/touch_test.py
--rw-rw-rw-   0        0        0    49044 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/transform_test.py
--rw-rw-rw-   0        0        0     1536 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/version_test.py
--rw-rw-rw-   0        0        0      696 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/tests/video_test.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:18:18.948022 myNeuropsydia-0.1.5/pygame/threads/
--rw-rw-rw-   0        0        0     8074 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.5/pygame/threads/__init__.py
--rw-rw-rw-   0        0        0     2526 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.5/pygame/version.py
--rw-rw-rw-   0        0        0       42 2023-05-04 18:18:18.952025 myNeuropsydia-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-04 18:18:08.000000 myNeuropsydia-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.695376 myNeuropsydia-0.1.7/
+-rw-rw-rw-   0        0        0      229 2023-05-04 18:30:18.694377 myNeuropsydia-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.103376 myNeuropsydia-0.1.7/myNeuropsydia/
+-rw-rw-rw-   0        0        0      330 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/__init__.py
+-rw-rw-rw-   0        0        0     8399 2023-05-04 09:12:53.000000 myNeuropsydia-0.1.7/myNeuropsydia/ask.py
+-rw-rw-rw-   0        0        0    27514 2023-05-04 16:37:28.000000 myNeuropsydia-0.1.7/myNeuropsydia/choice.py
+-rw-rw-rw-   0        0        0    27810 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/core.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.115378 myNeuropsydia-0.1.7/myNeuropsydia/files/
+-rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.157396 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/
+-rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/__init__.py
+-rw-rw-rw-   0        0        0    51416 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_desk.png
+-rw-rw-rw-   0        0        0    59438 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_man.png
+-rw-rw-rw-   0        0        0   288270 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption.png
+-rw-rw-rw-   0        0        0   302887 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption_validated.png
+-rw-rw-rw-   0        0        0    47525 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue.png
+-rw-rw-rw-   0        0        0    49880 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue_validated.png
+-rw-rw-rw-   0        0        0    43309 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green.png
+-rw-rw-rw-   0        0        0    50122 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green_validated.png
+-rw-rw-rw-   0        0        0    45849 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange.png
+-rw-rw-rw-   0        0        0    48981 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange_validated.png
+-rw-rw-rw-   0        0        0    47882 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple.png
+-rw-rw-rw-   0        0        0    51182 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple_validated.png
+-rw-rw-rw-   0        0        0    47248 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red.png
+-rw-rw-rw-   0        0        0    44401 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red_validated.png
+-rw-rw-rw-   0        0        0    34927 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal.png
+-rw-rw-rw-   0        0        0    48362 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal_validated.png
+-rw-rw-rw-   0        0        0    48420 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow.png
+-rw-rw-rw-   0        0        0    47363 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow_validated.png
+-rw-rw-rw-   0        0        0    18704 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/binary/scale_point.png
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.175375 myNeuropsydia-0.1.7/myNeuropsydia/files/font/
+-rw-rw-rw-   0        0        0   105048 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Bold.ttf
+-rw-rw-rw-   0        0        0   108168 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Regular.ttf
+-rw-rw-rw-   0        0        0   164936 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBlack.ttf
+-rw-rw-rw-   0        0        0   163448 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBold.ttf
+-rw-rw-rw-   0        0        0   162636 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoLight.ttf
+-rw-rw-rw-   0        0        0   158604 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoRegular.ttf
+-rw-rw-rw-   0        0        0    35596 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless-Bold.ttf
+-rw-rw-rw-   0        0        0    61212 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless.ttf
+-rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.198379 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/
+-rw-rw-rw-   0        0        0   169046 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/N.png
+-rw-rw-rw-   0        0        0   843848 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png
+-rw-rw-rw-   0        0        0   248442 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png
+-rw-rw-rw-   0        0        0  4359723 2022-05-03 22:36:13.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png
+-rw-rw-rw-   0        0        0    70561 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Python.png
+-rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/__init__.py
+-rw-rw-rw-   0        0        0     1611 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/icon.png
+-rw-rw-rw-   0        0        0   827647 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/files/logo/neuropsydia_banner.png
+-rw-rw-rw-   0        0        0     2792 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/fill_form.py
+-rw-rw-rw-   0        0        0    13763 2023-05-04 17:04:02.000000 myNeuropsydia-0.1.7/myNeuropsydia/image.py
+-rw-rw-rw-   0        0        0     3663 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/io.py
+-rw-rw-rw-   0        0        0    13500 2023-05-04 18:25:45.000000 myNeuropsydia-0.1.7/myNeuropsydia/meta.py
+-rw-rw-rw-   0        0        0    14412 2023-05-04 17:22:15.000000 myNeuropsydia-0.1.7/myNeuropsydia/miscellaneous.py
+-rw-rw-rw-   0        0        0      413 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/path.py
+-rw-rw-rw-   0        0        0     2801 2023-05-04 09:09:54.000000 myNeuropsydia-0.1.7/myNeuropsydia/procedures.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.238386 myNeuropsydia-0.1.7/myNeuropsydia/pygame/
+-rw-rw-rw-   0        0        0    10287 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.242387 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/
+-rw-rw-rw-   0        0        0       72 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0     1367 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/hook-pygame.py
+-rw-rw-rw-   0        0        0     4386 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_camera_opencv.py
+-rw-rw-rw-   0        0        0     3402 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_camera_vidcapture.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.244389 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_sdl2/
+-rw-rw-rw-   0        0        0      248 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/_sdl2/__init__.py
+-rw-rw-rw-   0        0        0     4496 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/camera.py
+-rw-rw-rw-   0        0        0    25773 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/colordict.py
+-rw-rw-rw-   0        0        0    18203 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/cursors.py
+-rw-rw-rw-   0        0        0    18687 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/draw_py.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.320377 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/
+-rw-rw-rw-   0        0        0        0 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/__init__.py
+-rw-rw-rw-   0        0        0     1034 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/aacircle.py
+-rw-rw-rw-   0        0        0    12055 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/aliens.py
+-rw-rw-rw-   0        0        0     3633 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/arraydemo.py
+-rw-rw-rw-   0        0        0     1563 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/audiocapture.py
+-rw-rw-rw-   0        0        0     3425 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/blend_fill.py
+-rw-rw-rw-   0        0        0     6345 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/blit_blends.py
+-rw-rw-rw-   0        0        0     3028 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/camera.py
+-rw-rw-rw-   0        0        0     5910 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/chimp.py
+-rw-rw-rw-   0        0        0     2873 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/cursors.py
+-rw-rw-rw-   0        0        0     2240 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/dropevent.py
+-rw-rw-rw-   0        0        0     5938 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/eventlist.py
+-rw-rw-rw-   0        0        0     9841 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/font_viewer.py
+-rw-rw-rw-   0        0        0     2080 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/fonty.py
+-rw-rw-rw-   0        0        0     3656 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/freetype_misc.py
+-rw-rw-rw-   0        0        0    16860 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/glcube.py
+-rw-rw-rw-   0        0        0     1301 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/headless_no_windows_needed.py
+-rw-rw-rw-   0        0        0     5333 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/joystick.py
+-rw-rw-rw-   0        0        0     2541 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/liquid.py
+-rw-rw-rw-   0        0        0     5811 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/mask.py
+-rw-rw-rw-   0        0        0    29414 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/midi.py
+-rw-rw-rw-   0        0        0     1824 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/moveit.py
+-rw-rw-rw-   0        0        0     8999 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/music_drop_fade.py
+-rw-rw-rw-   0        0        0     3450 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/pixelarray.py
+-rw-rw-rw-   0        0        0     5223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/playmus.py
+-rw-rw-rw-   0        0        0     2492 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/prevent_display_stretching.py
+-rw-rw-rw-   0        0        0     1046 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/resizing_new.py
+-rw-rw-rw-   0        0        0     4866 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scaletest.py
+-rw-rw-rw-   0        0        0     3056 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scrap_clipboard.py
+-rw-rw-rw-   0        0        0     6578 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scroll.py
+-rw-rw-rw-   0        0        0     1801 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/setmodescale.py
+-rw-rw-rw-   0        0        0     1172 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sound.py
+-rw-rw-rw-   0        0        0     5797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sound_array_demos.py
+-rw-rw-rw-   0        0        0     2516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sprite_texture.py
+-rw-rw-rw-   0        0        0     2762 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/stars.py
+-rw-rw-rw-   0        0        0     7001 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/testsprite.py
+-rw-rw-rw-   0        0        0     5394 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/textinput.py
+-rw-rw-rw-   0        0        0     3277 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/vgrade.py
+-rw-rw-rw-   0        0        0     4452 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/video.py
+-rw-rw-rw-   0        0        0     1694 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/fastevent.py
+-rw-rw-rw-   0        0        0     2216 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/freetype.py
+-rw-rw-rw-   0        0        0     6145 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/ftfont.py
+-rw-rw-rw-   0        0        0    11638 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/locals.py
+-rw-rw-rw-   0        0        0      399 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/macosx.py
+-rw-rw-rw-   0        0        0    24398 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/midi.py
+-rw-rw-rw-   0        0        0     2445 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/pkgdata.py
+-rw-rw-rw-   0        0        0     4083 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/sndarray.py
+-rw-rw-rw-   0        0        0    61450 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/sprite.py
+-rw-rw-rw-   0        0        0    14424 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/surfarray.py
+-rw-rw-rw-   0        0        0    16053 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/sysfont.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.535387 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/
+-rw-rw-rw-   0        0        0     1251 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/__init__.py
+-rw-rw-rw-   0        0        0     3826 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/__main__.py
+-rw-rw-rw-   0        0        0    22634 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/base_test.py
+-rw-rw-rw-   0        0        0     4740 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/blit_test.py
+-rw-rw-rw-   0        0        0    16511 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/bufferproxy_test.py
+-rw-rw-rw-   0        0        0       70 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/camera_test.py
+-rw-rw-rw-   0        0        0    47441 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/color_test.py
+-rw-rw-rw-   0        0        0     9516 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/constants_test.py
+-rw-rw-rw-   0        0        0    10834 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/controller_test.py
+-rw-rw-rw-   0        0        0     7700 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/cursors_test.py
+-rw-rw-rw-   0        0        0    29009 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/display_test.py
+-rw-rw-rw-   0        0        0     1091 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/docs_test.py
+-rw-rw-rw-   0        0        0   237007 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/draw_test.py
+-rw-rw-rw-   0        0        0    28625 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/event_test.py
+-rw-rw-rw-   0        0        0    22605 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/font_test.py
+-rw-rw-rw-   0        0        0      182 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/freetype_tags.py
+-rw-rw-rw-   0        0        0    64428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/freetype_test.py
+-rw-rw-rw-   0        0        0      180 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/ftfont_tags.py
+-rw-rw-rw-   0        0        0      523 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/ftfont_test.py
+-rw-rw-rw-   0        0        0    32375 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/gfxdraw_test.py
+-rw-rw-rw-   0        0        0     1198 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image__save_gl_surface_test.py
+-rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image_tags.py
+-rw-rw-rw-   0        0        0    37989 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image_test.py
+-rw-rw-rw-   0        0        0      135 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/imageext_tags.py
+-rw-rw-rw-   0        0        0     2889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/imageext_test.py
+-rw-rw-rw-   0        0        0     6168 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/joystick_test.py
+-rw-rw-rw-   0        0        0     4171 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/key_test.py
+-rw-rw-rw-   0        0        0   246451 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mask_test.py
+-rw-rw-rw-   0        0        0    87928 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/math_test.py
+-rw-rw-rw-   0        0        0    16914 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/midi_test.py
+-rw-rw-rw-   0        0        0      138 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_music_tags.py
+-rw-rw-rw-   0        0        0    13312 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_music_test.py
+-rw-rw-rw-   0        0        0      132 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_tags.py
+-rw-rw-rw-   0        0        0    43923 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_test.py
+-rw-rw-rw-   0        0        0    13149 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mouse_test.py
+-rw-rw-rw-   0        0        0    62428 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/pixelarray_test.py
+-rw-rw-rw-   0        0        0    25561 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/pixelcopy_test.py
+-rw-rw-rw-   0        0        0    75529 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/rect_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.546378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.590379 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_2_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_3_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_4_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_5_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_6_test.py
+-rw-rw-rw-   0        0        0      797 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/no_assertions__ret_code_of_1__test.py
+-rw-rw-rw-   0        0        0      545 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/zero_tests_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.605378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/fake_2_test.py
+-rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/incomplete_todo_test.py
+-rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/magic_tag_test.py
+-rw-rw-rw-   0        0        0      715 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/sleep_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.613378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/fake_2_test.py
+-rw-rw-rw-   0        0        0      925 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/invisible_tag_test.py
+-rw-rw-rw-   0        0        0      859 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/magic_tag_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.622377 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_2_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_3_test.py
+-rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_4_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.628375 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/__init__.py
+-rw-rw-rw-   0        0        0      889 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_2_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_3_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.633376 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/__init__.py
+-rw-rw-rw-   0        0        0      909 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_2_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_3_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.641374 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/__init__.py
+-rw-rw-rw-   0        0        0      906 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_1_test.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_2_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.648374 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_2_test.py
+-rw-rw-rw-   0        0        0      954 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_3_test.py
+-rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_4_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.657376 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_2_test.py
+-rw-rw-rw-   0        0        0     1012 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_3_test.py
+-rw-rw-rw-   0        0        0      949 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_4_test.py
+-rw-rw-rw-   0        0        0     4342 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/run_tests__test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.664377 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/
+-rw-rw-rw-   0        0        0        8 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/__init__.py
+-rw-rw-rw-   0        0        0      899 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/fake_2_test.py
+-rw-rw-rw-   0        0        0      716 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/sleep_test.py
+-rw-rw-rw-   0        0        0     4323 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/rwobject_test.py
+-rw-rw-rw-   0        0        0      671 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/scrap_tags.py
+-rw-rw-rw-   0        0        0     9160 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/scrap_test.py
+-rw-rw-rw-   0        0        0      190 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sndarray_tags.py
+-rw-rw-rw-   0        0        0     6297 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sndarray_test.py
+-rw-rw-rw-   0        0        0    46638 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sprite_test.py
+-rw-rw-rw-   0        0        0   163734 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surface_test.py
+-rw-rw-rw-   0        0        0      260 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surfarray_tags.py
+-rw-rw-rw-   0        0        0    25768 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surfarray_test.py
+-rw-rw-rw-   0        0        0     4728 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surflock_test.py
+-rw-rw-rw-   0        0        0     1463 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sysfont_test.py
+-rw-rw-rw-   0        0        0       21 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_test_.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.683378 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/
+-rw-rw-rw-   0        0        0     5371 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/__init__.py
+-rw-rw-rw-   0        0        0    14843 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/arrinter.py
+-rw-rw-rw-   0        0        0     9128 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/async_sub.py
+-rw-rw-rw-   0        0        0    23706 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/buftools.py
+-rw-rw-rw-   0        0        0      495 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/endian.py
+-rw-rw-rw-   0        0        0   152382 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/png.py
+-rw-rw-rw-   0        0        0    12049 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/run_tests.py
+-rw-rw-rw-   0        0        0     2483 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/test_machinery.py
+-rw-rw-rw-   0        0        0     9434 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/test_runner.py
+-rw-rw-rw-   0        0        0     7842 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/threads_test.py
+-rw-rw-rw-   0        0        0    15336 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/time_test.py
+-rw-rw-rw-   0        0        0     3223 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/touch_test.py
+-rw-rw-rw-   0        0        0    49044 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/transform_test.py
+-rw-rw-rw-   0        0        0     1536 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/version_test.py
+-rw-rw-rw-   0        0        0      696 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/video_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.686385 myNeuropsydia-0.1.7/myNeuropsydia/pygame/threads/
+-rw-rw-rw-   0        0        0     8074 2022-03-16 08:50:26.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/threads/__init__.py
+-rw-rw-rw-   0        0        0     2526 2022-03-16 08:50:25.000000 myNeuropsydia-0.1.7/myNeuropsydia/pygame/version.py
+-rw-rw-rw-   0        0        0    16381 2023-05-04 09:09:54.000000 myNeuropsydia-0.1.7/myNeuropsydia/scale.py
+-rw-rw-rw-   0        0        0     8770 2023-05-04 10:29:19.000000 myNeuropsydia-0.1.7/myNeuropsydia/start.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.691378 myNeuropsydia-0.1.7/myNeuropsydia/tests/
+-rw-rw-rw-   0        0        0       30 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/tests/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-04-20 09:43:09.000000 myNeuropsydia-0.1.7/myNeuropsydia/tests/test_color.py
+-rw-rw-rw-   0        0        0     8526 2023-05-04 10:24:43.000000 myNeuropsydia-0.1.7/myNeuropsydia/write.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:18.113377 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10661 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-04 18:30:17.000000 myNeuropsydia-0.1.7/myNeuropsydia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 18:30:18.695376 myNeuropsydia-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-05-04 18:30:03.000000 myNeuropsydia-0.1.7/setup.py
```

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/ask.py` & `myNeuropsydia-0.1.7/myNeuropsydia/ask.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/choice.py` & `myNeuropsydia-0.1.7/myNeuropsydia/choice.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/core.py` & `myNeuropsydia-0.1.7/myNeuropsydia/core.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/absorption_desk.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_desk.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/absorption_man.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/absorption_man.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_absorption.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_absorption_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_absorption_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_blue.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_blue_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_blue_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_green.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_green_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_green_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_orange.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_orange_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_orange_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_purple.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_purple_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_purple_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_red.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_red_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_red_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_teal.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_teal_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_teal_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_yellow.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/cursor_yellow_validated.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/cursor_yellow_validated.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/binary/scale_point.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/binary/scale_point.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/LiberationMono-Bold.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/LiberationMono-Regular.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/LiberationMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoBlack.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBlack.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoBold.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoBold.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoLight.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoLight.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/RobotoRegular.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/RobotoRegular.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/Timeless-Bold.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless-Bold.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/font/Timeless.ttf` & `myNeuropsydia-0.1.7/myNeuropsydia/files/font/Timeless.ttf`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/N.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/N.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_HEAD_white.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_PSY_blue.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Neuropsydia_TEXT_white.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/Python.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/Python.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/icon.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/icon.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/files/logo/neuropsydia_banner.png` & `myNeuropsydia-0.1.7/myNeuropsydia/files/logo/neuropsydia_banner.png`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/fill_form.py` & `myNeuropsydia-0.1.7/myNeuropsydia/fill_form.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/image.py` & `myNeuropsydia-0.1.7/myNeuropsydia/image.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/io.py` & `myNeuropsydia-0.1.7/myNeuropsydia/io.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/meta.py` & `myNeuropsydia-0.1.7/myNeuropsydia/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-import neurokit as nk
+ 
 import pandas as pd
 import datetime
 import random
 
 from .path import *
 from .core import *
 from .write import *
@@ -313,11 +313,9 @@
     df["Time_End"] = datetime.datetime.now()
     df["Total_Duration"] = (datetime.datetime.now()-time_start).total_seconds()
 
     if dimensions_mean == True:
         for dim in set(df[dimensions_key_name]):
             df[dim] = df[(df[dimensions_key_name]==dim)]["Answer"].mean()
 
-    if results_save == True:
-        nk.save_data(df, filename=results_name, path=results_path, participant_id=participant_id, index=True, index_label="Item_Number")
-
+    
     return(df)
```

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/miscellaneous.py` & `myNeuropsydia-0.1.7/myNeuropsydia/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/procedures.py` & `myNeuropsydia-0.1.7/myNeuropsydia/procedures.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/__init__.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/__init__.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/__pyinstaller/hook-pygame.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/__pyinstaller/hook-pygame.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/_camera_opencv.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/_camera_opencv.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/_camera_vidcapture.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/_camera_vidcapture.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/camera.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/camera.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/colordict.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/colordict.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/cursors.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/cursors.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/draw_py.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/draw_py.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/aacircle.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/aacircle.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/aliens.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/aliens.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/arraydemo.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/arraydemo.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/audiocapture.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/audiocapture.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/blend_fill.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/blend_fill.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/blit_blends.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/blit_blends.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/camera.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/camera.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/chimp.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/chimp.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/cursors.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/cursors.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/dropevent.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/dropevent.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/eventlist.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/eventlist.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/font_viewer.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/font_viewer.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/fonty.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/fonty.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/freetype_misc.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/freetype_misc.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/glcube.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/glcube.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/headless_no_windows_needed.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/headless_no_windows_needed.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/joystick.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/joystick.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/liquid.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/liquid.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/mask.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/mask.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/midi.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/midi.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/moveit.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/moveit.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/music_drop_fade.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/music_drop_fade.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/pixelarray.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/pixelarray.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/playmus.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/playmus.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/prevent_display_stretching.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/prevent_display_stretching.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/resizing_new.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/resizing_new.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/scaletest.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scaletest.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/scrap_clipboard.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scrap_clipboard.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/scroll.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/scroll.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/setmodescale.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/setmodescale.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/sound.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sound.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/sound_array_demos.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sound_array_demos.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/sprite_texture.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/sprite_texture.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/stars.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/stars.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/testsprite.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/testsprite.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/textinput.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/textinput.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/vgrade.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/vgrade.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/examples/video.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/examples/video.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/fastevent.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/fastevent.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/freetype.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/freetype.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/ftfont.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/ftfont.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/locals.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/locals.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/midi.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/midi.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/pkgdata.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/pkgdata.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/sndarray.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/sndarray.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/sprite.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/sprite.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/surfarray.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/surfarray.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/sysfont.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/sysfont.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/__init__.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/__main__.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/base_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/blit_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/blit_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/bufferproxy_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/bufferproxy_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/color_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/color_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/constants_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/controller_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/controller_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/cursors_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/cursors_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/display_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/display_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/docs_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/docs_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/draw_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/draw_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/event_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/event_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/font_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/font_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/freetype_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/freetype_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/ftfont_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/ftfont_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/gfxdraw_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/gfxdraw_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/image__save_gl_surface_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image__save_gl_surface_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/image_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/image_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/imageext_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/imageext_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/joystick_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/joystick_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/key_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/key_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mask_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mask_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/math_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/math_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/midi_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/midi_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mixer_music_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_music_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mixer_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mixer_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/mouse_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/mouse_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/pixelarray_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/pixelarray_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/pixelcopy_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/pixelcopy_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/rect_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/rect_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_3_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_3_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_4_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_4_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_5_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_5_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_6_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/fake_6_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/no_assertions__ret_code_of_1__test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/no_assertions__ret_code_of_1__test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/zero_tests_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/all_ok/zero_tests_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/incomplete_todo_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/incomplete_todo_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/magic_tag_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/magic_tag_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/everything/sleep_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/everything/sleep_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/invisible_tag_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/invisible_tag_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/exclude/magic_tag_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/exclude/magic_tag_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_3_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_3_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_4_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/failures1/fake_4_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_3_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete/fake_3_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_3_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/incomplete_todo/fake_3_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_1_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_1_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/infinite_loop/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_3_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_3_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_4_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stderr/fake_4_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_3_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_3_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_4_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/print_stdout/fake_4_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/run_tests__test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/run_tests__test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/timeout/fake_2_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/fake_2_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/run_tests__tests/timeout/sleep_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/run_tests__tests/timeout/sleep_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/rwobject_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/rwobject_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/scrap_tags.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/scrap_tags.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/scrap_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/scrap_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sndarray_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sndarray_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sprite_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sprite_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surface_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surface_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surfarray_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surfarray_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/surflock_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/surflock_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/sysfont_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/sysfont_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/__init__.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/arrinter.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/arrinter.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/async_sub.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/async_sub.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/buftools.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/buftools.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/png.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/png.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/run_tests.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/run_tests.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/test_machinery.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/test_machinery.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/test_utils/test_runner.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/test_utils/test_runner.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/threads_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/threads_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/time_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/time_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/touch_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/touch_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/transform_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/transform_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/version_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/version_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/tests/video_test.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/tests/video_test.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/threads/__init__.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/pygame/version.py` & `myNeuropsydia-0.1.7/myNeuropsydia/pygame/version.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/scale.py` & `myNeuropsydia-0.1.7/myNeuropsydia/scale.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/start.py` & `myNeuropsydia-0.1.7/myNeuropsydia/start.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/myNeuropsydia/write.py` & `myNeuropsydia-0.1.7/myNeuropsydia/write.py`

 * *Files identical despite different names*

### Comparing `myNeuropsydia-0.1.5/setup.py` & `myNeuropsydia-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 setup(
     name='myNeuropsydia',
     packages=find_packages(),
-    version='0.1.5',
+    version='0.1.7',
     description='Partially fixed version of Neuropsydia library, a Python module for creating experiments, tasks and questionnaires',
     author='Laborde',
     license='ENS_Paris_Saclay',
     package_data = {
                 	"myNeuropsydia.files.font":["*.ttf", "*.otf"],
                 	"myNeuropsydia.files.binary":["*.png"],
                 	"myNeuropsydia.files.logo":["*.png"]},
     dependency_links=[
 	"https://github.com/neuropsychology/NeuroKit.py/zipball/master"],
     install_requires=['Pillow',
-                      'cryptography',
-                      'neurokit',
+                      'cryptography', 
                       'numpy',
                       'pandas', 
                       'python-docx',
                       'pyxid',
                       'statsmodels'],
 )
```

