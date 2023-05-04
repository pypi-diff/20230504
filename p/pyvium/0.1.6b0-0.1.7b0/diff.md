# Comparing `tmp/pyvium-0.1.6b0.tar.gz` & `tmp/pyvium-0.1.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvium-0.1.6b0.tar", max compression
+gzip compressed data, was "pyvium-0.1.7b0.tar", max compression
```

## Comparing `pyvium-0.1.6b0.tar` & `pyvium-0.1.7b0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      618 2023-02-13 12:29:09.992636 pyvium-0.1.6b0/LICENSE
--rw-r--r--   0        0        0     1415 2023-05-04 18:58:12.012857 pyvium-0.1.6b0/pyproject.toml
--rw-r--r--   0        0        0       52 2023-05-03 22:44:37.236878 pyvium-0.1.6b0/pyvium/__init__.py
--rw-r--r--   0        0        0      306 2023-05-04 18:47:48.314812 pyvium-0.1.6b0/pyvium/core/__init__.py
--rw-r--r--   0        0        0      621 2023-05-04 18:47:48.315796 pyvium-0.1.6b0/pyvium/core/base.py
--rw-r--r--   0        0        0    10491 2023-05-04 18:47:48.316793 pyvium-0.1.6b0/pyvium/core/direct_mode_functions.py
--rw-r--r--   0        0        0     4468 2023-05-04 18:47:48.317810 pyvium-0.1.6b0/pyvium/core/generic_functions.py
--rw-r--r--   0        0        0     5673 2023-05-04 18:47:48.318806 pyvium-0.1.6b0/pyvium/core/method_mode_functions.py
--rw-r--r--   0        0        0     2483 2023-05-04 18:47:48.319800 pyvium-0.1.6b0/pyvium/core/we32_functions.py
--rw-r--r--   0        0        0      325 2023-02-13 12:29:10.046638 pyvium-0.1.6b0/pyvium/errors/__init__.py
--rw-r--r--   0        0        0      197 2023-02-13 12:29:10.047636 pyvium-0.1.6b0/pyvium/errors/cell_off.py
--rw-r--r--   0        0        0      317 2023-02-13 12:29:10.047636 pyvium-0.1.6b0/pyvium/errors/device_busy.py
--rw-r--r--   0        0        0      298 2023-02-13 12:29:10.047636 pyvium-0.1.6b0/pyvium/errors/device_not_connected_to_iviumsoft.py
--rw-r--r--   0        0        0      272 2023-02-13 12:29:10.048636 pyvium-0.1.6b0/pyvium/errors/driver_not_open.py
--rw-r--r--   0        0        0      289 2023-02-13 12:29:10.048636 pyvium-0.1.6b0/pyvium/errors/no_device_detected.py
--rw-r--r--   0        0        0      269 2023-02-13 12:29:10.048636 pyvium-0.1.6b0/pyvium/errors/no_iviumsoft_running.py
--rw-r--r--   0        0        0  5131844 2023-02-13 12:29:10.031671 pyvium-0.1.6b0/pyvium/IVIUM_remdriver.dll
--rw-r--r--   0        0        0  2187264 2023-02-13 12:29:10.045638 pyvium-0.1.6b0/pyvium/Ivium_remdriver64.dll
--rw-r--r--   0        0        0      250 2023-05-04 18:57:45.028858 pyvium-0.1.6b0/pyvium/pyvium/__init__.py
--rw-r--r--   0        0        0     9022 2023-05-04 18:55:01.107663 pyvium-0.1.6b0/pyvium/pyvium/direct_mode_functions.py
--rw-r--r--   0        0        0     5755 2023-05-04 18:55:22.266023 pyvium-0.1.6b0/pyvium/pyvium/generic_functions.py
--rw-r--r--   0        0        0     4324 2023-05-04 18:53:24.176949 pyvium-0.1.6b0/pyvium/pyvium/method_mode_functions.py
--rw-r--r--   0        0        0     1941 2023-02-13 12:29:10.049636 pyvium-0.1.6b0/pyvium/pyvium_verifiers.py
--rw-r--r--   0        0        0       52 2023-02-13 12:29:10.049636 pyvium-0.1.6b0/pyvium/util/__init__.py
--rw-r--r--   0        0        0      477 2023-02-13 12:29:10.050636 pyvium-0.1.6b0/pyvium/util/get_ivium_dll_path.py
--rw-r--r--   0        0        0     1620 2023-02-13 12:29:09.992636 pyvium-0.1.6b0/README.md
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyvium-0.1.6b0/setup.py
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pyvium-0.1.6b0/PKG-INFO
+-rw-r--r--   0        0        0      618 2023-02-13 12:29:09.992636 pyvium-0.1.7b0/LICENSE
+-rw-r--r--   0        0        0     1415 2023-05-04 19:53:56.634675 pyvium-0.1.7b0/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-05-03 22:44:37.236878 pyvium-0.1.7b0/pyvium/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-04 18:47:48.314812 pyvium-0.1.7b0/pyvium/core/__init__.py
+-rw-r--r--   0        0        0      143 2023-05-04 19:24:19.702820 pyvium-0.1.7b0/pyvium/core/constants.py
+-rw-r--r--   0        0        0     1087 2023-05-04 19:24:39.155834 pyvium-0.1.7b0/pyvium/core/core_base.py
+-rw-r--r--   0        0        0    10741 2023-05-04 19:32:48.053240 pyvium-0.1.7b0/pyvium/core/direct_mode_functions.py
+-rw-r--r--   0        0        0     4551 2023-05-04 19:34:42.515380 pyvium-0.1.7b0/pyvium/core/generic_functions.py
+-rw-r--r--   0        0        0     5745 2023-05-04 19:23:09.727741 pyvium-0.1.7b0/pyvium/core/method_mode_functions.py
+-rw-r--r--   0        0        0     2539 2023-05-04 19:23:11.379740 pyvium-0.1.7b0/pyvium/core/we32_functions.py
+-rw-r--r--   0        0        0      325 2023-02-13 12:29:10.046638 pyvium-0.1.7b0/pyvium/errors/__init__.py
+-rw-r--r--   0        0        0      197 2023-02-13 12:29:10.047636 pyvium-0.1.7b0/pyvium/errors/cell_off.py
+-rw-r--r--   0        0        0      317 2023-02-13 12:29:10.047636 pyvium-0.1.7b0/pyvium/errors/device_busy.py
+-rw-r--r--   0        0        0      298 2023-02-13 12:29:10.047636 pyvium-0.1.7b0/pyvium/errors/device_not_connected_to_iviumsoft.py
+-rw-r--r--   0        0        0      272 2023-02-13 12:29:10.048636 pyvium-0.1.7b0/pyvium/errors/driver_not_open.py
+-rw-r--r--   0        0        0      289 2023-02-13 12:29:10.048636 pyvium-0.1.7b0/pyvium/errors/no_device_detected.py
+-rw-r--r--   0        0        0      269 2023-02-13 12:29:10.048636 pyvium-0.1.7b0/pyvium/errors/no_iviumsoft_running.py
+-rw-r--r--   0        0        0  5131844 2023-02-13 12:29:10.031671 pyvium-0.1.7b0/pyvium/IVIUM_remdriver.dll
+-rw-r--r--   0        0        0  2187264 2023-02-13 12:29:10.045638 pyvium-0.1.7b0/pyvium/Ivium_remdriver64.dll
+-rw-r--r--   0        0        0      250 2023-05-04 18:57:45.028858 pyvium-0.1.7b0/pyvium/pyvium/__init__.py
+-rw-r--r--   0        0        0     9022 2023-05-04 18:55:01.107663 pyvium-0.1.7b0/pyvium/pyvium/direct_mode_functions.py
+-rw-r--r--   0        0        0     5755 2023-05-04 18:55:22.266023 pyvium-0.1.7b0/pyvium/pyvium/generic_functions.py
+-rw-r--r--   0        0        0     4324 2023-05-04 19:52:25.297439 pyvium-0.1.7b0/pyvium/pyvium/method_mode_functions.py
+-rw-r--r--   0        0        0     1941 2023-02-13 12:29:10.049636 pyvium-0.1.7b0/pyvium/pyvium_verifiers.py
+-rw-r--r--   0        0        0       52 2023-02-13 12:29:10.049636 pyvium-0.1.7b0/pyvium/util/__init__.py
+-rw-r--r--   0        0        0      477 2023-02-13 12:29:10.050636 pyvium-0.1.7b0/pyvium/util/get_ivium_dll_path.py
+-rw-r--r--   0        0        0     1620 2023-02-13 12:29:09.992636 pyvium-0.1.7b0/README.md
+-rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyvium-0.1.7b0/setup.py
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pyvium-0.1.7b0/PKG-INFO
```

### Comparing `pyvium-0.1.6b0/LICENSE` & `pyvium-0.1.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/pyproject.toml` & `pyvium-0.1.7b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 homepage = "https://github.com/SF-Tec/pyvium"
 keywords = ["ivium", "iviumsoft", "ivium software", "ivium compactstat"]
 repository = "https://github.com/SF-Tec/pyvium"
 license = "Apache-2.0"
 name = "pyvium"
 packages = [{ include = "pyvium" }]
 readme = "README.md"
-version = "0.1.6beta"
+version = "0.1.7beta"
 classifiers = [
     # How mature is this project? Common values are
     #   3 - Alpha
     #   4 - Beta
     #   5 - Production/Stable
     'Development Status :: 4 - Beta',
```

### Comparing `pyvium-0.1.6b0/pyvium/core/direct_mode_functions.py` & `pyvium-0.1.7b0/pyvium/core/direct_mode_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .base import DOUBLE_PTR, LONG_PTR, Base, ffi
+from .constants import DOUBLE_PTR, LONG_PTR
+from .core_base import CoreBase, ffi
 
 ffi.cdef("""
     long __stdcall IV_getcellstatus(long *devcellstatus);
     long __stdcall IV_setconnectionmode(long *value);
     long __stdcall IV_setcellon(long *cellon);
     long __stdcall IV_setpotential(double *value);
     long __stdcall IV_setpotentialWE2(double *value);
@@ -24,200 +25,202 @@
     long __stdcall IV_setamplitude(double *value);
     long __stdcall IV_getcurrenttrace(long* npoints, double *rate, double *values);
     long __stdcall IV_getcurrentWE2trace(long* npoints, double *rate, double *values);
     long __stdcall IV_getpotentialtrace(long* npoints, double *rate, double *values);
 """)
 
 
-class DirectModeFunctions(Base):
-
+class DirectModeFunctions(CoreBase):
+    """
+    DirectModeFunctions class provides access to the direct mode functions of the IviumSoft library.
+    """
     @staticmethod
     def IV_getcellstatus() -> tuple[int, int]:
         '''Returns cell status labels
             ["I_ovl", "Anin1_ovl","E_ovl", "CellOff_button pressed", "Cell on"]'''
         cell_status_ptr = ffi.new(LONG_PTR)
-        result_code = Base.get_lib().IV_getcellstatus(cell_status_ptr)
+        result_code = CoreBase.get_lib().IV_getcellstatus(cell_status_ptr)
         return result_code, cell_status_ptr[0]
 
     @staticmethod
     def IV_setconnectionmode(connection_mode_number: int) -> int:
         ''' Select the connection mode for the currently connected device.
             The available modes depend on the connected device.
             These are all the supported connection modes: 0=off; 1=EStat4EL(default), 2=EStat2EL,
             3=EstatDummy1,4=EStatDummy2,5=EstatDummy3,6=EstatDummy4
             7=Istat4EL, 8=Istat2EL, 9=IstatDummy, 10=BiStat4EL, 11=BiStat2EL'''
         connection_mode_number_ptr = ffi.new(LONG_PTR, connection_mode_number)
-        result_code = Base.get_lib().IV_setconnectionmode(
+        result_code = CoreBase.get_lib().IV_setconnectionmode(
             connection_mode_number_ptr)
         return result_code
 
     @staticmethod
     def IV_setcellon(cell_on_mode_number: int) -> int:
         '''Set cell on off to close cell relais (0=off;1=on)'''
         cell_on_mode_number_ptr = ffi.new(LONG_PTR, cell_on_mode_number)
-        result_code = Base.get_lib().IV_setcellon(
+        result_code = CoreBase.get_lib().IV_setcellon(
             cell_on_mode_number_ptr)
         return result_code
 
     @staticmethod
     def IV_setpotential(potential_value: float) -> int:
         '''Set cell potential'''
         potential_value_ptr = ffi.new(DOUBLE_PTR, potential_value)
-        result_code = Base.get_lib().IV_setpotential(potential_value_ptr)
+        result_code = CoreBase.get_lib().IV_setpotential(potential_value_ptr)
         return result_code
 
     @staticmethod
     def IV_setpotentialWE2(potential_we2_value: float) -> int:
         '''Set BiStat offset potential'''
         potential_we2_value_ptr = ffi.new(DOUBLE_PTR, potential_we2_value)
-        result_code = Base.get_lib().IV_setpotentialWE2(potential_we2_value_ptr)
+        result_code = CoreBase.get_lib().IV_setpotentialWE2(potential_we2_value_ptr)
         return result_code
 
     @staticmethod
     def IV_setcurrent(current_value: float) -> int:
         '''Set cell current (galvanostatic mode)'''
         current_value_ptr = ffi.new(DOUBLE_PTR, current_value)
-        result_code = Base.get_lib().IV_setpotentialWE2(current_value_ptr)
+        result_code = CoreBase.get_lib().IV_setpotentialWE2(current_value_ptr)
         return result_code
 
     @staticmethod
     def IV_getpotential() -> tuple[int, float]:
         '''Returns measured potential'''
         potential_value_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getpotential(potential_value_ptr)
+        result_code = CoreBase.get_lib().IV_getpotential(potential_value_ptr)
         return result_code, potential_value_ptr[0]
 
     @staticmethod
     def IV_setcurrentrange(current_range_number: int) -> int:
         '''Set current range, 0=10A, 1=1A, etc,'''
         current_range_number_ptr = ffi.new(LONG_PTR, current_range_number)
-        result_code = Base.get_lib().IV_setcurrentrange(current_range_number_ptr)
+        result_code = CoreBase.get_lib().IV_setcurrentrange(current_range_number_ptr)
         return result_code
 
     @staticmethod
     def IV_setcurrentrangeWE2(current_range_number: int) -> int:
         '''Set current range for BiStat, 0=10mA, 1=1mA, etc,'''
         current_range_number_ptr = ffi.new(LONG_PTR, current_range_number)
-        result_code = Base.get_lib().IV_setcurrentrangeWE2(
+        result_code = CoreBase.get_lib().IV_setcurrentrangeWE2(
             current_range_number_ptr)
         return result_code
 
     @staticmethod
     def IV_getcurrent() -> tuple[int, float]:
         '''Returns measured current'''
         current_value_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getcurrent(current_value_ptr)
+        result_code = CoreBase.get_lib().IV_getcurrent(current_value_ptr)
         return result_code, current_value_ptr[0]
 
     @staticmethod
     def IV_getcurrentWE2() -> tuple[int, float]:
         '''Returns measured current from WE2 (bipotentiostat)'''
         current_value_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getcurrentWE2(current_value_ptr)
+        result_code = CoreBase.get_lib().IV_getcurrentWE2(current_value_ptr)
         return result_code, current_value_ptr[0]
 
     @staticmethod
     def IV_setfilter(filter_number: int) -> int:
         '''Set filter, for int :0=1MHz, 1=100kHz, 2=10kHz, 3=1kHz, 4=10Hz'''
         filter_number_ptr = ffi.new(LONG_PTR, filter_number)
-        result_code = Base.get_lib().IV_setfilter(filter_number_ptr)
+        result_code = CoreBase.get_lib().IV_setfilter(filter_number_ptr)
         return result_code
 
     @staticmethod
     def IV_setstability(stability_number: int) -> int:
         '''Set stability, for int 0=HighSpeed, 1=Standard, 2=HighStability'''
         stability_number_ptr = ffi.new(LONG_PTR, stability_number)
-        result_code = Base.get_lib().IV_setstability(stability_number_ptr)
+        result_code = CoreBase.get_lib().IV_setstability(stability_number_ptr)
         return result_code
 
     @staticmethod
     def IV_setbistatmode(value: int) -> int:
         '''REVISE! --> IV_bistat_mode(int) in documentation
             Select mode for BiStat, for int 0=standard, 1=scanning
             This bistat_mode function also can be used to control the Automatic E-ranging function of the instrument;
             0=AutoEranging off; 1=AutoEranging on'''
         value_ptr = ffi.new(LONG_PTR, value)
-        result_code = Base.get_lib().IV_setbistatmode(value_ptr)
+        result_code = CoreBase.get_lib().IV_setbistatmode(value_ptr)
         return result_code
 
     @staticmethod
     def IV_setdac(channel_number: int, value: float) -> int:
         '''Set dac on external port, int=0 for dac1, int=1 for dac2'''
         channel_number_ptr = ffi.new(LONG_PTR, channel_number)
         value_ptr = ffi.new(DOUBLE_PTR, value)
-        result_code = Base.get_lib().IV_setdac(channel_number_ptr, value_ptr)
+        result_code = CoreBase.get_lib().IV_setdac(channel_number_ptr, value_ptr)
         return result_code
 
     @staticmethod
     def IV_getadc(channel_number: int) -> tuple[int, float]:
         '''REVISE! Returns measured voltage on external ADC port, int=channelnr. 0-7'''
         channel_number_ptr = ffi.new(LONG_PTR, channel_number)
         measured_voltage_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getadc(
+        result_code = CoreBase.get_lib().IV_getadc(
             channel_number_ptr, measured_voltage_ptr)
         return result_code, measured_voltage_ptr[0]
 
     @staticmethod
     def IV_setmuxchannel(channel_number=0) -> int:
         '''Set channel of multiplexer, int=channelnr. starting from 0(default)'''
         channel_number_ptr = ffi.new(LONG_PTR, channel_number)
-        result_code = Base.get_lib().IV_setmuxchannel(channel_number_ptr)
+        result_code = CoreBase.get_lib().IV_setmuxchannel(channel_number_ptr)
         return result_code
 
     @staticmethod
     def IV_setdigout(value: int) -> int:
         '''REVISE! Set digital lines on external port, int is bitmask'''
         value_ptr = ffi.new(LONG_PTR, value)
-        result_code = Base.get_lib().IV_setdigout(value_ptr)
+        result_code = CoreBase.get_lib().IV_setdigout(value_ptr)
         return result_code
 
     @staticmethod
     def IV_getdigin() -> tuple[int, int]:
         '''REVISE! Returns status of digital inputs from external port, int is bitmask'''
         value_ptr = ffi.new(LONG_PTR)
-        result_code = Base.get_lib().IV_getdigin(value_ptr)
+        result_code = CoreBase.get_lib().IV_getdigin(value_ptr)
         return result_code, value_ptr[0]
 
     @staticmethod
     def IV_setfrequency(frequency: float) -> int:
         frequency_ptr = ffi.new(DOUBLE_PTR, frequency)
-        result_code: int = Base.get_lib().IV_setfrequency(frequency_ptr)
+        result_code: int = CoreBase.get_lib().IV_setfrequency(frequency_ptr)
         return result_code
 
     @staticmethod
     def IV_setamplitude(amplitude: float) -> int:
         amplitude_ptr = ffi.new(DOUBLE_PTR, amplitude)
-        result_code: int = Base.get_lib().IV_setamplitude(amplitude_ptr)
+        result_code: int = CoreBase.get_lib().IV_setamplitude(amplitude_ptr)
         return result_code
 
     @staticmethod
     def IV_getcurrenttrace(points_quantity: int, interval_rate: float) -> tuple[int, float]:
         '''Returns a sequence of measured currents at defined samplingrate
             (npoints, interval, array of double): npoints<=256, interval: 10us to 20ms'''
         points_quantity_ptr = ffi.new(LONG_PTR, points_quantity)
         interval_rate_ptr = ffi.new(DOUBLE_PTR, interval_rate)
         result_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getcurrenttrace(
+        result_code = CoreBase.get_lib().IV_getcurrenttrace(
             points_quantity_ptr, interval_rate_ptr, result_ptr)
         return result_code, result_ptr[0]
 
     @staticmethod
     def IV_getcurrentWE2trace(points_quantity: int, interval_rate: float) -> tuple[int, float]:
         '''Returns a sequence of measured WE2 currents at defined samplingrate
             (npoints, interval, array of double): npoints<=256, interval: 10us to 20ms'''
         points_quantity_ptr = ffi.new(LONG_PTR, points_quantity)
         interval_rate_ptr = ffi.new(DOUBLE_PTR, interval_rate)
         result_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getcurrentWE2trace(
+        result_code = CoreBase.get_lib().IV_getcurrentWE2trace(
             points_quantity_ptr, interval_rate_ptr, result_ptr)
         return result_code, result_ptr[0]
 
     @staticmethod
     def IV_getpotentialtrace(points_quantity: int, interval_rate: float) -> tuple[int, float]:
         '''Returns a sequence of measured potentials at defined samplingrate
             (npoints, interval, array of double): npoints<=256, interval: 10us to 20ms'''
         points_quantity_ptr = ffi.new(LONG_PTR, points_quantity)
         interval_rate_ptr = ffi.new(DOUBLE_PTR, interval_rate)
         result_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getpotentialtrace(
+        result_code = CoreBase.get_lib().IV_getpotentialtrace(
             points_quantity_ptr, interval_rate_ptr, result_ptr)
         return result_code, result_ptr[0]
```

### Comparing `pyvium-0.1.6b0/pyvium/core/generic_functions.py` & `pyvium-0.1.7b0/pyvium/core/generic_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .base import CHAR_ARRAY, LONG_PTR, UTF_ENCODING, Base, ffi
+from .constants import CHAR_ARRAY, LONG_PTR, UTF_ENCODING
+from .core_base import CoreBase, ffi
 
 ffi.cdef("""
     long __stdcall IV_open();
     long __stdcall IV_close();
     long __stdcall IV_MaxDevices();
     long __stdcall IV_selectdevice(long *devnr);
     long __stdcall IV_getdevicestatus();
@@ -14,94 +15,96 @@
     long __stdcall IV_HostHandle();
     long __stdcall IV_VersionDllFile();
     long __stdcall IV_VersionDllFileStr();
     long __stdcall IV_SelectChannel(long *channel);
 """)
 
 
-class GenericFunctions(Base):
+class GenericFunctions(CoreBase):
     @staticmethod
     def IV_open() -> int:
         '''Open the driver to manipulate the Ivium software'''
-        Base.set_driver_open(True)
-        return Base.get_lib().IV_open()
+        CoreBase.set_driver_open(True)
+        return CoreBase.get_lib().IV_open()
 
     @staticmethod
     def IV_close() -> int:
         '''Closes the iviumSoft driver'''
-        Base.set_driver_open(False)
-        return Base.get_lib().IV_close()
+        CoreBase.set_driver_open(False)
+        return CoreBase.get_lib().IV_close()
 
     @staticmethod
     def IV_MaxDevices() -> int:
         '''Returns the maximum number of devices that can be managed by IviumSoft'''
-        return Base.get_lib().IV_MaxDevices()
+        return CoreBase.get_lib().IV_MaxDevices()
 
     @staticmethod
     def IV_selectdevice(iviumsoft_instance_number: int = 1) -> tuple[int, int]:
         '''It allows to select one instance of the currently running IviumSoft instances'''
         instance_number_ptr = ffi.new(LONG_PTR, iviumsoft_instance_number)
-        result_code = Base.get_lib().IV_selectdevice(instance_number_ptr)
+        result_code = CoreBase.get_lib().IV_selectdevice(instance_number_ptr)
         return result_code, instance_number_ptr[0]
 
     @staticmethod
     def IV_getdevicestatus() -> int:
         '''It returns -1 (no IviumSoft), 0 (not connected), 1 (available_idle), 2 (available_busy),
             3 (no device available)'''
-        return Base.get_lib().IV_getdevicestatus()
+        return CoreBase.get_lib().IV_getdevicestatus()
 
     @staticmethod
     def IV_readSN() -> tuple[int, str]:
         '''Returns the serial number of the currently selected device'''
         device_serial_number_ptr = ffi.new(CHAR_ARRAY, 16)
-        result_code = Base.get_lib().IV_readSN(device_serial_number_ptr)
+        result_code = CoreBase.get_lib().IV_readSN(device_serial_number_ptr)
         return result_code, ffi.string(device_serial_number_ptr).decode(UTF_ENCODING)
 
     @staticmethod
     def IV_connect(connection_status: int) -> tuple[int, int]:
         '''It connects the currently selected device'''
         connection_status_ptr = ffi.new(LONG_PTR, connection_status)
-        result_code = Base.get_lib().IV_connect(connection_status_ptr)
+        result_code = CoreBase.get_lib().IV_connect(connection_status_ptr)
         return result_code, connection_status_ptr[0]
 
     @staticmethod
     def IV_VersionHost(version_host: int) -> tuple[int, int]:
         '''REVISE!!! Returns the version Host'''
         version_host_ptr = ffi.new(LONG_PTR, version_host)
-        result_code = Base.get_lib().IV_VersionHost(version_host_ptr)
+        result_code = CoreBase.get_lib().IV_VersionHost(version_host_ptr)
         return result_code, version_host_ptr[0]
 
     @staticmethod
     def IV_VersionDll() -> int:
         '''Returns the version of the IviumSoft dll'''
-        return Base.get_lib().IV_VersionDll()
+        return CoreBase.get_lib().IV_VersionDll()
 
     @staticmethod
     def IV_VersionCheck() -> int:
         '''It returns 1 if the selected instance of IviumSoft is running'''
-        return Base.get_lib().IV_VersionCheck()
+        return CoreBase.get_lib().IV_VersionCheck()
 
     @staticmethod
     def IV_HostHandle() -> int:
         '''REVISE!!! Returns Host Handle'''
-        return Base.get_lib().IV_HostHandle()
+        return CoreBase.get_lib().IV_HostHandle()
 
     @staticmethod
     def IV_VersionDllFile() -> int:
         '''REVISE!!! Returns DLL file version'''
-        return Base.get_lib().IV_VersionDllFile()
+        return CoreBase.get_lib().IV_VersionDllFile()
 
     @staticmethod
     def IV_VersionDllFileStr() -> str:
         '''REVISE!!! Returns DLL file version str'''
-        return Base.get_lib().IV_VersionDllFileStr()
+        return CoreBase.get_lib().IV_VersionDllFileStr()
 
     @staticmethod
     def IV_SelectChannel(channel_number: int) -> int:
-        '''Sending the integer value communicates with Multichannel control:
-            if not yet active, the [int] number of tabs is automatically opened and the [int] tab becomes active;
-            if Ivium-n-Soft is active already, the [int] tab becomes active. 
-            Now the channel/instrument that is connected to this tab can be controlled. 
-            If no instrument is connected, the next available instrument in the list can be connected (IV_connect) and controlled.'''
+        '''Selects a channel:
+            - if not yet active, the [int] number of tabs is automatically opened and
+              the [int] tab becomes active.
+            - if Ivium-n-Soft is active already, the [int] tab becomes active.
+            Now the channel/instrument that is connected to this tab can be controlled.
+            If no instrument is connected, the next available instrument in the list can
+            be connected (IV_connect) and controlled.'''
         channel_number_ptr = ffi.new(LONG_PTR, channel_number)
-        result_code = Base.get_lib().IV_SelectChannel(channel_number_ptr)
+        result_code = CoreBase.get_lib().IV_SelectChannel(channel_number_ptr)
         return result_code
```

### Comparing `pyvium-0.1.6b0/pyvium/core/method_mode_functions.py` & `pyvium-0.1.7b0/pyvium/core/method_mode_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,107 +1,108 @@
-from .base import CHAR_ARRAY, DOUBLE_PTR, LONG_PTR, UTF_ENCODING, Base, ffi
+from .constants import CHAR_ARRAY, DOUBLE_PTR, LONG_PTR, UTF_ENCODING
+from .core_base import CoreBase, ffi
 
 ffi.cdef("""
     long __stdcall IV_readmethod(char *fname);
     long __stdcall IV_savemethod(char *fname);
     long __stdcall IV_startmethod(char *fname);
     long __stdcall IV_abort();
     long __stdcall IV_savedata(char *fname);
     long __stdcall IV_setmethodparameter(char *parname, char *parvalue);
     long __stdcall IV_Ndatapoints(long *value);
     long __stdcall IV_getdata(long *pointnr, double *x, double *y, double *z);
     long __stdcall IV_getdatafromline(long *pointnr, long *scannr, double *x, double *y, double *z);
 """)
 
 
-class MethodModeFunctions(Base):
+class MethodModeFunctions(CoreBase):
     @staticmethod
     def IV_readmethod(method_file_path: str) -> tuple[int, str]:
         '''Loads method procedure previously saved to a file.
             method_file_path represents the full path to the file.'''
         method_file_path_ptr = ffi.new(
             CHAR_ARRAY, method_file_path.encode(UTF_ENCODING))
-        result_code = Base.get_lib().IV_readmethod(method_file_path_ptr)
+        result_code = CoreBase.get_lib().IV_readmethod(method_file_path_ptr)
         return result_code, ffi.string(method_file_path_ptr).decode(UTF_ENCODING)
 
     @staticmethod
     def IV_savemethod(method_file_path: str) -> tuple[int, str]:
         '''Saves currently loaded method procedure to a file.
             method_file_path represents the full path to the new file.'''
         method_file_path_ptr = ffi.new(
             CHAR_ARRAY, method_file_path.encode(UTF_ENCODING))
-        result_code = Base.get_lib().IV_savemethod(method_file_path_ptr)
+        result_code = CoreBase.get_lib().IV_savemethod(method_file_path_ptr)
         return result_code, ffi.string(method_file_path_ptr).decode(UTF_ENCODING)
 
     @staticmethod
     def IV_startmethod(method_file_path='') -> tuple[int, str]:
         '''Starts a method procedure.
             If method_file_path is an empty string then the presently loaded procedure is started.
             If the full path to a previously saved method is provided
             then the procedure is loaded from the file and started.'''
         method_file_path_ptr = ffi.new(
             CHAR_ARRAY, method_file_path.encode(UTF_ENCODING))
-        result_code = Base.get_lib().IV_startmethod(method_file_path_ptr)
+        result_code = CoreBase.get_lib().IV_startmethod(method_file_path_ptr)
         return result_code, ffi.string(method_file_path_ptr).decode(UTF_ENCODING)
 
     @staticmethod
     def IV_abort() -> int:
         '''Aborts the ongoing method procedure'''
-        return Base.get_lib().IV_abort()
+        return CoreBase.get_lib().IV_abort()
 
     @staticmethod
     def IV_savedata(method_data_file_path: str) -> tuple[int, str]:
         '''Saves the results of the last method execution into a file.
             method_file_path represents the full path to the new file.'''
         method_data_file_path_ptr = ffi.new(
             CHAR_ARRAY, method_data_file_path.encode(UTF_ENCODING))
-        result_code = Base.get_lib().IV_savedata(method_data_file_path_ptr)
+        result_code = CoreBase.get_lib().IV_savedata(method_data_file_path_ptr)
         return result_code, ffi.string(method_data_file_path_ptr).decode(UTF_ENCODING)
 
     @staticmethod
     def IV_setmethodparameter(parameter_name: str, parameter_value: str) -> int:
         '''Allows updating the parameter values for the currently loaded method procedrue.
             It only works for text based parameters and dropdowns (multiple option selectors).'''
         parameter_name_ptr = ffi.new(
             CHAR_ARRAY, parameter_name.encode(UTF_ENCODING))
         parameter_value_ptr = ffi.new(
             CHAR_ARRAY, parameter_value.encode(UTF_ENCODING))
-        result_code = Base.get_lib().IV_setmethodparameter(
+        result_code = CoreBase.get_lib().IV_setmethodparameter(
             parameter_name_ptr, parameter_value_ptr)
         return result_code
 
     @staticmethod
     def IV_Ndatapoints() -> tuple[int, int]:
         '''Returns actual available number of datapoints: indicates the progress during a run'''
         data_point_ptr = ffi.new(LONG_PTR)
-        result_code = Base.get_lib().IV_Ndatapoints(data_point_ptr)
+        result_code = CoreBase.get_lib().IV_Ndatapoints(data_point_ptr)
         return result_code, data_point_ptr[0]
 
     @staticmethod
     def IV_getdata(data_point_index: int) -> tuple[int, float, float, float]:
         '''Get the data from a datapoint with index int, returns 3 values that depend on
             the used technique. For example LSV/CV methods return (E/I/0) Transient methods
             return (time/I,E/0), Impedance methods return (Z1,Z2,freq) etc.'''
         selected_data_point_index_ptr = ffi.new(LONG_PTR, data_point_index)
         measured_value1_ptr = ffi.new(DOUBLE_PTR)
         measured_value2_ptr = ffi.new(DOUBLE_PTR)
         measured_value3_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getdata(
+        result_code = CoreBase.get_lib().IV_getdata(
             selected_data_point_index_ptr, measured_value1_ptr, measured_value2_ptr, measured_value3_ptr)
         return result_code, measured_value1_ptr[0], measured_value2_ptr[0], measured_value3_ptr[0]
 
     @staticmethod
     def IV_getdatafromline(data_point_index: int, scan_index: int) -> tuple[int, float, float, float]:
         '''Same as get_data_point, but with the additional scan_index parameter.
             This function will allow reading data from non-selected (previous) scans.'''
         selected_data_point_index_ptr = ffi.new(LONG_PTR, data_point_index)
         selected_line_index_ptr = ffi.new(LONG_PTR, scan_index)
         measured_value1_ptr = ffi.new(DOUBLE_PTR)
         measured_value2_ptr = ffi.new(DOUBLE_PTR)
         measured_value3_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_getdatafromline(
+        result_code = CoreBase.get_lib().IV_getdatafromline(
             selected_data_point_index_ptr,
             selected_line_index_ptr,
             measured_value1_ptr,
             measured_value2_ptr,
             measured_value3_ptr)
         return result_code, measured_value1_ptr[0], measured_value2_ptr[0], measured_value3_ptr[0]
```

### Comparing `pyvium-0.1.6b0/pyvium/core/we32_functions.py` & `pyvium-0.1.7b0/pyvium/core/we32_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-from .base import DOUBLE_PTR, LONG_PTR, Base, ffi
+from .constants import DOUBLE_PTR, LONG_PTR
+from .core_base import CoreBase, ffi
 
 ffi.cdef("""
     long __stdcall IV_we32setchannel(long *index);
     long __stdcall IV_we32setoffset(long *index, double *value);
     long __stdcall IV_we32setoffsets(long *nval, double *values);
     long __stdcall IV_we32getoffsets(long *nval, double *values);
     long __stdcall IV_we32readcurrents(double *values);
 """)
 
 
-class We32Functions(Base):
+class We32Functions(CoreBase):
     @staticmethod
     def IV_we32setchannel(channel_index: int) -> int:
         '''Select active WE32 channel (chan)'''
         channel_index_ptr = ffi.new(LONG_PTR, channel_index)
-        result_code = Base.get_lib().IV_we32setchannel(channel_index_ptr)
+        result_code = CoreBase.get_lib().IV_we32setchannel(channel_index_ptr)
         return result_code
 
     @staticmethod
     def IV_we32setoffset(channel_index: int, value: float) -> int:
         '''Set WE32 offset (chan,value), value -2 to +2V.
             Use chan=0 to apply the same offset to all channels.'''
         channel_index_ptr = ffi.new(LONG_PTR, channel_index)
         value_ptr = ffi.new(DOUBLE_PTR, value)
-        result_code = Base.get_lib().IV_we32setoffset(channel_index_ptr, value_ptr)
+        result_code = CoreBase.get_lib().IV_we32setoffset(channel_index_ptr, value_ptr)
         return result_code
 
     @staticmethod
     def IV_we32setoffsets(number_of_channels: int, value: float) -> int:
         '''REVISE! Set WE32 offsets values (Nchan,values),
             with Nchan the number of channels (1..32)'''
         number_of_channels_index_ptr = ffi.new(LONG_PTR, number_of_channels)
         value_ptr = ffi.new(DOUBLE_PTR, value)
-        result_code = Base.get_lib().IV_we32setoffsets(
+        result_code = CoreBase.get_lib().IV_we32setoffsets(
             number_of_channels_index_ptr, value_ptr)
         return result_code
 
     @staticmethod
     def IV_we32getoffsets(number_of_channels: int) -> tuple[int, float]:
         '''REVISE! Returns actual WE32 offset values (Nchan,values),
             with Nchan the number of channels (1..32)'''
         number_of_channels_index_ptr = ffi.new(LONG_PTR, number_of_channels)
         values_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_we32getoffsets(
+        result_code = CoreBase.get_lib().IV_we32getoffsets(
             number_of_channels_index_ptr, values_ptr)
         return result_code, values_ptr[0]
 
     @staticmethod
     def IV_we32readcurrents() -> tuple[int, float]:
         '''REVISE! Returns array with 32 WE32 current values,
             that are measured simultaneously'''
         current_values_ptr = ffi.new(DOUBLE_PTR)
-        result_code = Base.get_lib().IV_we32readcurrents(current_values_ptr)
+        result_code = CoreBase.get_lib().IV_we32readcurrents(current_values_ptr)
         return result_code, current_values_ptr[0]
```

### Comparing `pyvium-0.1.6b0/pyvium/IVIUM_remdriver.dll` & `pyvium-0.1.7b0/pyvium/IVIUM_remdriver.dll`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/pyvium/Ivium_remdriver64.dll` & `pyvium-0.1.7b0/pyvium/Ivium_remdriver64.dll`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/pyvium/pyvium/direct_mode_functions.py` & `pyvium-0.1.7b0/pyvium/pyvium/direct_mode_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/pyvium/pyvium/generic_functions.py` & `pyvium-0.1.7b0/pyvium/pyvium/generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/pyvium/pyvium/method_mode_functions.py` & `pyvium-0.1.7b0/pyvium/pyvium/method_mode_functions.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/pyvium/pyvium_verifiers.py` & `pyvium-0.1.7b0/pyvium/pyvium_verifiers.py`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/README.md` & `pyvium-0.1.7b0/README.md`

 * *Files identical despite different names*

### Comparing `pyvium-0.1.6b0/setup.py` & `pyvium-0.1.7b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cffi>=1.15.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyvium',
-    'version': '0.1.6b0',
+    'version': '0.1.7b0',
     'description': 'A tiny Python wrapper around the <Software development driver DLL> for IviumSoft.',
     'long_description': '# PYVIUM\n\nTiny Python wrapper around the "Software development driver DLL" for IviumSoft.\n\n# Important:\n\nThis module uses a dll from the IviumSoft application. You need to have this software installed on a Windows machine. The IviumSoft application can be downloaded from here: https://www.ivium.com/support/#Software%20update\n\nThis version of Pyvium has been tested for IviumSoft release 4.1100.\n\n## Installation\n\nInstall PYVIUM easily with pip:\n\n```\npip install pyvium\n```\n\nOr with poetry:\n\n```\npoetry add pyvium\n```\n\n## Usage Example (Using IviumSoft Core functions)\n\nTo use the same functions available in the "IviumSoft driver DLL" you can import the Core class as follows. All functions return a result code (integer) and a result value if available. For further information you can check the IviumSoft documentation.\n\n```\nfrom pyvium import Core\n\nCore.IV_open()\nCore.IV_getdevicestatus()\nCore.IV_close()\n```\n\n## Usage Example (Using Pyvium methods)\n\nThis is a wrapper around the Core functions that adds a few things:\n\n- Exception management (you can find an example [here](https://github.com/SF-Tec/pyvium/blob/main/docs/error_management.md))\n- New functionalities\n\n```\nfrom pyvium import Pyvium\n\nPyvium.open_driver()\nPyvium.get_device_status()\nPyvium.close_driver()\n\n```\n\n## Supported functions\n\nThe list of currently supported and implemented functions can be found [here](https://github.com/SF-Tec/pyvium/blob/main/docs/method_list.md).\n\n## Links\n\n- [See on GitHub](https://github.com/sf-tec/pyvium)\n- [See on PyPI](https://pypi.org/project/pyvium)\n',
     'author': 'Alejandro Gutiérrez',
     'author_email': 'agutierrez@stec.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SF-Tec/pyvium',
```

### Comparing `pyvium-0.1.6b0/PKG-INFO` & `pyvium-0.1.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvium
-Version: 0.1.6b0
+Version: 0.1.7b0
 Summary: A tiny Python wrapper around the <Software development driver DLL> for IviumSoft.
 Home-page: https://github.com/SF-Tec/pyvium
 License: Apache-2.0
 Keywords: ivium,iviumsoft,ivium software,ivium compactstat
 Author: Alejandro Gutiérrez
 Author-email: agutierrez@stec.es
 Requires-Python: >=3.11,<4.0
```

