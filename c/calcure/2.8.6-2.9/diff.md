# Comparing `tmp/calcure-2.8.6.tar.gz` & `tmp/calcure-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcure-2.8.6.tar", last modified: Wed Apr 12 05:06:50 2023, max compression
+gzip compressed data, was "calcure-2.9.tar", last modified: Thu May  4 11:42:08 2023, max compression
```

## Comparing `calcure-2.8.6.tar` & `calcure-2.9.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.8.6/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-04-12 05:06:50.951349 calcure-2.8.6/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.8.6/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/calcure/
--rw-r--r--   0 r         (1000) r         (1000)    42325 2023-04-12 05:05:40.000000 calcure-2.8.6/calcure/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.8.6/calcure/calendars.py
--rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.8.6/calcure/colors.py
--rw-r--r--   0 r         (1000) r         (1000)    20292 2023-04-12 05:05:37.000000 calcure-2.8.6/calcure/configuration.py
--rw-r--r--   0 r         (1000) r         (1000)    22876 2023-04-12 05:05:26.000000 calcure-2.8.6/calcure/controls.py
--rw-r--r--   0 r         (1000) r         (1000)    12945 2023-03-01 12:10:25.000000 calcure-2.8.6/calcure/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3564 2023-03-14 09:29:08.000000 calcure-2.8.6/calcure/dialogues.py
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-04-05 00:48:10.000000 calcure-2.8.6/calcure/errors.py
--rw-r--r--   0 r         (1000) r         (1000)     3687 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/importers.py
--rw-r--r--   0 r         (1000) r         (1000)    14438 2023-03-14 04:33:36.000000 calcure-2.8.6/calcure/loaders.py
--rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/savers.py
--rw-r--r--   0 r         (1000) r         (1000)     4534 2023-04-05 00:48:09.000000 calcure-2.8.6/calcure/screen.py
--rw-r--r--   0 r         (1000) r         (1000)      836 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/test_async.py
--rw-r--r--   0 r         (1000) r         (1000)      463 2023-03-14 13:14:44.000000 calcure-2.8.6/calcure/test_decoration.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/calcure/translations/
--rw-r--r--   0 r         (1000) r         (1000)     5562 2023-03-10 03:04:29.000000 calcure-2.8.6/calcure/translations/br.py
--rw-r--r--   0 r         (1000) r         (1000)     5026 2023-03-10 03:05:54.000000 calcure-2.8.6/calcure/translations/en.py
--rw-r--r--   0 r         (1000) r         (1000)     6015 2023-03-10 03:05:59.000000 calcure-2.8.6/calcure/translations/fr.py
--rw-r--r--   0 r         (1000) r         (1000)     6036 2023-03-10 03:04:49.000000 calcure-2.8.6/calcure/translations/it.py
--rw-r--r--   0 r         (1000) r         (1000)     7908 2023-03-10 03:06:06.000000 calcure-2.8.6/calcure/translations/ru.py
--rw-r--r--   0 r         (1000) r         (1000)     5895 2023-03-10 03:05:11.000000 calcure-2.8.6/calcure/translations/tr.py
--rw-r--r--   0 r         (1000) r         (1000)     5239 2023-03-10 03:05:22.000000 calcure-2.8.6/calcure/translations/zh.py
--rw-r--r--   0 r         (1000) r         (1000)      905 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/weather.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/calcure.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      721 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       49 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       23 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        8 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.8.6/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-04-12 05:06:50.951349 calcure-2.8.6/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.8.6/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     3906 2023-05-04 11:42:08.356486 calcure-2.9/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/calcure/
+-rw-r--r--   0 r         (1000) r         (1000)    41137 2023-05-04 11:06:59.000000 calcure-2.9/calcure/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9/calcure/calendars.py
+-rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9/calcure/colors.py
+-rw-r--r--   0 r         (1000) r         (1000)    20290 2023-05-04 10:23:28.000000 calcure-2.9/calcure/configuration.py
+-rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-04 11:25:37.000000 calcure-2.9/calcure/controls.py
+-rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-04 11:25:39.000000 calcure-2.9/calcure/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3564 2023-05-03 20:15:00.000000 calcure-2.9/calcure/dialogues.py
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-05-03 19:07:50.000000 calcure-2.9/calcure/errors.py
+-rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9/calcure/importers.py
+-rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9/calcure/loaders.py
+-rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9/calcure/savers.py
+-rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-03 18:19:49.000000 calcure-2.9/calcure/screen.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/calcure/translations/
+-rw-r--r--   0 r         (1000) r         (1000)     5793 2023-05-04 11:34:28.000000 calcure-2.9/calcure/translations/br.py
+-rw-r--r--   0 r         (1000) r         (1000)     5289 2023-05-04 11:33:46.000000 calcure-2.9/calcure/translations/en.py
+-rw-r--r--   0 r         (1000) r         (1000)     6251 2023-05-04 11:37:01.000000 calcure-2.9/calcure/translations/fr.py
+-rw-r--r--   0 r         (1000) r         (1000)     6283 2023-05-04 11:34:29.000000 calcure-2.9/calcure/translations/it.py
+-rw-r--r--   0 r         (1000) r         (1000)     8277 2023-05-04 11:34:30.000000 calcure-2.9/calcure/translations/ru.py
+-rw-r--r--   0 r         (1000) r         (1000)     6134 2023-05-04 11:34:30.000000 calcure-2.9/calcure/translations/tr.py
+-rw-r--r--   0 r         (1000) r         (1000)     5433 2023-05-04 11:36:18.000000 calcure-2.9/calcure/translations/zh.py
+-rw-r--r--   0 r         (1000) r         (1000)      905 2023-03-01 08:49:55.000000 calcure-2.9/calcure/weather.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/calcure.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     3906 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-04 11:42:08.356486 calcure-2.9/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9/setup.py
```

### Comparing `calcure-2.8.6/LICENSE` & `calcure-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/PKG-INFO` & `calcure-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.8.6
+Version: 2.9
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.8.6/README.md` & `calcure-2.9/README.md`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/calcure/__main__.py` & `calcure-2.9/calcure/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from calcure.translations.tr import *
 elif cf.LANG == "zh":
     from calcure.translations.zh import *
 else:
     from calcure.translations.en import *
 
 
-__version__ = "2.8.6"
+__version__ = "2.9"
 
 
 def read_items_from_user_arguments(screen, user_tasks, user_events, task_saver_csv, event_saver_csv):
     """Read --task and --event flags from user arguments to create new tasks or events"""
     try:
         opts, _ = getopt.getopt(sys.argv[1:], "pjhvi", ["folder=", "config=", "task=", "event="])
         for opt, arg in opts:
@@ -75,32 +75,32 @@
         self.y = y
         self.x = x
 
     def fill_background(self):
         """Fill the screen background with background color"""
         y_max, x_max = self.stdscr.getmaxyx()
         for index in range(y_max - 1):
-            self.stdscr.addstr(index, 0, " " * x_max, curses.color_pair(1))
+            self.stdscr.addstr(index, 0, " " * x_max, curses.color_pair(Color.EMPTY.value))
 
     def display_line(self, y, x, text, color, bold=False, underlined=False):
         """Display the line of text respecting the slyling and available space"""
 
         # Make sure that we display inside the screen:
         y_max, x_max = self.stdscr.getmaxyx()
         if y >= y_max or x >= x_max:
             return
 
         # Cut the text if it does not fit the screen:
         real_text = text.replace('\u0336', "")
         number_of_characters = len(real_text)
-        available_space = x_max - x
+        avaliable_space = x_max - x
         number_of_special = text.count('\u0336')
-        if number_of_characters > available_space:
+        if number_of_characters > avaliable_space:
             coefficient = 2 if number_of_special > 0 else 1
-            text = f"{text[:(available_space - 1)*coefficient]}"
+            text = f"{text[:(avaliable_space - 1)*coefficient]}"
 
         try:
             if bold and underlined:
                 self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_BOLD | curses.A_UNDERLINE)
             elif bold and not underlined:
                 self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_BOLD)
             elif underlined and not bold:
@@ -257,14 +257,17 @@
         """Select the right icon for the event"""
         return cf.EVENT_ICON
 
     @property
     def color(self):
         """Assign color depending on the status or calendar number if it's from .ics file"""
         if self.event.calendar_number is None:
+
+            if self.event.status == Status.DONE:
+                return Color.DONE
             if self.event.status == Status.IMPORTANT:
                 return Color.IMPORTANT
             if self.event.status == Status.UNIMPORTANT:
                 return Color.UNIMPORTANT
             return Color.EVENTS
         else:
             for color in Color:
@@ -497,15 +500,15 @@
     def __init__(self, stdscr, y, x, title, screen):
         super().__init__(stdscr, y, x)
         self.title = title
         self.screen = screen
 
     def render(self):
         """Render this view on the screen"""
-        if self.screen.active_pane and self.screen.split:
+        if self.screen.is_active_pane and self.screen.split:
             self.display_line(0, self.screen.x_min, self.title, Color.ACTIVE_PANE, cf.BOLD_ACTIVE_PANE, cf.UNDERLINED_ACTIVE_PANE)
         else:
             self.display_line(0, self.screen.x_min, self.title, Color.CALENDAR_HEADER, cf.BOLD_TITLE, cf.UNDERLINED_TITLE)
 
 
 class HeaderView(View):
     """Show the header that includes the weather, time, and title"""
@@ -697,19 +700,17 @@
     @property
     def icon(self):
         """Icon of today"""
         return cf.TODAY_ICON if self.screen.date == self.screen.today else ''
 
     def render(self):
         """Render this view on the screen"""
-        self.screen.state = AppState.CALENDAR
+        self.screen.currently_drawn = AppState.CALENDAR
         if self.screen.x_max < 6 or self.screen.y_max < 3:
             return
-        # self.fill_background()
-        curses.halfdelay(255)
 
         # Form a string with month, year, and day with today icon:
         month_names = MONTHS_PERSIAN if cf.USE_PERSIAN_CALENDAR else MONTHS
         month_string = str(month_names[self.screen.month-1])
         # date_string = f'{month_string} {self.screen.day}, {self.screen.year} {icon}'
         date_string = f'{month_string} {self.screen.year}'
 
@@ -753,17 +754,16 @@
         self.birthdays = birthdays
         self.user_tasks = user_tasks
         self.user_ics_tasks = user_ics_tasks
         self.screen = screen
 
     def render(self):
         """Render this view on the screen"""
-        self.screen.state = AppState.CALENDAR
+        self.screen.currently_drawn = AppState.CALENDAR
         if self.screen.x_max < 6 or self.screen.y_max < 3: return
-        curses.halfdelay(255)
 
         # Info about the month:
         month_names = MONTHS_PERSIAN if cf.USE_PERSIAN_CALENDAR else MONTHS
         month_year_string = month_names[self.screen.month-1] + " " + str(self.screen.year)
         dates = Calendar(cf.START_WEEK_DAY - 1, cf.USE_PERSIAN_CALENDAR).monthdayscalendar(self.screen.year, self.screen.month)
 
         y_cell = (self.screen.y_max - 3) // 6
@@ -801,35 +801,21 @@
 class JournalScreenView(View):
     def __init__(self, stdscr, y, x, weather, user_tasks, user_ics_tasks, screen):
         super().__init__(stdscr, y, x)
         self.weather = weather
         self.user_tasks = user_tasks
         self.user_ics_tasks = user_ics_tasks
         self.screen = screen
-        self.refresh_time = 255
-
-    def calculate_refresh_rate(self):
-        """Check if a timer is running and change the refresh rate"""
-        self.refresh_time = 255
-        for task in self.user_tasks.items:
-            if task.timer.is_counting:
-                self.refresh_time = cf.REFRESH_INTERVAL * 10
-                self.screen.refresh_now = False
-                break
 
     def render(self):
         """Journal view showing all tasks"""
-        self.screen.state = AppState.JOURNAL
+        self.screen.currently_drawn = AppState.JOURNAL
         if self.screen.x_max < 6 or self.screen.y_max < 3:
             return
 
-        # Check if any of the timers is counting, and increase the update time:
-        self.calculate_refresh_rate()
-        curses.halfdelay(self.refresh_time)
-
         # Display header and footer:
         header_view = HeaderView(self.stdscr, 0, 0, cf.JOURNAL_HEADER, self.weather, self.screen)
         header_view.render()
 
         # Display the tasks:
         journal_view = JournalView(self.stdscr, 2, self.screen.x_min, self.user_tasks, self.user_ics_tasks, self.screen)
         journal_view.render()
@@ -845,15 +831,14 @@
     def calibrate_position(self):
         """Depending on the screen space calculate the best position"""
         self.y_max, self.x_max = self.stdscr.getmaxyx()
 
     def render(self):
         """Draw the welcome screen"""
         self.calibrate_position()
-        curses.halfdelay(255)
         self.stdscr.clear()
         self.fill_background()
 
         if self.x_max < len(MSG_WELCOME_4)+2 or self.y_max < 12:
             self.display_line(0, 0, "Welcome!", Color.ACTIVE_PANE)
             return
 
@@ -895,15 +880,14 @@
             self.global_shift_y = 0
 
     def render(self):
         """Draw the help screen"""
         self.calibrate_position()
         if self.x_max < 6 or self.y_max < 3:
             return
-        curses.halfdelay(255)
         self.stdscr.clear()
         self.fill_background()
 
         # Left column:
         self.display_line(self.global_shift_y, self.global_shift_x + 1, f"{MSG_NAME} {__version__}",
                             Color.ACTIVE_PANE, cf.BOLD_TITLE, cf.UNDERLINED_TITLE)
         self.display_line(self.global_shift_y + 2, self.global_shift_x + 8,
@@ -992,62 +976,50 @@
         screen.state = AppState.WELCOME
     while screen.state == AppState.WELCOME:
         welcome_screen_view.render()
         control_welcome_screen(stdscr, screen)
 
     # Running different screens depending on the state:
     while screen.state != AppState.EXIT:
-        if not screen.split:
-            stdscr.clear()
-            app_view.fill_background()
-        screen.active_pane = False
-
-        # CALENDARS
-
-        # Monthly (active) screen:
-        if screen.state == AppState.CALENDAR and screen.calendar_state == CalState.MONTHLY:
-            if screen.split and not screen.selection_mode:
-                stdscr.clear()
-                app_view.fill_background()
-                journal_screen_view.render()
-            screen.active_pane = True
-            monthly_screen_view.render()
-            if screen.split: separator_view.render()
-            footer_view.render()
-            error_view.render()
-            control_monthly_screen(stdscr, screen, user_events, importer)
+        stdscr.clear()
+        app_view.fill_background()
 
-        # Daily (active) screen:
-        elif screen.state == AppState.CALENDAR and screen.calendar_state == CalState.DAILY:
-            if screen.split and not screen.selection_mode:
-                stdscr.clear()
-                app_view.fill_background()
+        # Calculate screen refreh rate:
+        curses.halfdelay(200)
+        if user_tasks.has_active_timer and screen.state == AppState.JOURNAL:
+            curses.halfdelay(cf.REFRESH_INTERVAL * 10)
+
+        # Calendar screens:
+        if screen.state == AppState.CALENDAR:
+
+            if screen.calendar_state == CalState.MONTHLY:
+                monthly_screen_view.render()
+            else:
+                daily_screen_view.render()
+
+            if screen.split:
                 journal_screen_view.render()
-            screen.active_pane = True
-            daily_screen_view.render()
-            if screen.split: separator_view.render()
+                separator_view.render()
             footer_view.render()
             error_view.render()
-            control_daily_screen(stdscr, screen, user_events, importer)
 
-        # JOURNAL
+            if screen.calendar_state == CalState.MONTHLY:
+                control_monthly_screen(stdscr, screen, user_events, importer)
+            else:
+                control_daily_screen(stdscr, screen, user_events, importer)
 
-        # Journal (active) screen:
+        # Journal screen:
         elif screen.state == AppState.JOURNAL:
-            if screen.split and not screen.selection_mode:
-                if screen.refresh_now:
-                    stdscr.clear()
-                    app_view.fill_background()
+            if screen.split:
                 if screen.calendar_state == CalState.MONTHLY:
                     monthly_screen_view.render()
                 else:
                     daily_screen_view.render()
-            screen.active_pane = True
+                separator_view.render()
             journal_screen_view.render()
-            if screen.split: separator_view.render()
             footer_view.render()
             error_view.render()
             control_journal_screen(stdscr, screen, user_tasks, importer)
 
         # Help screen:
         elif screen.state == AppState.HELP:
             help_screen_view.render()
```

### Comparing `calcure-2.8.6/calcure/calendars.py` & `calcure-2.9/calcure/calendars.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/calcure/colors.py` & `calcure-2.9/calcure/colors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/calcure/configuration.py` & `calcure-2.9/calcure/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt == '-d':
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt in ('-h'):
                     self.DEFAULT_VIEW = AppState.HELP
                 elif opt in ('-v'):
                     self.DEFAULT_VIEW = AppState.EXIT
-                    print ('Calcure - version 2.8.6')
+                    print ('Calcure - version 2.9')
                 elif opt in ('-i'):
                     self.USE_PERSIAN_CALENDAR = True
         except getopt.GetoptError as e_message:
             logging.error("Invalid user arguments. %s", e_message)
             pass
```

### Comparing `calcure-2.8.6/calcure/controls.py` & `calcure-2.9/calcure/controls.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,71 +63,92 @@
                 event_id = user_events.filter_events_that_month(screen).items[number].item_id
                 user_events.toggle_item_status(event_id, Status.UNIMPORTANT)
         if screen.key == 'u':
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_RESET)
             if user_events.filter_events_that_month(screen).is_valid_number(number):
                 event_id = user_events.filter_events_that_month(screen).items[number].item_id
                 user_events.toggle_item_status(event_id, Status.NORMAL)
+        if screen.key == 'd':
+            number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_DONE)
+            if user_events.filter_events_that_month(screen).is_valid_number(number):
+                event_id = user_events.filter_events_that_month(screen).items[number].item_id
+                user_events.toggle_item_status(event_id, Status.DONE)
 
         # Toggle event privacy:
         if screen.key == '.':
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_PRIVACY)
             if user_events.filter_events_that_month(screen).is_valid_number(number):
                 event_id = user_events.filter_events_that_month(screen).items[number].item_id
                 user_events.toggle_item_privacy(event_id)
 
         # Delete event:
-        if screen.key in ['d', 'x']:
+        if screen.key in ['x']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_DEL)
             if user_events.filter_events_that_month(screen).is_valid_number(number):
                 event_id = user_events.filter_events_that_month(screen).items[number].item_id
                 user_events.delete_item(event_id)
 
-        # Edit event:
-        if screen.key in ['e', 'c']:
+        # Rename event:
+        if screen.key in ['e', 'r']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_REN)
             if user_events.filter_events_that_month(screen).is_valid_number(number):
                 event_id = user_events.filter_events_that_month(screen).items[number].item_id
                 clear_line(stdscr, screen.y_max-2)
                 new_name = input_string(stdscr, screen.y_max-2, 0, MSG_NEW_TITLE, screen.x_max-len(MSG_NEW_TITLE)-2)
                 user_events.rename_item(event_id, new_name)
 
         # Move event:
-        if screen.key == 'm':
-            number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_MOVE)
+        if screen.key in ['m', 'M']:
+            number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_MV)
             if user_events.filter_events_that_month(screen).is_valid_number(number):
                 event_id = user_events.filter_events_that_month(screen).items[number].item_id
                 clear_line(stdscr, screen.y_max-2)
-                question = f'{MSG_EVENT_MOVE_TO} {screen.year}/{screen.month}/'
-                day = input_day(stdscr, screen.y_max-2, 0, question)
-                if screen.is_valid_day(day):
-                    user_events.change_day(event_id, day)
+                if screen.key == 'm':
+                    year, month, day = input_date(stdscr, screen.y_max-2, 0, MSG_EVENT_MV_TO)
+                    if screen.is_valid_date(year, month, day):
+                        user_events.change_date(event_id, year, month, day)
+
+                if screen.key == 'M':
+                    question = f'{MSG_EVENT_MV_TO_D} {screen.year}/{screen.month}/'
+                    day = input_day(stdscr, screen.y_max-2, 0, question)
+                    if screen.is_valid_day(day):
+                        user_events.change_day(event_id, day)
 
     # Otherwise, we check for user input:
     else:
         # Wait for user to press a key:
         screen.key = stdscr.getkey()
 
         # If we need to select an event, change to selection mode:
-        if screen.key in ['h', 'l', 'u', 'i', 'd', 'x', 'e', 'c', 'm', '.']:
+        if screen.key in ['h', 'l', 'u', 'i', 'd', 'x', 'e', 'r', 'c', 'm', 'M', '.']:
             screen.selection_mode = True
 
         # Navigation:
         if screen.key in ["n", "j", "KEY_UP", "KEY_RIGHT"]:
             screen.next_month()
         if screen.key in ["p", "k", "KEY_DOWN", "KEY_LEFT"]:
             screen.previous_month()
-        if screen.key in ["KEY_HOME", "G"]:
+        if screen.key in ["KEY_HOME", "R"]:
             screen.reset_to_today()
 
-        # Handle "g" as go to selected day:
+        # Handle "g" and "G" as go to selected day:
         if screen.key == "g":
-            question = f'Go to date: {str(screen.year)}/{str(screen.month)}/'
+            clear_line(stdscr, screen.y_max-2, 0)
+            year, month, day = input_date(stdscr, screen.y_max-2, 0, MSG_GOTO)
+            if screen.is_valid_date(year, month, day):
+                screen.day = day
+                screen.month = month
+                screen.year = year
+                screen.calendar_state = CalState.DAILY
+
+        if screen.key == "G":
+            clear_line(stdscr, screen.y_max-2, 0)
+            question = f"{MSG_GOTO_D} {screen.year}/{screen.month}/"
             day = input_day(stdscr, screen.y_max-2, 0, question)
-            if screen.is_valid_day(day):
+            if screen.is_valid_date(screen.year, screen.month, day):
                 screen.day = day
                 screen.calendar_state = CalState.DAILY
 
         # Change the view to daily:
         if screen.key == "v":
             screen.day = 1
             screen.calendar_state = CalState.DAILY
@@ -200,64 +221,75 @@
                 item_id = user_events.filter_events_that_day(screen).items[number].item_id
                 user_events.toggle_item_status(item_id, Status.UNIMPORTANT)
         if screen.key == 'u':
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_RESET)
             if user_events.filter_events_that_day(screen).is_valid_number(number):
                 item_id = user_events.filter_events_that_day(screen).items[number].item_id
                 user_events.toggle_item_status(item_id, Status.NORMAL)
+        if screen.key == 'd':
+            number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_DONE)
+            if user_events.filter_events_that_day(screen).is_valid_number(number):
+                item_id = user_events.filter_events_that_day(screen).items[number].item_id
+                user_events.toggle_item_status(item_id, Status.DONE)
 
         # Toggle event privacy:
         if screen.key == '.':
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_PRIVACY)
             if user_events.filter_events_that_day(screen).is_valid_number(number):
                 event_id = user_events.filter_events_that_day(screen).items[number].item_id
                 user_events.toggle_item_privacy(event_id)
 
         # Delete event:
-        if screen.key in ['d', 'x']:
+        if screen.key in ['x']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_DEL)
             if user_events.filter_events_that_day(screen).is_valid_number(number):
                 item_id = user_events.filter_events_that_day(screen).items[number].item_id
                 user_events.delete_item(item_id)
 
-        # Edit event:
-        if screen.key in ['e', 'c']:
+        # Remane event:
+        if screen.key in ['e', 'r']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_REN)
             if user_events.filter_events_that_day(screen).is_valid_number(number):
                 item_id = user_events.filter_events_that_day(screen).items[number].item_id
                 clear_line(stdscr, screen.y_max-2)
                 new_name = input_string(stdscr, screen.y_max-2, 0, MSG_NEW_TITLE, screen.x_max-len(MSG_NEW_TITLE)-2)
                 user_events.rename_item(item_id, new_name)
 
         # Move event:
-        if screen.key == 'm':
-            number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_MOVE)
+        if screen.key in ['m', 'M']:
+            number = input_integer(stdscr, screen.y_max-2, 0, MSG_EVENT_MV)
             if user_events.filter_events_that_day(screen).is_valid_number(number):
                 item_id = user_events.filter_events_that_day(screen).items[number].item_id
                 clear_line(stdscr, screen.y_max-2)
-                question = f'{MSG_EVENT_MOVE_TO}{screen.year}/{screen.month}/'
-                day = input_day(stdscr, screen.y_max-2, 0, question)
-                if screen.is_valid_day(day):
-                    user_events.change_day(item_id, day)
+                if screen.key == 'm':
+                    year, month, day = input_date(stdscr, screen.y_max-2, 0, MSG_EVENT_MV_TO)
+                    if screen.is_valid_date(year, month, day):
+                        user_events.change_date(event_id, year, month, day)
+
+                if screen.key == 'M':
+                    question = f'{MSG_EVENT_MV_TO_D}{screen.year}/{screen.month}/'
+                    day = input_day(stdscr, screen.y_max-2, 0, question)
+                    if screen.is_valid_day(day):
+                        user_events.change_day(event_id, day)
 
     # Otherwise, we check for user input:
     else:
         # Wait for user to press a key:
         screen.key = stdscr.getkey()
 
         # If we need to select an event, change to selection mode:
-        if screen.key in ['h', 'l', 'u', 'i', 'd', 'x', 'e', 'c', 'm', '.']:
+        if screen.key in ['h', 'l', 'u', 'i', 'd', 'x', 'e', 'r', 'c', 'm', 'M', '.']:
             screen.selection_mode = True
 
         # Navigation:
         if screen.key in ["n", "j", "KEY_UP", "KEY_RIGHT"]:
             screen.next_day()
         if screen.key in ["p", "k", "KEY_DOWN", "KEY_LEFT"]:
             screen.previous_day()
-        if screen.key in ["KEY_HOME", "G"]:
+        if screen.key in ["KEY_HOME", "R"]:
             screen.reset_to_today()
 
         # Add single event:
         if screen.key == "a":
             name = input_string(stdscr, screen.y_max-2, 0, MSG_EVENT_TITLE, screen.x_max-len(MSG_EVENT_TITLE)-2)
             item_id = user_events.items[-1].item_id + 1 if not user_events.is_empty() else 1
             user_events.add_item(UserEvent(item_id, screen.year, screen.month, screen.day, name, 1, Frequency.ONCE, Status.NORMAL, False))
@@ -274,14 +306,32 @@
 
         # Import from calcurse:
         if screen.key == "C":
             confirmed = ask_confirmation(stdscr, MSG_EVENT_IMP, cf.ASK_CONFIRMATIONS)
             if confirmed:
                 importer.import_events_from_calcurse()
 
+        # Handle "g" and "G" as go to selected (prefilled) day:
+        if screen.key == "g":
+            clear_line(stdscr, screen.y_max-2, 0)
+            year, month, day = input_date(stdscr, screen.y_max-2, 0, MSG_GOTO)
+            if screen.is_valid_date(year, month, day):
+                screen.day = day
+                screen.month = month
+                screen.year = year
+                screen.calendar_state = CalState.DAILY
+
+        if screen.key == "G":
+            clear_line(stdscr, screen.y_max-2, 0)
+            question = f"{MSG_GOTO_D} {screen.year}/{screen.month}/"
+            day = input_day(stdscr, screen.y_max-2, 0, question)
+            if screen.is_valid_date(screen.year, screen.month, day):
+                screen.day = day
+                screen.calendar_state = CalState.DAILY
+
         # Change the view to monthly:
         if screen.key == "v":
             screen.calendar_state = CalState.MONTHLY
 
         # Other actions:
         if vim_style_exit(stdscr, screen):
             confirmed = ask_confirmation(stdscr, MSG_EXIT, cf.ASK_CONFIRMATIONS)
@@ -350,40 +400,40 @@
                 task_id = user_tasks.items[number].item_id
                 user_tasks.toggle_item_status(task_id, Status.UNIMPORTANT)
         if screen.key == 'u':
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_RES)
             if user_tasks.is_valid_number(number):
                 task_id = user_tasks.items[number].item_id
                 user_tasks.toggle_item_status(task_id, Status.NORMAL)
-        if screen.key == 'v':
+        if screen.key in ['d', 'v']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_DONE)
             if user_tasks.is_valid_number(number):
                 task_id = user_tasks.items[number].item_id
                 user_tasks.toggle_item_status(task_id, Status.DONE)
 
         # Toggle task privacy:
         if screen.key == '.':
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_PRIVACY)
             if user_tasks.is_valid_number(number):
                 task_id = user_tasks.items[number].item_id
                 user_tasks.toggle_item_privacy(task_id)
 
         # Modify the task:
-        if screen.key in ['d', 'x']:
+        if screen.key in ['x']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_DEL)
             if user_tasks.is_valid_number(number):
                 task_id = user_tasks.items[number].item_id
                 user_tasks.delete_item(task_id)
         if screen.key == 'm':
             number_from = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_MOVE)
             if user_tasks.is_valid_number(number_from):
                 clear_line(stdscr, screen.y_max-2)
                 number_to = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_MOVE_TO)
                 user_tasks.move_task(number_from, number_to)
-        if screen.key in ['e', 'c']:
+        if screen.key in ['e', 'r']:
             number = input_integer(stdscr, screen.y_max-2, 0, MSG_TS_EDIT)
             if user_tasks.is_valid_number(number):
                 task_id = user_tasks.items[number].item_id
                 clear_line(stdscr, number+2, screen.x_min)
                 new_name = input_string(stdscr, number+2, screen.x_min, cf.TODO_ICON+' ', screen.x_max-4)
                 user_tasks.rename_item(task_id, new_name)
 
@@ -404,34 +454,34 @@
 
     # Otherwise, we check for user input:
     else:
         # Wait for user to press a key:
         screen.key = stdscr.getkey()
 
         # If we need to select a task, change to selection mode:
-        if screen.key in ['t', 'T', 'h', 'l', 'v', 'u', 'i', 's', 'd', 'x', 'e', 'c', 'A', 'm', '.', 'f', 'F']:
+        if screen.key in ['t', 'T', 'h', 'l', 'v', 'u', 'i', 's', 'd', 'x', 'e', 'r', 'c', 'A', 'm', '.', 'f', 'F']:
             screen.selection_mode = True
 
         # Add single task:
         if screen.key == "a":
             clear_line(stdscr, len(user_tasks.items) + 2, screen.x_min)
             task_name = input_string(stdscr, len(user_tasks.items) + 2, screen.x_min, cf.TODO_ICON+' ', screen.x_max - 4)
             task_id = user_tasks.generate_id()
             user_tasks.add_item(Task(task_id, task_name, Status.NORMAL, Timer([]), False))
 
         # Bulk operations:
-        if screen.key == "V":
+        if screen.key in ["V", "D"]:
             user_tasks.change_all_statuses(Status.DONE)
         if screen.key == "U":
             user_tasks.change_all_statuses(Status.NORMAL)
         if screen.key == "L":
             user_tasks.change_all_statuses(Status.UNIMPORTANT)
         if screen.key in ["I", "H"]:
             user_tasks.change_all_statuses(Status.IMPORTANT)
-        if screen.key in ["D", "X"]:
+        if screen.key in ["X"]:
             confirmed = ask_confirmation(stdscr, MSG_TS_DEL_ALL, cf.ASK_CONFIRMATIONS)
             if confirmed:
                 user_tasks.delete_all_items()
 
         # Imports:
         if screen.key == "C":
             confirmed = ask_confirmation(stdscr, MSG_TS_IM, cf.ASK_CONFIRMATIONS)
```

### Comparing `calcure-2.8.6/calcure/data.py` & `calcure-2.9/calcure/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,21 @@
         events_of_the_month.items = sorted(events_of_the_month.items, key=lambda item: item.day)
         return events_of_the_month
 
 
 class Tasks(Collection):
     """List of tasks created by the user"""
 
+    @property
+    def has_active_timer(self):
+        for item in self.items:
+            if item.timer.is_counting:
+                return True
+        return False
+
     def add_subtask(self, task, number):
         """Add a subtask for certain task in the journal"""
         level = '----'if (self.items[number].name[:2] == '--') else '--'
         task.name = level + task.name
         if 100 > len(task.name) > 0:
             self.items.insert(number+1, task)
             self.changed = True
@@ -305,21 +312,30 @@
                 and event.year == new_event.year
                 and event.month == new_event.month
                 and event.day == new_event.day):
                 return True
         return False
 
     def change_day(self, selected_item_id, new_day):
-        """Move an event to another day"""
+        """Move an event to another day within this month"""
         for item in self.items:
             if item.item_id == selected_item_id:
                 item.day = new_day
                 self.changed = True
                 break
 
+    def change_date(self, selected_item_id, new_year, new_month, new_day):
+        """Move an event to another date"""
+        for item in self.items:
+            if item.item_id == selected_item_id:
+                item.year = new_year
+                item.month = new_month
+                item.day = new_day
+                self.changed = True
+                break
 
 class Birthdays(Events):
     """List of birthdays imported from abook"""
 
     def filter_events_that_day(self, screen):
         """Filter only birthdays that happen on the particular day"""
         events_of_the_day = Events()
```

### Comparing `calcure-2.8.6/calcure/dialogues.py` & `calcure-2.9/calcure/dialogues.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     question = question[:(x_max - x - 1)]
     stdscr.addstr(y, x, question, curses.color_pair(color.value))
 
 
 def clear_line(stdscr, y, x=0):
     """Clear a line from any text"""
     _, x_max = stdscr.getmaxyx()
-    stdscr.addstr(y, x, " " * (x_max - x - 2), curses.color_pair(Color.EMPTY.value))
+    stdscr.addstr(y, x, " " * (x_max - x - 1), curses.color_pair(Color.EMPTY.value))
 
 
 def input_string(stdscr, y, x, question, answer_length):
     """Ask user to input something and return it as a string"""
     curses.echo()
     curses.curs_set(True)
     display_question(stdscr, y, x, question, Color.PROMPTS)
```

### Comparing `calcure-2.8.6/calcure/errors.py` & `calcure-2.9/calcure/errors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/calcure/importers.py` & `calcure-2.9/calcure/importers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def read_file(self, filename):
         """Try to read a file and return its lines"""
         try:
             with open(filename, "r", encoding="utf-8") as file:
                 lines = file.readlines()
             return lines
         except (IOError, FileNotFoundError, NameError):
-            logging.error("Problem occured acessing %s.", filename)
+            logging.error("Problem occurred accessing %s.", filename)
             return []
 
     def import_tasks_from_calcurse(self):
         """Import tasks from calcurse database"""
         lines = self.read_file(self.calcurse_todo_file)
         for line in lines:
             name = line[4:-1]
```

### Comparing `calcure-2.8.6/calcure/loaders.py` & `calcure-2.9/calcure/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -273,15 +273,20 @@
             return ics_files
 
         # Otherwise, assume it's a folder, and read every file inside:
         for root, directories, files in os.walk(path):
             for filename in files:
                 # Get the full path to the file
                 file_path = os.path.join(root, filename)
-                ics_files.append(self.read_file(file_path))
+
+                # `path` may contain files with metadata, e.g. `color` and
+                # `displayname`. For now, exclude those while loading.
+                if file_path.endswith('.ics'):
+                    ics_files.append(self.read_file(file_path))
+
         return ics_files
 
 
 class TaskLoaderICS(LoaderICS):
     """Load tasks from ICS files"""
 
     def __init__(self, cf):
```

### Comparing `calcure-2.8.6/calcure/savers.py` & `calcure-2.9/calcure/savers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/calcure/screen.py` & `calcure-2.9/calcure/screen.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,28 @@
         self.stdscr = stdscr
         self.privacy = cf.PRIVACY_MODE
         self.state = cf.DEFAULT_VIEW
         self.calendar_state = CalState.DAILY if cf.DEFAULT_CALENDAR_VIEW == "daily" else CalState.MONTHLY
         self.use_persian_calendar = cf.USE_PERSIAN_CALENDAR
         self.split = cf.SPLIT_SCREEN
         self.right_pane_percentage = cf.RIGHT_PANE_PERCENTAGE
-        self.active_pane = False
+        self.currently_drawn = self.state
         self.selection_mode = False
-        self.refresh_now = False
+        self.refresh_now = True
         self.key = None
         self.day = self.today.day
         self.month = self.today.month
         self.year = self.today.year
 
     @property
+    def is_active_pane(self):
+        """Return True if currently drawn pane in the active one"""
+        return self.state == self.currently_drawn
+
+    @property
     def y_max(self):
         """Get maximum size of the screen"""
         y_max, _ = self.stdscr.getmaxyx()
         return y_max
 
     @property
     def journal_pane_width(self):
@@ -41,25 +46,25 @@
 
     @property
     def x_max(self):
         """Calculate the right boundary of the screen"""
         _, x_max = self.stdscr.getmaxyx()
         if x_max < 40:
             self.split = False
-        if self.split and self.state != AppState.JOURNAL:
+        if self.split and self.currently_drawn != AppState.JOURNAL:
             return x_max - self.journal_pane_width
         return x_max
 
     @property
     def x_min(self):
         """Calculate the left boundary of the screen"""
         _, x_max = self.stdscr.getmaxyx()
         if x_max < self.journal_pane_width:
             self.split = False
-        if self.split and self.state == AppState.JOURNAL:
+        if self.split and self.currently_drawn == AppState.JOURNAL:
             return x_max - self.journal_pane_width + 2
         return 0
 
     @property
     def date(self) -> datetime:
         """Return displayed date in datetime format"""
         if self.use_persian_calendar:
```

### Comparing `calcure-2.8.6/calcure/translations/br.py` & `calcure-2.9/calcure/translations/br.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,35 +18,36 @@
         "   q   ": "Sair",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "Adiciona um evento (recorrente)",
         "  n,🠒  ": "Próximo mês (dia)",
         "  p,🠐  ": "Mês (dia) anterior",
-        "  d,x  ": "Deletar um evento",
-        "  e,c  ": "Editar um evento",
-        "   m   ": "Mover evento",
+        "   x   ": "Deletar um evento",
+        "   r   ": "Editar um evento",
+        "  m(M) ": "Mover evento",
         "   v   ": "Alternar visualização diária/mensal",
-        "   g   ": "Ir para dia específico",
+        "  g(G) ": "Ir para dia específico",
         "   h   ": "Alternar evento como alta prioridade",
         "   l   ": "Alternar evento como baixa prioridade",
+        "   d   ": "Toggle event as done",
         "   .   ": "Alternar privacidade do evento",
         "   C   ": "Importar eventos do calcurse",
         "   G   ": "Retornar para o mês (dia) recorrente",
         }
 
 KEYS_TODO = {
         "  a(A) ": "Adicionar uma nova (sub)tarefa",
         "  h(H) ": "Alternar uma (todas) as tarefas como alta prioridade",
         "  l(L) ": "Alternar uma (todas) as tarefas como baixa prioridade",
-        "  v(V) ": "Alternar uma (todas) as tarefas como feitas",
+        "  d(D) ": "Alternar uma (todas) as tarefas como feitas",
         "  u(U) ": "Desmarcar uma (todas) as tarefas",
-        "  d(D) ": "Deletar uma (todas) as tarefas (com todas as subtarefas)",
+        "  x(X) ": "Deletar uma (todas) as tarefas (com todas as subtarefas)",
         "  t(T) ": "Começar/pausar temporizador para a tarefa",
-        "  e,c  ": "Editar uma tarefa",
+        "   r   ": "Editar uma tarefa",
         "   s   ": "Alternar entre tarefa e subtarefa",
         "   .   ": "Alternar privacidade da tarefa",
         "  f(F) ": "Mudar (remover) data limite da tarefa",
         "   m   ": "Mover tarefa",
         "  C(W) ": "Importar tarefas do calcurse (taskwarrior)",
         }
 
@@ -54,20 +55,22 @@
 MSG_VIM           = "Teclas Vim (j, k, ZZ, ZQ) também funcionam!"
 MSG_INFO          = "Para mais informações, visite:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "Realmente sair? (y/n) "
 
 MSG_EVENT_HIGH    = "Marca como alta prioridade evento número: "
 MSG_EVENT_LOW     = "Marca como baixa prioridade evento número: "
+MSG_EVENT_DONE    = "Mark as done event number: "
 MSG_EVENT_RESET   = "Reseta status para evento número:"
 MSG_EVENT_DEL     = "Deleta evento número: "
 MSG_EVENT_REN     = "Renomeia evento número: "
 MSG_NEW_TITLE     = "Digitar novo título: "
-MSG_EVENT_MOVE    = "Move evento número: "
-MSG_EVENT_MOVE_TO = "Mover evento para: "
+MSG_EVENT_MV      = "Move evento número: "
+MSG_EVENT_MV_TO   = "Mover evento para (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "Mover evento para: "
 MSG_EVENT_DATE    = "Digitar data: "
 MSG_EVENT_TITLE   = "Digitar título: "
 MSG_EVENT_REP     = "Repetir evento quantas vezes: "
 MSG_EVENT_FR      = "Repetir evento cada (d)ia, (w)semana, (m)ês ou (y)ano? "
 MSG_EVENT_IMP     = "Importar eventos do Calcurse? (y/n)"
 MSG_EVENT_PRIVACY = "Alternar privacidade do evento número: "
 MSG_TM_ADD        = "Adicionar/pausar temporizador para tarefa número: "
@@ -89,17 +92,19 @@
 MSG_TS_NOTHING    = "Nada planejado..."
 MSG_TS_PRIVACY    = "Alternar privacidade de tarefa número: "
 MSG_TS_DEAD_ADD   = "Adicionar data limite da tarefa número: "
 MSG_TS_DEAD_DEL   = "Remover data limite da tarefa número: "
 MSG_TS_DEAD_DATE  = "Adicionar data limite em (AAAA/MM/DD): "
 MSG_WEATHER       = "Clima está carregando..."
 MSG_ERRORS        = "Errors have occurred. See info.log file in your config folder."
+MSG_GOTO          = "Go to date (YYYY/MM/DD): "
+MSG_GOTO_D        = "Go to date: "
 
 CALENDAR_HINT     = "Espaço · Mudar para diário   a · Adicionar evento  n/p · Mudar mês   ? · Todas as combinações de teclas"
 CALENDAR_HINT_D   = "Espaço · Mudar para diário   a · Adicionar evento  n/p · Mudar dia   ? · Todas as combinações de teclas"
-JOURNAL_HINT      = "Espaço · Mudar para calendar   a · Adicionar tarefa   v · Feito   i · Importante   ? · Todas as combinações de teclas"
+JOURNAL_HINT      = "Espaço · Mudar para calendar   a · Adicionar tarefa   d · Feito   i · Importante   ? · Todas as combinações de teclas"
 
 DAYS = ["SEGUNDA", "TERÇA", "QUARTA", "QUINTA", "SEXTA", "SÁBADO", "DOMINGO"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
 
 MONTHS = ["JANEIRO", "FEVEREIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMBRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"]
 MONTHS_PERSIAN = ["FARVARDIN", "ORDIBEHESHT", "KHORDAD", "TIR", "MORDAD", "SHAHRIVAR", "MEHR", "ABAN", "AZAR", "DEY", "BAHMAN", "ESFAND"]
```

### Comparing `calcure-2.8.6/calcure/translations/en.py` & `calcure-2.9/calcure/translations/en.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,35 +18,36 @@
         "   q   ": "Quit",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "Add a (recurring) event",
         "  n,🠒  ": "Next month (day)",
         "  p,🠐  ": "Previous month (day)",
-        "  d,x  ": "Delete an event",
-        "  e,c  ": "Edit an event",
-        "   m   ": "Move event",
-        "   g   ": "Go to a certain day",
+        "   x   ": "Delete an event",
+        "   r   ": "Rename an event",
+        "  m(M) ": "Move event (in this month)",
+        "  g(G) ": "Go to a certain day (in this month)",
         "   v   ": "Toggle daily/monthly view",
         "   h   ": "Toggle event as high priority",
         "   l   ": "Toggle event as low priority",
+        "   d   ": "Toggle event as done",
         "   .   ": "Toggle event privacy",
         "   C   ": "Import events from calcurse",
-        "   G   ": "Return to current month (day)",
+        "   R   ": "Return to current month (day)",
         }
 
 KEYS_TODO = {
         "  a(A) ": "Add new (sub)task",
         "  h(H) ": "Toggle one (all) of the tasks as high priority",
         "  l(L) ": "Toggle one (all) of the tasks as low priority",
-        "  v(V) ": "Toggle one (all) of the tasks as done",
+        "  d(D) ": "Toggle one (all) of the tasks as done",
         "  u(U) ": "Unmark one (all) of the tasks",
-        "  d(D) ": "Delete one (all) of the tasks (with all subtasks)",
+        "  x(X) ": "Delete one (all) of the tasks (with all subtasks)",
         "  t(T) ": "Start/pause (remove) timer for a task",
-        "  e,c  ": "Edit a task",
+        "   r   ": "Rename a task",
         "   s   ": "Toggle between task and subtask",
         "   .   ": "Toggle task privacy",
         "  f(F) ": "Change (remove) task deadline",
         "   m   ": "Move a task",
         "  C(W) ": "Import tasks from calcurse (taskwarrior)",
         }
 
@@ -54,20 +55,22 @@
 MSG_VIM           = "Vim keys (j, k, ZZ, ZQ) work as well!"
 MSG_INFO          = "For more information, visit:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "Really exit? (y/n) "
 
 MSG_EVENT_HIGH    = "Mark as high priority event number: "
 MSG_EVENT_LOW     = "Mark as low priority event number: "
+MSG_EVENT_DONE    = "Mark as done event number: "
 MSG_EVENT_RESET   = "Reset status for event number: "
 MSG_EVENT_DEL     = "Delete event number: "
 MSG_EVENT_REN     = "Rename event number: "
 MSG_NEW_TITLE     = "Enter new title: "
-MSG_EVENT_MOVE    = "Move event number: "
-MSG_EVENT_MOVE_TO = "Move event to: "
+MSG_EVENT_MV      = "Move event number: "
+MSG_EVENT_MV_TO   = "Move event to (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "Move event to: "
 MSG_EVENT_DATE    = "Enter date: "
 MSG_EVENT_TITLE   = "Enter title: "
 MSG_EVENT_REP     = "How many times repeat the event: "
 MSG_EVENT_FR      = "Repeat the event every (d)ay, (w)eek, (m)onth or (y)ear? "
 MSG_EVENT_IMP     = "Import events from Calcurse? (y/n)"
 MSG_EVENT_PRIVACY = "Toggle privacy of event number: "
 MSG_TM_ADD        = "Add/pause timer for task number: "
@@ -89,17 +92,19 @@
 MSG_TS_NOTHING    = "Nothing planned..."
 MSG_TS_PRIVACY    = "Toggle privacy of task number: "
 MSG_TS_DEAD_ADD   = "Add deadline for task number: "
 MSG_TS_DEAD_DEL   = "Remove deadline of the task number: "
 MSG_TS_DEAD_DATE  = "Add deadline on (YYYY/MM/DD): "
 MSG_WEATHER       = "Weather is loading..."
 MSG_ERRORS        = "Errors have occurred. See info.log in your config folder."
+MSG_GOTO          = "Go to date (YYYY/MM/DD): "
+MSG_GOTO_D        = "Go to date: "
 
 CALENDAR_HINT     = "Space · Switch to journal   a · Add event  n/p · Change month   ? · All keybindings"
 CALENDAR_HINT_D   = "Space · Switch to journal   a · Add event  n/p · Change day   ? · All keybindings"
-JOURNAL_HINT      = "Space · Switch to calendar   a · Add task   v · Done   i · Important   ? · All keybindings"
+JOURNAL_HINT      = "Space · Switch to calendar   a · Add task   d · Done   i · Important   ? · All keybindings"
 
 DAYS = ["MONDAY", "TUESDAY", "WEDNESDAY", "THURSDAY", "FRIDAY", "SATURDAY", "SUNDAY"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
 
 MONTHS = ["JANUARY", "FEBRUARY", "MARCH", "APRIL", "MAY", "JUNE", "JULY", "AUGUST", "SEPTEMBER", "OCTOBER", "NOVEMBER", "DECEMBER"]
 MONTHS_PERSIAN = ["FARVARDIN", "ORDIBEHESHT", "KHORDAD", "TIR", "MORDAD", "SHAHRIVAR", "MEHR", "ABAN", "AZAR", "DEY", "BAHMAN", "ESFAND"]
```

### Comparing `calcure-2.8.6/calcure/translations/fr.py` & `calcure-2.9/calcure/translations/fr.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,88 +18,93 @@
         "   q   ": "Quitter",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "Ajouter un événement (récurrent)",
         "  n,🠒  ": "Le mois (jour) prochain",
         "  p,🠐  ": "mois (jour) précédent",
-        "  d,x  ": "Supprimer un événement",
-        "  e,c  ": "Modifier un événement",
-        "   m   ": "Déplacer l'événement",
+        "   x   ": "Supprimer un événement",
+        "   r   ": "Modifier un événement",
+        "  m(M) ": "Déplacer l'événement",
+        "  g(G) ": "Aller à un certain jour",
         "   v   ": "Basculer la vue quotidienne/mensuelle",
-        "   g   ": "Aller à un certain jour",
         "   h   ": "Désactiver l'événement en haute priorité",
         "   l   ": "Basculer l'événement en priorité basse",
+        "   d   ": "Toggle event as done",
         "   .   ": "Activer la confidentialité des événements",
         "   C   ": "Importer des événements depuis calcurse",
-        "   G   ": "Revenir au mois (jour) en cours",
+        "   R   ": "Revenir au mois (jour) en cours",
         }
 
 KEYS_TODO = {
         "  a(A) ": "Ajouter une nouvelle (sous-)tâche",
         "  h(H) ": "Bascule une (toutes) des tâches en haute priorité",
         "  l(L) ": "Désactiver une (toutes) les tâches en priorité basse",
-        "  v(V) ": "Bascule une (toutes) les tâches comme terminée",
+        "  d(D) ": "Bascule une (toutes) les tâches comme terminée",
         "  u(U) ": "Démarquer une (toutes) les tâches",
-        "  d(D) ": "Supprimer une (toutes) les tâches (avec toutes les sous-tâches)",
+        "  x(X) ": "Supprimer une (toutes) les tâches (avec toutes les sous-tâches)",
         "  t(T) ": "Démarrer/mettre en pause (supprimer) le minuteur pour une tâche",
-        "  e,c  ": "Modifier une tâche",
+        "   r   ": "Modifier une tâche",
         "   s   ": "Basculer entre tâche et sous-tâche",
         "   .   ": "Basculer la confidentialité des tâches",
         "  f(F) ": "Modifier (supprimer) l'échéance de la tâche",
         "   m   ": "Déplacer une tâche",
         "  C(W) ": "Importer des tâches de calcurse (taskwarrior)",
         }
 
 MSG_NAME          = "CALCURE"
 MSG_VIM           = "Les touches de Vim (j, k, ZZ, ZQ) fonctionnent également!"
 MSG_INFO          = "Pour plus d'informations, visitez:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "Vraiment quitter ? (y/n) "
 
-MSG_EVENT_HIGH    = "Marquer comme numéro d'événement hautement prioritaire: "
-MSG_EVENT_LOW     = "Marquer comme numéro d'événement basse priorité: "
+MSG_EVENT_HIGH    = "Marquer comme hautement prioritaire l'événement numéro: "
+MSG_EVENT_LOW     = "Marquer comme basse priorité l'événement numéro: "
+MSG_EVENT_DONE    = "Marquer comme terminé l'événement numéro: "
 MSG_EVENT_RESET   = "Réinitialiser le statut pour l'événement numéro : "
-MSG_EVENT_DEL     = "Supprimer le numéro d'événement: "
-MSG_EVENT_REN     = "Renommer le numéro d'événement: "
+MSG_EVENT_DEL     = "Supprimer l'événement numéro: "
+MSG_EVENT_REN     = "Renommer l'événement numéro: "
 MSG_NEW_TITLE     = "Entrez un nouveau titre: "
-MSG_EVENT_MOVE    = "Déplacer le numéro d'événement: "
-MSG_EVENT_MOVE_TO = "Déplacer l'événement vers: "
+MSG_EVENT_MV      = "Déplacer l'événement numéro: "
+MSG_EVENT_MV_TO   = "Déplacer l'événement vers (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "Déplacer l'événement vers: "
 MSG_EVENT_DATE    = "Entrez la date: "
 MSG_EVENT_TITLE   = "Entrez le titre: "
 MSG_EVENT_REP     = "Combien de répétitions de l'événement: "
 MSG_EVENT_FR      = "Répéter l'événement tous les jours (d), semaines (w), mois (m) ou années (y) ?"
 MSG_EVENT_IMP     = "Importer des événements depuis Calcurse ? (y/n)"
 MSG_EVENT_PRIVACY = "Basculer la confidentialité du numéro d'événement: "
 MSG_TM_ADD        = "Ajouter/mettre en pause le temporisateur pour la tâche numéro: "
 MSG_TM_RESET      = "Supprimer le temporisateur pour la tâche numéro: "
 MSG_TS_HIGH       = "Marquer comme haute priorité le numéro de tâche: "
 MSG_TS_LOW        = "Marquer comme basse priorité le numéro de tâche: "
 MSG_TS_RES        = "Réinitialiser l'état de la tâche numéro: "
 MSG_TS_DONE       = "Marquer comme terminé le numéro de tâche: "
 MSG_TS_DEL        = "Supprimer le numéro de tâche: "
 MSG_TS_DEL_ALL    = "Vraiment supprimer toutes les tâches ? (y/n)"
-MSG_TS_MOVE       = "Déplacer la tâche du numéro: "
+MSG_TS_MOVE       = "Déplacer la tâche numéro: "
 MSG_TS_MOVE_TO    = "Déplacer la tâche vers le numéro: "
-MSG_TS_EDIT       = "Modifier le numéro de tâche: "
+MSG_TS_EDIT       = "Modifier le numéro tâche: "
 MSG_TS_TOG        = "Basculer le numéro de sous-tâche: "
 MSG_TS_SUB        = "Ajouter une sous-tâche pour la tâche numéro: "
 MSG_TS_TITLE      = "Entrez la sous-tâche: "
 MSG_TS_IM         = "Importer des tâches depuis Calcurse ? (y/n)"
 MSG_TS_TW         = "Importer des tâches depuis Taskwarrior ? (y/n)"
 MSG_TS_NOTHING    = "Rien de prévu..."
 MSG_TS_PRIVACY    = "Basculer la confidentialité du numéro de tâche: "
-MSG_TS_DEAD_ADD   = "Ajouter un délai pour la tâche numéro: "
-MSG_TS_DEAD_DEL   = "Supprimer l'échéance de la tâche numéro: "
-MSG_TS_DEAD_DATE  = "Ajouter une date limite le (AAAA/MM/JJ): "
+MSG_TS_DEAD_ADD   = "Ajouter le deadline pour la tâche numéro: "
+MSG_TS_DEAD_DEL   = "Supprimer le deadline de la tâche numéro: "
+MSG_TS_DEAD_DATE  = "Ajouter le deadline (AAAA/MM/JJ): "
 MSG_WEATHER       = "La météo se charge..."
 MSG_ERRORS        = "Des erreurs se sont produites. Voir info.log dans votre dossier de configuration."
+MSG_GOTO          = "Aller au (YYYY/MM/DD): "
+MSG_GOTO_D        = "Aller au: "
 
 CALENDAR_HINT     = "Espace · Passer au journal  a · Ajouter un événement  n/p · Changer de mois  ? · Aider"
 CALENDAR_HINT_D   = "Espace · Passer au journal  a · Ajouter un événement  n/p · Changer de jour  ? · All keybindings"
-JOURNAL_HINT      = "Espace · Passer au calendrier  a · Ajouter une tâche  v · Terminé  i · Important  ? · All keybindings"
+JOURNAL_HINT      = "Espace · Passer au calendrier  a · Ajouter une tâche  d · Terminé  i · Important  ? · All keybindings"
 
 DAYS = ["LUNDI", "MARDI", "MERCREDI", "JEUDI", "VENDREDI", "SAMEDI", "DIMANCHE"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
 
 MONTHS = ["JANVIER", "FEVRIER", "MARS", "AVRIL", "MAI", "JUIN", "JUILLET", "AOUT", "SEPTEMBRE", "OCTOBRE", "NOVEMBRE", "DECEMBRE"]
 MONTHS_PERSIAN = ["FARVARDIN", "ORDIBEHESHT", "KHORDAD", "TIR", "MORDAD", "SHAHRIVAR", "MEHR", "ABAN", "AZAR", "DEY", "BAHMAN", "ESFAND"]
```

### Comparing `calcure-2.8.6/calcure/translations/it.py` & `calcure-2.9/calcure/translations/it.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,35 +18,36 @@
         "   q   ": "Esci",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "Aggiungi un evento (ricorrente)",
         "  n,🠒  ": "Mese successivo (giorno)",
         "  p,🠐  ": "Mese precedente (giorno)",
-        "  d,x  ": "Cancella un evento",
-        "  e,c  ": "Modifica un evento",
-        "   m   ": "Sposta un evento",
+        "   x   ": "Cancella un evento",
+        "   r   ": "Modifica un evento",
+        "  m(M) ": "Sposta un evento",
         "   v   ": "Alterna la visualizzazione giornaliera/mensile",
-        "   g   ": "Vai ad un determinato giorno",
+        "  g(G) ": "Vai ad un determinato giorno",
         "   h   ": "Imposta un evento come ad alta priorità",
         "   l   ": "Imposta un evento come a bassa priorità",
+        "   d   ": "Imposta un evento come fatto",
         "   .   ": "Imposta la privacy per un evento",
         "   C   ": "Importa eventi da calcurse",
-        "   G   ": "Ritorna al mese corrente (giorno)",
+        "   R   ": "Ritorna al mese corrente (giorno)",
         }
 
 KEYS_TODO = {
         "  a(A) ": "Aggiungi una nuova (sotto)attività",
         "  h(H) ": "Imposta una fra (o tutte) le attività come ad alta priorità",
         "  l(L) ": "Imposta una fra (o tutte) le attività come a bassa priorità",
-        "  v(V) ": "Imposta una fra (o tutte) le attività come completate",
+        "  d(D) ": "Imposta una fra (o tutte) le attività come completate",
         "  u(U) ": "Deseleziona una fra (o tutte) le attività",
-        "  d(D) ": "Cancella una fra (o tutte) le attività (con tutte le sue sottoattività)",
+        "  x(X) ": "Cancella una fra (o tutte) le attività (con tutte le sue sottoattività)",
         "  t(T) ": "Avvia/ferma (o cancella) il timer per una attività",
-        "  e,c  ": "Modifica una attività",
+        "   r   ": "Modifica una attività",
         "   s   ": "Passa da attività a sottoattività (e viceversa)",
         "   .   ": "Imposta la privacy dell'attività",
         "  f(F) ": "Cambia (o rimuovi) la scadenza per una attività",
         "   m   ": "Sposta una attività",
         "  C(W) ": "Importa le attività da calcurse (taskwarrior)",
         }
 
@@ -54,20 +55,22 @@
 MSG_VIM           = "È possibile usare i tasti di Vim (j, k, ZZ, ZQ)!"
 MSG_INFO          = "Per maggiori informazioni, visitare:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "Vuoi davvero uscire? (y/n) "
 
 MSG_EVENT_HIGH    = "Imposta ad alta priorità l'evento con numero: "
 MSG_EVENT_LOW     = "Imposta come a bassa priorità l'evento con numero: "
+MSG_EVENT_DONE    = "Mark as done event number: "
 MSG_EVENT_RESET   = "Ripristina lo stato per l'evento con numero: "
 MSG_EVENT_DEL     = "Cancella l'evento con numero: "
 MSG_EVENT_REN     = "Rinomina l'evento con numero: "
 MSG_NEW_TITLE     = "Inserisci il nuovo titolo: "
-MSG_EVENT_MOVE    = "Sposta l'evento con numero: "
-MSG_EVENT_MOVE_TO = "Postponi l'evento a: "
+MSG_EVENT_MV      = "Sposta l'evento con numero: "
+MSG_EVENT_MV_TO   = "Postponi l'evento a (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "Postponi l'evento a: "
 MSG_EVENT_DATE    = "Inserisci una data: "
 MSG_EVENT_TITLE   = "Inserisci un titolo: "
 MSG_EVENT_REP     = "Quante volte vuoi ripetere l'evento: "
 MSG_EVENT_FR      = "Ripetere l'evento ogni giorno(d), settimana(w), mese(m) o anno(y)? "
 MSG_EVENT_IMP     = "Vuoi importare un evento da Calcurse? (y/n)"
 MSG_EVENT_PRIVACY = "Attiva la privacy dell'evento con numero: "
 MSG_TM_ADD        = "Avvia/ferma il timer per l'attività con numero: "
@@ -89,17 +92,19 @@
 MSG_TS_NOTHING    = "Nulla di pianificato..."
 MSG_TS_PRIVACY    = "Attiva la privacy dell'attività con numero: "
 MSG_TS_DEAD_ADD   = "Aggiungi una scadenza per l'attività con numero: "
 MSG_TS_DEAD_DEL   = "Rimuovi la scadenza per l'attività con numero: "
 MSG_TS_DEAD_DATE  = "Aggiungi una scandeza per il (AAAA/MM/GG): "
 MSG_WEATHER       = "Caricamento del meteo..."
 MSG_ERRORS        = "Errors have occurred. See info.log file in your config folder."
+MSG_GOTO          = "Vai alla data (YYYY/MM/DD): "
+MSG_GOTO_D        = "Vai alla data: "
 
 CALENDAR_HINT     = "Barra spaziatrice · Passa al diario   a · Aggiungi un evento  n/p · Cambia mese   ? · Mostra tutte le scorciatoie"
 CALENDAR_HINT_D   = "Barra spaziatrice · Passa al diario   a · Aggiungi un evento  n/p · Cambia giorno  ? · Mostra tutte le scorciatoie"
-JOURNAL_HINT      = "Barra spaziatrice · Passa al calendario   a · Add task   v · Finito   i · Importante   ? · Mostra tutte le scorciatoie"
+JOURNAL_HINT      = "Barra spaziatrice · Passa al calendario   a · Add task   d · Finito   i · Importante   ? · Mostra tutte le scorciatoie"
 
 DAYS = ["LUNEDÌ", "MARTEDÌ", "MERCOLEDÌ", "GIOVEDÌ", "VENERDì", "SABATO", "DOMENICA"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
 
 MONTHS = ["GENNAIO", "FEBBRAIO", "MARZO", "APRILE", "MAGGIO", "GIUGNO", "LUGLIO", "AGOSTO", "SETTEMBRE", "OTTOBRE", "NOVEMBRE", "DICEMBRE"]
 MONTHS_PERSIAN = ["FARVARDIN", "ORDIBEHESHT", "KHORDAD", "TIR", "MORDAD", "SHAHRIVAR", "MEHR", "ABAN", "AZAR", "DEY", "BAHMAN", "ESFAND"]
```

### Comparing `calcure-2.8.6/calcure/translations/ru.py` & `calcure-2.9/calcure/translations/ru.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,36 @@
         "   q   ": "Выйти",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "Добавить (повторяющееся) событие",
         "  n,🠒  ": "Следующий месяц (день)",
         "  p,🠐  ": "Предыдущий месяц (день)",
-        "  d,x  ": "Удалить событие",
-        "  e,c  ": "Переименовать событие",
-        "   m   ": "Переместить событие",
+        "   x   ": "Удалить событие",
+        "   r   ": "Переименовать событие",
+        "  m(M) ": "Переместить событие",
         "   v   ": "Переключать дневной/месячный вид",
-        "   g   ": "Открыть определённый день",
+        "  g(G) ": "Открыть определённый день",
         "   h   ": "Переключать высокий приоритет",
         "   l   ": "Переключать низкий приоритет",
+        "   d   ": "Переключать статус завершено",
         "   .   ": "Переключать приватность события",
         "   C   ": "Импортировать события из calcurse",
-        "   G   ": "Вернуться к текущему месяцу (дню)",
+        "   R   ": "Вернуться к текущему месяцу (дню)",
         }
 
 KEYS_TODO = {
         "  a(A) ": "Добавить новую (под)задачу",
         "  h(H) ": "Переключать приоритет одной (всех) задач как высокий",
         "  l(L) ": "Переключать приоритет одной (всех) задач как низкий",
-        "  v(V) ": "Переключать приоритет одной (всех) задач как завершено",
+        "  d(D) ": "Переключать приоритет одной (всех) задач как завершено",
         "  u(U) ": "Убрать все метки с одной (всех) задач",
-        "  d(D) ": "Удалить одну (все) задачи (со всеми подзадачами)",
+        "  x(X) ": "Удалить одну (все) задачи (со всеми подзадачами)",
         "  t(T) ": "Запустить/приостановить (удалить) таймер задачи",
-        "  e,c  ": "Переименовать задачу",
+        "   r   ": "Переименовать задачу",
         "   s   ": "Переключать между задачей и подзадачей",
         "   .   ": "Переключать приватность задачи",
         "  f(F) ": "Изменить (удалить) дедлайн задачи",
         "   m   ": "Переместить задачу",
         "  C(W) ": "Импортировать задачи из calcurse (taskwarrior)",
         }
 
@@ -54,20 +55,22 @@
 MSG_VIM           = "Vim клавиши (j, k, ZZ, ZQ) работают!"
 MSG_INFO          = "Больше информации вы найдёте на:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "Действительно выйти? (y/n) "
 
 MSG_EVENT_HIGH    = "Отметить как высокоприоритетное событие номер: "
 MSG_EVENT_LOW     = "Отметить как низкоприоритетное событие номер: "
+MSG_EVENT_DONE    = "Отметить как завершенное событие номер: "
 MSG_EVENT_RESET   = "Обнулить статус событие номер: "
 MSG_EVENT_DEL     = "Удалить событие номер: "
 MSG_EVENT_REN     = "Переименовать событие номер: "
 MSG_NEW_TITLE     = "Введите новое название: "
-MSG_EVENT_MOVE    = "Переместить событие номер: "
-MSG_EVENT_MOVE_TO = "Переместить событие на: "
+MSG_EVENT_MV      = "Переместить событие номер: "
+MSG_EVENT_MV_TO   = "Переместить событие на (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "Переместить событие на: "
 MSG_EVENT_DATE    = "Введите дату: "
 MSG_EVENT_TITLE   = "Введите название: "
 MSG_EVENT_REP     = "Сколько раз повторить событие: "
 MSG_EVENT_FR      = "Повторить событие каждый день (d), неделю (w), месяц (m) или год(y)? "
 MSG_EVENT_IMP     = "Импортировать события из Calcurse? (y/n)"
 MSG_EVENT_PRIVACY = "Изменить приватность события номер: "
 MSG_TM_ADD        = "Запустить/приостановить таймер для задачи: "
@@ -89,17 +92,19 @@
 MSG_TS_NOTHING    = "Ничего не запланировано..."
 MSG_TS_PRIVACY    = "Переключать приватность задачи номер: "
 MSG_TS_DEAD_ADD   = "Добавить дедлайн к задаче номер: "
 MSG_TS_DEAD_DEL   = "Удалить дедлайн задачи номер: "
 MSG_TS_DEAD_DATE  = "Установить дедлайн на (YYYY/MM/DD): "
 MSG_WEATHER       = "Загружается информации о погоде..."
 MSG_ERRORS        = "Возникли ошибки. Детали в info.log файле в конфиг директории."
+MSG_GOTO          = "Перейти к дате (YYYY/MM/DD): "
+MSG_GOTO_D        = "Перейти к дате: "
 
 CALENDAR_HINT     = "Пробел · Переключить на журнал   a · Новое событие  n/p · Сменить месяц   ? · Клавиши"
 CALENDAR_HINT_D   = "Пробел · Переключить на журнал   a · Новое событие  n/p · Сменить день   ? · Клавиши"
-JOURNAL_HINT      = "Пробел · Переключить на календарь   a · Новая задача   v · Выполнено   h · Важно   ? · Клавиши"
+JOURNAL_HINT      = "Пробел · Переключить на календарь   a · Новая задача   d · Выполнено   h · Важно   ? · Клавиши"
 
 DAYS         = ["ПОНЕДЕЛЬНИК", "ВТОРНИК", "СРЕДА", "ЧЕТВЕРГ", "ПЯТНИЦА", "СУББОТА", "ВОСКРЕСЕНЬЕ"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
 
 MONTHS         = ["ЯНВАРЬ", "ФЕВРАЛЬ", "МАРТ", "АПРЕЛЬ", "МАЙ", "ИЮНЬ", "ИЮЛЬ", "АВГУСТ", "СЕНТЯБРЬ", "ОКТЯБРЬ", "НОЯБРЬ", "ДЕКАБРЬ"]
 MONTHS_PERSIAN = ["FARVARDIN", "ORDIBEHESHT", "KHORDAD", "TIR", "MORDAD", "SHAHRIVAR", "MEHR", "ABAN", "AZAR", "DEY", "BAHMAN", "ESFAND"]
```

### Comparing `calcure-2.8.6/calcure/translations/tr.py` & `calcure-2.9/calcure/translations/tr.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,34 @@
         "   q   ": "Çıkış",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "Etkinlik (yinelenen) ekleme",
         "  n,🠒  ": "Gelecek ay (gün)",
         "  p,🠐  ": "Önceki ay (gün)",
-        "  d,x  ": "Etkinlik silme",
-        "  e,c  ": "Etkinlik düzenleme",
-        "   m   ": "Etkinlik taşıma",
-        "   g   ": "Belirli bir güne git",
+        "   x   ": "Etkinlik silme",
+        "  e,r  ": "Etkinlik düzenleme",
+        "  m(M) ": "Etkinlik taşıma",
+        "  g(G) ": "Belirli bir güne git",
         "   v   ": "Günlük/aylık görünümü değiştir",
         "   h   ": "Etkinliği yüksek öncelikli olarak değiştir",
         "   l   ": "Etkinliği düşük öncelikli olarak değiştir",
+        "   d   ": "Toggle event as done",
         "   .   ": "Etkinlik gizliliğini aç / kapat",
         "   C   ": "Calcurse'den etkinlikleri içe aktarma",
-        "   G   ": "Geçerli aya (güne) dön",
+        "   R   ": "Geçerli aya (güne) dön",
         }
 
 KEYS_TODO = {
         "  a(A) ": "Yeni (alt) görev ekle",
         "  h(H) ": "Görevlerden birini (tümünü) yüksek öncelikli olarak değiştirin",
         "  l(L) ": "Görevlerden birini (tümünü) düşük öncelikli olarak değiştirin",
-        "  v(V) ": "Görevlerden birini (tümünü) yapıldı olarak değiştirin",
+        "  d(D) ": "Görevlerden birini (tümünü) yapıldı olarak değiştirin",
         "  u(U) ": "Görevlerden birinin (tümünün) işaretini kaldırın",
-        "  d(D) ": "Görevlerden birini (tümünü) silme (tüm alt görevlerle birlikte)",
+        "  x(X) ": "Görevlerden birini (tümünü) silme (tüm alt görevlerle birlikte)",
         "  t(T) ": "Bir görev için zamanlayıcıyı başlatma/duraklatma (kaldırma)",
         "  e,c  ": "Görev düzenleme",
         "   s   ": "Görev ve alt görev arasında geçiş yapma",
         "   .   ": "Görev gizliliğini aç / kapat",
         "  f(F) ": "Görev son tarihini değiştir (kaldır)",
         "   m   ": "Görev taşıma",
         "  C(W) ": "Calcurse'den görevleri içe aktarma (taskwarrior)",
@@ -54,20 +55,22 @@
 MSG_VIM           = "Vim tuşları (j, k, ZZ, ZQ) da çalışıyor!"
 MSG_INFO          = "Daha fazla bilgi için ziyaret edin:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "Gerçekten çıkıyorsun musun? (y/n) "
 
 MSG_EVENT_HIGH    = "Yüksek öncelikli olay numarası olarak işaretle: "
 MSG_EVENT_LOW     = "Düşük öncelikli olay numarası olarak işaretle: "
+MSG_EVENT_DONE    = "Mark as done event number: "
 MSG_EVENT_RESET   = "Etkinlik numarası için durumu sıfırla: "
 MSG_EVENT_DEL     = "Etkinlik numarasını sil: "
 MSG_EVENT_REN     = "Etkinlik numarasını yeniden adlandır: "
 MSG_NEW_TITLE     = "Yeni başlık girin: "
-MSG_EVENT_MOVE    = "Etkinlik numarasını taşı: "
-MSG_EVENT_MOVE_TO = "Etkinliği şuraya taşı: "
+MSG_EVENT_MV      = "Etkinlik numarasını taşı: "
+MSG_EVENT_MV_TO   = "Etkinliği şuraya taşı (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "Etkinliği şuraya taşı: "
 MSG_EVENT_DATE    = "Tarih girin: "
 MSG_EVENT_TITLE   = "Başlığı girin: "
 MSG_EVENT_REP     = "Etkinliğin kaç kez tekrarlanacağı: "
 MSG_EVENT_FR      = "Etkinliği her gün(d), hafta(w), ay(m) veya yıl(y) tekrarlayın? "
 MSG_EVENT_IMP     = "Calcurse'den etkinlikleri içe aktarma? (y/n)"
 MSG_EVENT_PRIVACY = "Etkinlik numarasının gizliliğini aç / kapat: "
 MSG_TM_ADD        = "Görev numarası için zamanlayıcı ekle/duraklat: "
@@ -89,17 +92,19 @@
 MSG_TS_NOTHING    = "Planlanmış bir şey yok..."
 MSG_TS_PRIVACY    = "Görev numarasının gizliliğini aç / kapat: "
 MSG_TS_DEAD_ADD   = "Görev numarası için son tarih ekle: "
 MSG_TS_DEAD_DEL   = "Görev numarasının son tarihini kaldırın: "
 MSG_TS_DEAD_DATE  = "Son tarih ekleyin (YYYY/MM/DD): "
 MSG_WEATHER       = "Hava durumu yükleniyor..."
 MSG_ERRORS        = "Errors have occurred. See info.log in your config folder."
+MSG_GOTO          = "Go to date (YYYY/MM/DD): "
+MSG_GOTO_G        = "Go to date: "
 
 CALENDAR_HINT     = "Space · Günlüğe geç   a · Etkinlik ekle  n/p · Ayı değiştir   ? · Tüm tuş atamaları"
 CALENDAR_HINT_D   = "Space · Günlüğe geç   a · Etkinlik ekle  n/p · Günü değiştir   ? · Tüm tuş atamaları"
-JOURNAL_HINT      = "Space · Takvime geç   a · Görev ekle   v · Tamamlandı   i · Önemli   ? · Tüm tuş atamaları"
+JOURNAL_HINT      = "Space · Takvime geç   a · Görev ekle   d · Tamamlandı   i · Önemli   ? · Tüm tuş atamaları"
 
 DAYS = ["PAZARTESİ", "SALI", "ÇARŞAMBA", "PERŞEMBE", "CUMA", "CUMARTESİ", "PAZAR"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
 
 MONTHS = ["OCAK", "ŞUBAT", "MART", "NİSAN", "MAYIS", "HAZİRAN", "TEMMUZ", "AĞUSTOS", "EYLÜL", "EKİM", "KASIM", "ARALIK"]
 MONTHS_PERSIAN = ["FARVARDIN", "ORDIBEHESHT", "KHORDAD", "TIR", "MORDAD", "SHAHRIVAR", "MEHR", "ABAN", "AZAR", "DEY", "BAHMAN", "ESFAND"]
```

### Comparing `calcure-2.8.6/calcure/translations/zh.py` & `calcure-2.9/calcure/translations/zh.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,35 +18,36 @@
         "   q   ": "退出",
         }
 
 KEYS_CALENDAR = {
         "  a(A) ": "增加一个（再次发生）事件",
         "  n,🠒  ": "下个月 (日)",
         "  p,🠐  ": "上个月 (日)",
-        "  d,x  ": "删除事件",
-        "  e,c  ": "编辑事件",
-        "   m   ": "移动事件",
-        "   g   ": "跳转到指定的一天",
+        "   x   ": "删除事件",
+        "   r   ": "编辑事件",
+        "  m(M) ": "移动事件",
+        "  g(G) ": "跳转到指定的一天",
         "   v   ": "切换每天/每月视图模式",
         "   h   ": "切换事件为更高的优先级",
         "   l   ": "切换事件为更低的优先级",
+        "   d   ": "Toggle event as done",
         "   .   ": "切换事件为隐私模式",
         "   C   ": "从calcurse中导入事件",
         "   G   ": "返回当前的月 (日)",
         }
 
 KEYS_TODO = {
         "  a(A) ": "新增一个 (子) 任务",
         "  h(H) ": "切换一个 (所有) 任务为更高优先级",
         "  l(L) ": "切换一个 (所有) 任务为更低优先级",
-        "  v(V) ": "切换一个 (所有) 任务为已完成",
+        "  d(D) ": "切换一个 (所有) 任务为已完成",
         "  u(U) ": "不标记一个 (所有) 任务",
-        "  d(D) ": "删除一个 (所有) 任务 (和其子任务)",
+        "  x(X) ": "删除一个 (所有) 任务 (和其子任务)",
         "  t(T) ": "开始/暂停 (移除) 时刻为一个任务",
-        "  e,c  ": "编辑一个任务",
+        "   r   ": "编辑一个任务",
         "   s   ": "切换任务和子任务",
         "   .   ": "切换任务为隐私模式",
         "  f(F) ": "修改 (移除) 任务的截止日期",
         "   m   ": "移动一个任务",
         "  C(W) ": "导入任务从calcurse (taskwarrior)",
         }
 
@@ -54,20 +55,22 @@
 MSG_VIM           = "Vim 键位 (j, k, ZZ, ZQ) 也可以工作!"
 MSG_INFO          = "对于更多信息, 参看:"
 MSG_SITE          = "https://anufrievroman.gitbook.io/calcure"
 MSG_EXIT          = "是否真的要退出? (y/n) "
 
 MSG_EVENT_HIGH    = "标记为更高优先级的事件号码: "
 MSG_EVENT_LOW     = "标记为更低优先级的事件号码: "
+MSG_EVENT_DONE    = "Mark as done event number: "
 MSG_EVENT_RESET   = "重设状态的事件号码: "
 MSG_EVENT_DEL     = "删除事件的号码: "
 MSG_EVENT_REN     = "重命名事件的号码: "
 MSG_NEW_TITLE     = "输入新的标题: "
-MSG_EVENT_MOVE    = "移动事件的号码: "
-MSG_EVENT_MOVE_TO = "移动事件到: "
+MSG_EVENT_MV      = "移动事件的号码: "
+MSG_EVENT_MV_TO   = "移动事件到 (YYYY/MM/DD): "
+MSG_EVENT_MV_TO_D = "移动事件到: "
 MSG_EVENT_DATE    = "输入日期: "
 MSG_EVENT_TITLE   = "输入标题: "
 MSG_EVENT_REP     = "事件重复多少次: "
 MSG_EVENT_FR      = "重复事件 (d)天, (w)周, (m)月 或者 (y)年? "
 MSG_EVENT_IMP     = "是否从Calcurse中导入事件? (y/n)"
 MSG_EVENT_PRIVACY = "切换为隐私模式的事件号码: "
 MSG_TM_ADD        = "增加/暂停计时器的任务号码: "
@@ -89,14 +92,15 @@
 MSG_TS_NOTHING    = "没有事情被计划..."
 MSG_TS_PRIVACY    = "切换为隐私模式的事件号码: "
 MSG_TS_DEAD_ADD   = "增加截至日期为事件号码: "
 MSG_TS_DEAD_DEL   = "移除截止日期为事件号码: "
 MSG_TS_DEAD_DATE  = "增加截至日期在(YYYY/MM/DD): "
 MSG_WEATHER       = "天气插件正在加载..."
 MSG_ERRORS        = "Errors have occurred. See info.log in your config folder."
+MSG_GOTO          = "Go to date (YYYY/MM/DD): "
 
 CALENDAR_HINT     = "Space · 转换到通知栏   a · 增加事件  n/p · 改变月   ? · 所有键位绑定"
 CALENDAR_HINT_D   = "Space · 转换到通知栏   a · 增加事件  n/p · 改变日   ? · 所有键位绑定"
 JOURNAL_HINT      = "Space · 转换到日历栏   a · 增加任务   v · 已完成   i · 重要的   ? · 所有键位绑定"
 
 DAYS = ["周一", "周二", "周三", "周四", "周五", "周六", "周日"]
 DAYS_PERSIAN = ["SHANBEH", "YEKSHANBEH", "DOSHANBEH", "SESHANBEH", "CHAHARSHANBEH", "PANJSHANBEH", "JOMEH"]
```

### Comparing `calcure-2.8.6/calcure/weather.py` & `calcure-2.9/calcure/weather.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.6/calcure.egg-info/PKG-INFO` & `calcure-2.9/calcure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.8.6
+Version: 2.9
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.8.6/calcure.egg-info/SOURCES.txt` & `calcure-2.9/calcure.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 calcure/data.py
 calcure/dialogues.py
 calcure/errors.py
 calcure/importers.py
 calcure/loaders.py
 calcure/savers.py
 calcure/screen.py
-calcure/test_async.py
-calcure/test_decoration.py
 calcure/weather.py
 calcure.egg-info/PKG-INFO
 calcure.egg-info/SOURCES.txt
 calcure.egg-info/dependency_links.txt
 calcure.egg-info/entry_points.txt
 calcure.egg-info/requires.txt
 calcure.egg-info/top_level.txt
```

### Comparing `calcure-2.8.6/setup.py` & `calcure-2.9/setup.py`

 * *Files identical despite different names*

