# Comparing `tmp/unitbrow-0.1.0.tar.gz` & `tmp/unitbrow-0.2.0.tar.gz`

## Comparing `unitbrow-0.1.0.tar` & `unitbrow-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 unitbrow-0.1.0/.release.sh
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/conversions/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/conversions/unit_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/parsers/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/parsers/unit_parser.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/values/constants/__init__.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/values/constants/constants.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/values/dimensions/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/values/dimensions/dimensions.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/values/units/__init__.py
--rw-r--r--   0        0        0    17194 2020-02-02 00:00:00.000000 unitbrow-0.1.0/uniTbrow/values/units/units.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 unitbrow-0.1.0/.gitignore
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 unitbrow-0.1.0/LICENSE
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 unitbrow-0.1.0/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unitbrow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 unitbrow-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 unitbrow-0.2.0/.release.sh
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 unitbrow-0.2.0/tests/unit_tests.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/constants/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/constants/constants.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/conversions/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/conversions/base_unit_systems.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/conversions/unit_conversions.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/dimensions/__init__.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/dimensions/dimensions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/parsers/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/parsers/unit_parser.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/units/__init__.py
+-rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/units/units.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unitbrow-0.2.0/.gitignore
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 unitbrow-0.2.0/LICENSE
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 unitbrow-0.2.0/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unitbrow-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 unitbrow-0.2.0/PKG-INFO
```

### Comparing `unitbrow-0.1.0/uniTbrow/values/constants/constants.py` & `unitbrow-0.2.0/uniTbrow/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uniTbrow.values.units.units import metre, second, newton, kelvin, joule, mole, ampere, gram, hertz, coulomb
+from uniTbrow.units.units import metre, second, newton, kelvin, joule, mole, ampere, gram, hertz, coulomb
 from sympy import pi
 
 c = 299792458 * metre * second**-1
 """Speed of light in vacuum"""
 
 G = 6.6743015*10**-11 * metre**3 * (1000*gram)**-1 * second**-2
 """Newtonian gravitational constant"""
```

### Comparing `unitbrow-0.1.0/uniTbrow/values/dimensions/dimensions.py` & `unitbrow-0.2.0/uniTbrow/dimensions/dimensions.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,20 @@
         if dimension is None:
             self.name = name
             self.dimension = _symbols(name)
         else:
             self.name = name
             self.dimension = dimension
 
+    def __repr__(self):
+        return self.name
+
+    def __str__(self):
+        return self.name + " = " + str(self.dimension)
+
 
 # SI Base Dimensions
 length = Dimension("length")
 time = Dimension("time")
 amount = Dimension("amount")
 current = Dimension("current")
 temperature = Dimension("temperature")
```

### Comparing `unitbrow-0.1.0/uniTbrow/values/units/units.py` & `unitbrow-0.2.0/uniTbrow/units/units.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sympy import symbols as _symbols, pi as _pi
-from uniTbrow.values.dimensions.dimensions import *
+from uniTbrow import dimensions
 
 _metric_prefixes = [
     ("Q", ["quetta"], 10**30),
     ("R", ["ronna"], 10**27),
     ("Y", ["yotta"], 10**24),
     ("Z", ["zetta"], 10**21),
     ("E", ["exa"], 10**18),
@@ -26,17 +26,19 @@
     ("y", ["yocto"], 10**-24),
     ("r", ["ronto"], 10**-27),
     ("q", ["quecto"], 10**-30)
 ]
 
 
 class Unit:
-    def __init__(self, dimension: Dimension, abbr_symbol: str, alternates: list, base, metric=True):
+    def __init__(self, dimension: dimensions.Dimension, abbr_symbol: str, alternates=None, base=None, metric=True):
+        if alternates is None:
+            alternates = []
         assert base is True or (base is not None), "Need to provide a conversion to a base unit"
-        self.dimension: Dimension = dimension
+        self.dimension: dimensions.Dimension = dimension
         self.symbol = _symbols(abbr_symbol)
         self.alternates: list = alternates
         self.conversions: dict = dict()
         self.metric: bool = metric
         self.base = base
 
     # add_conversion defines the factor used to convert from other_unit to this unit
@@ -48,19 +50,19 @@
 
     def generate_metric_prefixes(self):
         if not self.metric:
             return []
         metric_units = []
         for abbr, alts, factor in _metric_prefixes:
             alternates = []
-            for prefix in alts:
+            for alt_prefix in alts:
                 for suffix in self.alternates:
-                    alternates.append(str(prefix+suffix))
+                    alternates.append(str(alt_prefix+suffix))
 
-            new_unit = Unit(self.dimension, abbr+str(self.symbol), alternates, metric=False, base=factor*self.symbol)
+            new_unit = Unit(self.dimension, abbr+str(self.symbol), alternates=[], metric=False, base=factor*self.symbol)
             new_unit.add_conversion(self, factor*self.symbol)
             self.add_conversion(new_unit, (1/factor)*new_unit.symbol)
             metric_units.append(new_unit)
 
         return metric_units
 
     def __repr__(self):
@@ -70,29 +72,29 @@
         string_to_return = str(self.symbol)
         string_to_return += "[" + str(self.dimension.dimension) + "]"
         if len(self.alternates) >= 1:
             string_to_return += "\t" + str(len(self.alternates)) + " alternate spellings"
             string_to_return += " (e.g. " + str(self.alternates[0]) + ")"
         return string_to_return
 
+    def __pow__(self, power, modulo=None):
+        return pow(self.symbol, power, modulo)
+
     def __mul__(self, other):
         return self.symbol * other
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __truediv__(self, other):
         return self.symbol / other
 
     def __rtruediv__(self, other):
         return other / self.symbol
 
-    def __pow__(self, power, modulo=None):
-        return self.symbol.__pow__(power, modulo)
-
 
 class UnitLibrary:
     def __init__(self):
         self.unit_dictionary = dict()
         self.reverse_unit_dictionary = dict()
 
     def lookup(self, unit_to_lookup):
@@ -117,160 +119,160 @@
 
     def add_all(self, unit_list: list[Unit]):
         for u in unit_list:
             self.add(u)
 
 
 # Base Units
-metre = meter = Unit(length, "m", ["meter", "metre", "meters", "metres"], base=True)
-second = Unit(time, "s", ["second", "seconds", "sec", "secs"], base=True)
-mole = Unit(amount, "mole", ["mol", "moles"], base=True)
-ampere = Unit(current, "A", ["ampere", "amps", "amperes", "amp"], base=True)
-kelvin = Unit(temperature, "K", ["kelvin"], base=True)
-candela = Unit(luminous_intensity, "cd", ["candela"], base=True)
-gram = Unit(mass, "g", ["gram", "grams"], base=True)
+metre = meter = Unit(dimensions.length, "m", ["meter", "metre", "meters", "metres"], base=True)
+second = Unit(dimensions.time, "s", ["second", "seconds", "sec", "secs"], base=True)
+mole = Unit(dimensions.amount, "mole", ["mol", "moles"], base=True)
+ampere = Unit(dimensions.current, "A", ["ampere", "amps", "amperes", "amp"], base=True)
+kelvin = Unit(dimensions.temperature, "K", ["kelvin"], base=True)
+candela = Unit(dimensions.luminous_intensity, "cd", ["candela"], base=True)
+gram = Unit(dimensions.mass, "g", ["gram", "grams"], base=True)
 
 # Derived Units
 
-hertz = Unit(frequency, "Hz", ["hertz"], base=(1/second.symbol))
+hertz = Unit(dimensions.frequency, "Hz", ["hertz"], base=(1 / second.symbol))
 
-radian = Unit(angle, "rad", ["radians", "radian"], base=1)
+radian = Unit(dimensions.angle, "rad", ["radians", "radian"], base=1)
 
-steradian = Unit(solid_angle, "sr", ["steradians", "steradian"], base=1)
+steradian = Unit(dimensions.solid_angle, "sr", ["steradians", "steradian"], base=1)
 
-newton = Unit(force, "N", ["newtons", "newton"], base=(1000*gram.symbol*metre.symbol/(second.symbol**2)))
+newton = Unit(dimensions.force, "N", ["newtons", "newton"], base=(1000 * gram.symbol * metre.symbol / (second.symbol ** 2)))
 
-pascal = Unit(pressure, "Pa", ["pascals", "pascal"], base=(1000*gram.symbol * metre.symbol**-1 * second.symbol**-2))
+pascal = Unit(dimensions.pressure, "Pa", ["pascals", "pascal"], base=(1000 * gram.symbol * metre.symbol ** -1 * second.symbol ** -2))
 
-joule = Unit(energy, "J", ["joule", "joules"], base=(1000*gram.symbol * metre.symbol**2 * second.symbol**-2))
+joule = Unit(dimensions.energy, "J", ["joule", "joules"], base=(1000 * gram.symbol * metre.symbol ** 2 * second.symbol ** -2))
 
-watt = Unit(power, "W", ["watt", "watts"], base=(1000*gram.symbol * metre.symbol**2 * second.symbol**-3))
+watt = Unit(dimensions.power, "W", ["watt", "watts"], base=(1000 * gram.symbol * metre.symbol ** 2 * second.symbol ** -3))
 
-coulomb = Unit(charge, "C", ["coulombs", "coulomb"], base=(second.symbol * ampere.symbol))
+coulomb = Unit(dimensions.charge, "C", ["coulombs", "coulomb"], base=(second.symbol * ampere.symbol))
 
-volt = Unit(electric_potential, "V", ["volts", "volt"], base=(1000*gram.symbol * metre.symbol**2 * second.symbol**-3 * ampere.symbol**-1))
+volt = Unit(dimensions.electric_potential, "V", ["volts", "volt"], base=(1000 * gram.symbol * metre.symbol ** 2 * second.symbol ** -3 * ampere.symbol ** -1))
 
-farad = Unit(capacitance, "F", ["farads", "farad"], base=((1000*gram.symbol)**-1 * metre.symbol**-2 * second.symbol**4 * ampere.symbol**2))
+farad = Unit(dimensions.capacitance, "F", ["farads", "farad"], base=((1000 * gram.symbol) ** -1 * metre.symbol ** -2 * second.symbol ** 4 * ampere.symbol ** 2))
 
-ohm = Unit(resistance, "Ω", ["ohms", "ohm"], base=(1000*gram.symbol * metre.symbol**2 * second.symbol**-3 * ampere.symbol**-2))
+ohm = Unit(dimensions.resistance, "Ω", ["ohms", "ohm"], base=(1000 * gram.symbol * metre.symbol ** 2 * second.symbol ** -3 * ampere.symbol ** -2))
 
-siemens = Unit(conductance, "S", ["siemens", "siemen", "mho", "mhos"], base=((1000*gram.symbol)**-1 * metre.symbol**-2 * second.symbol**3 * ampere.symbol**2))
+siemens = Unit(dimensions.conductance, "S", ["siemens", "siemen", "mho", "mhos"], base=((1000 * gram.symbol) ** -1 * metre.symbol ** -2 * second.symbol ** 3 * ampere.symbol ** 2))
 
-weber = Unit(magnetic_flux, "Wb", ["weber", "webers"], base=(1000*gram.symbol * metre.symbol**2 * second.symbol**-2 * ampere.symbol**-1))
+weber = Unit(dimensions.magnetic_flux, "Wb", ["weber", "webers"], base=(1000 * gram.symbol * metre.symbol ** 2 * second.symbol ** -2 * ampere.symbol ** -1))
 
-tesla = Unit(magnetic_induction, "T", ["tesla", "teslas"], base=(1000*gram.symbol * second.symbol**-2 * ampere.symbol**-1))
+tesla = Unit(dimensions.magnetic_induction, "T", ["tesla", "teslas"], base=(1000 * gram.symbol * second.symbol ** -2 * ampere.symbol ** -1))
 
-henry = Unit(electric_inductance, "H", ["henry", "henrys"], base=(1000*gram.symbol * metre.symbol**2 * second.symbol**-2 * ampere.symbol**-2))
+henry = Unit(dimensions.electric_inductance, "H", ["henry", "henrys"], base=(1000 * gram.symbol * metre.symbol ** 2 * second.symbol ** -2 * ampere.symbol ** -2))
 
 # Astronomical Units
-mass_sun = Unit(mass, "M_⊙", ["solar_mass", "solar_masses", "M_sun"], metric=False, base=(1.98847*10**33 * gram.symbol))
-parsec = Unit(length, "pc", ["parsec", "parsecs"], base=(3.0856775814913*10**16*metre.symbol))
-astronomical_unit = Unit(length, "AU", ["au", "astronomical_units", "astronomical_unit"], metric=False, base=(1.495978707*10**11*metre.symbol))
-lightyear = Unit(length, "ly", ["lightyear", "lyr", "lyrs", "lightyears", "light_year", "light_years"], base=(9460730472580800*metre.symbol))
-solar_luminosity = Unit(power, "L_⊙", ["L_sun", "solar_luminosity", "solar_luminosities"], metric=False, base=(3.828*10**26*watt.base))
+mass_sun = Unit(dimensions.mass, "M_⊙", ["solar_mass", "solar_masses", "M_sun"], metric=False, base=(1.98847 * 10 ** 33 * gram.symbol))
+parsec = Unit(dimensions.length, "pc", ["parsec", "parsecs"], base=(3.0856775814913 * 10 ** 16 * metre.symbol))
+astronomical_unit = Unit(dimensions.length, "AU", ["au", "astronomical_units", "astronomical_unit"], metric=False, base=(1.495978707 * 10 ** 11 * metre.symbol))
+lightyear = Unit(dimensions.length, "ly", ["lightyear", "lyr", "lyrs", "lightyears", "light_year", "light_years"], base=(9460730472580800 * metre.symbol))
+solar_luminosity = Unit(dimensions.power, "L_⊙", ["L_sun", "solar_luminosity", "solar_luminosities"], metric=False, base=(3.828 * 10 ** 26 * watt.base))
 
 # Additional length units
-fermi = Unit(length, "fermi", ["fermis"], base=(10**-15*metre.symbol))
-angstrom = Unit(length, "Å", ["angstrom", "angstroms"], metric=False, base=(100*10**-12*metre.symbol))
-micron = Unit(length, "micron", ["microns"], metric=False, base=(10**-6*metre.symbol))
-yard = Unit(length, "yd", ["yards", "yds", "yard"], metric=False, base=(0.9144*metre.symbol))
-foot = Unit(length, "ft", ["feet", "foot"], metric=False, base=(yard.base/3))
-inch = Unit(length, "in", ["inch", "inches"], metric=False, base=(foot.base/12))
-mile = Unit(length, "mile", ["miles"], metric=False, base=(foot.base*5280))
-fathom = Unit(length, "fathom", ["fathoms"], metric=False, base=(6 * foot.base))
-nautical_mile = Unit(length, "nmi", ["NM", "M", "nautical_mile", "nautical_miles"], metric=False, base=(1852*metre.symbol))
-furlong = Unit(length, "furlong", ["furlongs"], metric=False, base=(220*yard.base))
+fermi = Unit(dimensions.length, "fermi", ["fermis"], base=(10 ** -15 * metre.symbol))
+angstrom = Unit(dimensions.length, "Å", ["angstrom", "angstroms"], metric=False, base=(100 * 10 ** -12 * metre.symbol))
+micron = Unit(dimensions.length, "micron", ["microns"], metric=False, base=(10 ** -6 * metre.symbol))
+yard = Unit(dimensions.length, "yd", ["yards", "yds", "yard"], metric=False, base=(0.9144 * metre.symbol))
+foot = Unit(dimensions.length, "ft", ["feet", "foot"], metric=False, base=(yard.base / 3))
+inch = Unit(dimensions.length, "in", ["inch", "inches"], metric=False, base=(foot.base / 12))
+mile = Unit(dimensions.length, "mile", ["miles"], metric=False, base=(foot.base * 5280))
+fathom = Unit(dimensions.length, "fathom", ["fathoms"], metric=False, base=(6 * foot.base))
+nautical_mile = Unit(dimensions.length, "nmi", ["NM", "M", "nautical_mile", "nautical_miles"], metric=False, base=(1852 * metre.symbol))
+furlong = Unit(dimensions.length, "furlong", ["furlongs"], metric=False, base=(220 * yard.base))
 
 # Additional time units
-minute = Unit(time, "min", ["mins", "minutes", "minute"], metric=False, base=(60*second.symbol))
-hour = Unit(time, "hr", ["hrs", "hours", "hour"], metric=False, base=(3600*second.symbol))
-day = Unit(time, "day", ["days"], metric=False, base=(86400*second.symbol))
-week = Unit(time, "week", ["weeks"], metric=False, base=(7*86400*second.symbol))
-year = Unit(time, "yr", ["year", "years", "yrs"], base=(86400*365.25*second.symbol))
+minute = Unit(dimensions.time, "min", ["mins", "minutes", "minute"], metric=False, base=(60 * second.symbol))
+hour = Unit(dimensions.time, "hr", ["hrs", "hours", "hour"], metric=False, base=(3600 * second.symbol))
+day = Unit(dimensions.time, "day", ["days"], metric=False, base=(86400 * second.symbol))
+week = Unit(dimensions.time, "week", ["weeks"], metric=False, base=(7 * 86400 * second.symbol))
+year = Unit(dimensions.time, "yr", ["year", "years", "yrs"], base=(86400 * 365.25 * second.symbol))
 
 # Additional temperature units
-# TODO celsius = Unit(temperature, "°C", ["degrees_celsius", "°celsius", "celsius"], base=(1 + 273.15 * kelvin.symbol))
-# TODO fahrenheit = Unit(temperature, "°F", ["degrees_fahrenheit", "°fahrenheit", "fahrenheit"], base=(1))
-rankine = Unit(temperature, "°R", ["rankine", "degrees_rankine", "°rankine"], base=((5/9)*kelvin.symbol))
+# TODO celsius = Unit(dimensions.temperature, "°C", ["degrees_celsius", "°celsius", "celsius"], base=(1 + 273.15 * kelvin.symbol))
+# TODO fahrenheit = Unit(dimensions.temperature, "°F", ["degrees_fahrenheit", "°fahrenheit", "fahrenheit"], base=(1))
+rankine = Unit(dimensions.temperature, "°R", ["rankine", "degrees_rankine", "°rankine"], base=((5 / 9) * kelvin.symbol))
 
 # Additional luminosity units
-lumen = Unit(luminous_flux, "lm", ["lumen", "lumens"], base=(candela.symbol * steradian.symbol))
+lumen = Unit(dimensions.luminous_flux, "lm", ["lumen", "lumens"], base=(candela.symbol * steradian.symbol))
 
-lux = Unit(illuminance, "lx", ["lux"], metric=False, base=(candela.symbol * steradian.symbol * metre.symbol**-2))
-foot_candle = Unit(illuminance, "fc", ["foot_candle", "ft_c"], metric=False, base=(lumen.base * foot.base**-2))
-phot = Unit(illuminance, "ph", ["phot", "phots"], metric=False, base=(10000 * lux.base))
+lux = Unit(dimensions.illuminance, "lx", ["lux"], metric=False, base=(candela.symbol * steradian.symbol * metre.symbol ** -2))
+foot_candle = Unit(dimensions.illuminance, "fc", ["foot_candle", "ft_c"], metric=False, base=(lumen.base * foot.base ** -2))
+phot = Unit(dimensions.illuminance, "ph", ["phot", "phots"], metric=False, base=(10000 * lux.base))
 
 # Additional mass units
-tonne = Unit(mass, "t", ["tonne", "tonnes", "metric_ton", "metric_tons"], metric=False, base=(1000000*gram.symbol))
-dalton = Unit(mass, "Da", ["u", "dalton", "daltons"], base=(1.6604390666050*10**-24*gram.symbol))
-slug = Unit(mass, "sl", ["slug", "slugs"], metric=False, base=(14593.90*gram.symbol))
-pound = Unit(mass, "lb", ["lbs", "pound", "pounds"], metric=False, base=(453.59237*gram.symbol))
-ounce = Unit(mass, "oz", ["ounce", "ounces"], metric=False, base=(pound.base/16))
-ton = Unit(mass, "tons", ["ton", "short_ton", "short_tons"], metric=False, base=(2000*pound.base))
-long_ton = Unit(mass, "long_tons", ["long_ton", "imperial_ton", "imperial_tons", "displacement_ton", "displacement_tons"], metric=False, base=(2240*pound.base))
-carat = Unit(mass, "ct", ["carat", "carats"], base=(0.2*gram.symbol))
-imperial_carat = Unit(mass, "imp_ct", ["imp_carat", "imp_carats", "imperial_carat", "imperial_carats"], metric=False, base=(0.00705*ounce.base))
+tonne = Unit(dimensions.mass, "t", ["tonne", "tonnes", "metric_ton", "metric_tons"], metric=False, base=(1000000 * gram.symbol))
+dalton = Unit(dimensions.mass, "Da", ["u", "dalton", "daltons"], base=(1.6604390666050 * 10 ** -24 * gram.symbol))
+slug = Unit(dimensions.mass, "sl", ["slug", "slugs"], metric=False, base=(14593.90 * gram.symbol))
+pound = Unit(dimensions.mass, "lb", ["lbs", "pound", "pounds"], metric=False, base=(453.59237 * gram.symbol))
+ounce = Unit(dimensions.mass, "oz", ["ounce", "ounces"], metric=False, base=(pound.base / 16))
+ton = Unit(dimensions.mass, "tons", ["ton", "short_ton", "short_tons"], metric=False, base=(2000 * pound.base))
+long_ton = Unit(dimensions.mass, "long_tons", ["long_ton", "imperial_ton", "imperial_tons", "displacement_ton", "displacement_tons"], metric=False, base=(2240 * pound.base))
+carat = Unit(dimensions.mass, "ct", ["carat", "carats"], base=(0.2 * gram.symbol))
+imperial_carat = Unit(dimensions.mass, "imp_ct", ["imp_carat", "imp_carats", "imperial_carat", "imperial_carats"], metric=False, base=(0.00705 * ounce.base))
 
 # Additional force units
-pound_force = Unit(force, "lbf", ["pound_force, pound_of_force"], metric=False, base=(4.4482216152605*newton.base))
-dyne = Unit(force, "dyn", ["dyne", "dynes"], metric=False, base=(10**-5*newton.base))
-poundal = Unit(force, "pdl", ["poundal"], metric=False, base=(pound.base * foot.base * second.symbol**-2))
+pound_force = Unit(dimensions.force, "lbf", ["pound_force, pound_of_force"], metric=False, base=(4.4482216152605 * newton.base))
+dyne = Unit(dimensions.force, "dyn", ["dyne", "dynes"], metric=False, base=(10 ** -5 * newton.base))
+poundal = Unit(dimensions.force, "pdl", ["poundal"], metric=False, base=(pound.base * foot.base * second.symbol ** -2))
 
 # Additional energy units
-erg = Unit(energy, "erg", ["ergs"], metric=False, base=(10**-7*joule.base))
-calorie = Unit(energy, "cal", ["calorie", "calories"], base=(4.184*joule.base))
-electron_volt = Unit(energy, "eV", ["electronvolt", "electronvolts", "electron_volt", "electron_volts"], base=(1.602176634*10**-19 * joule.base))
+erg = Unit(dimensions.energy, "erg", ["ergs"], metric=False, base=(10 ** -7 * joule.base))
+calorie = Unit(dimensions.energy, "cal", ["calorie", "calories"], base=(4.184 * joule.base))
+electron_volt = Unit(dimensions.energy, "eV", ["electronvolt", "electronvolts", "electron_volt", "electron_volts"], base=(1.602176634 * 10 ** -19 * joule.base))
 
 # Additional power units
-metric_horsepower = Unit(power, "hp", ["hp_M", "horsepower", "metric_horsepower"], base=(735.49875*watt.base))
-mechanical_horsepower = Unit(power, "hp_I", ["mechanical_horsepower", "imperial_horsepower"], metric=False, base=(550*foot.base*pound_force.base / second.symbol))
-electical_horsepower = Unit(power, "hp_E", ["electrical_horsepower"], metric=False, base=(746*watt.base))
-boiler_horsepower = Unit(power, "hp_S", ["boiler_horsepower"], metric=False, base=(9812.5*watt.base))
+metric_horsepower = Unit(dimensions.power, "hp", ["hp_M", "horsepower", "metric_horsepower"], base=(735.49875 * watt.base))
+mechanical_horsepower = Unit(dimensions.power, "hp_I", ["mechanical_horsepower", "imperial_horsepower"], metric=False, base=(550 * foot.base * pound_force.base / second.symbol))
+electical_horsepower = Unit(dimensions.power, "hp_E", ["electrical_horsepower"], metric=False, base=(746 * watt.base))
+boiler_horsepower = Unit(dimensions.power, "hp_S", ["boiler_horsepower"], metric=False, base=(9812.5 * watt.base))
 
 # Additional pressure units
-bar = Unit(pressure, "bar", ["bars"], base=(100000*pascal.base))
-standard_atmosphere = Unit(pressure, "atm", ["atmosphere", "atmospheres", "standard_atmosphere", "standard_atmospheres"], metric=False, base=(101325*pascal.base))
-millimetre_mercury = millimeter_mercury = Unit(pressure, "mmHg", ["mm_Hg"], metric=False, base=(133.322*pascal.base))
-inch_mercury = Unit(pressure, "inHg", ["in_Hg"], metric=False, base=(3386.389*pascal.base))
-torr = Unit(pressure, "Torr", ["torr"], metric=False, base=((101325/760)*pascal.base))
+bar = Unit(dimensions.pressure, "bar", ["bars"], base=(100000 * pascal.base))
+standard_atmosphere = Unit(dimensions.pressure, "atm", ["atmosphere", "atmospheres", "standard_atmosphere", "standard_atmospheres"], metric=False, base=(101325 * pascal.base))
+millimetre_mercury = millimeter_mercury = Unit(dimensions.pressure, "mmHg", ["mm_Hg"], metric=False, base=(133.322 * pascal.base))
+inch_mercury = Unit(dimensions.pressure, "inHg", ["in_Hg"], metric=False, base=(3386.389 * pascal.base))
+torr = Unit(dimensions.pressure, "Torr", ["torr"], metric=False, base=((101325 / 760) * pascal.base))
 
 # Additional angular measurements
-degree = Unit(angle, "°", ["deg", "degree", "degrees", "arcdegree", "arcdegrees", "degree_of_arc", "degrees_of_arc", "arc_degree", "arc_degrees"], metric=False, base=((_pi/180)*radian.base))
-turn = Unit(angle, "tr", ["pla", "turn", "turns"], metric=False, base=(2*_pi*radian.base))
-gradian = Unit(angle, "gon", ["ᵍ", "grad", "grade", "grads", "grades"], metric=False, base=((_pi/200)*radian.base))
-square_degree = Unit(solid_angle, "square_deg", ["sq_deg", "square_degree", "square_degrees"], metric=False, base=((_pi/180)**2 * steradian.base))
-arcminute = Unit(angle, "arcmin", ["arc_minute", "arc_minutes", "arcminute", "arcminutes", "minute_arc", "minutes_arc"], metric=False, base=(degree.base / 60))
-arcsecond = Unit(angle, "as", ["arcsec", "asec", "arc_second", "arc_seconds", "arcsecond", "arcseconds", "second_of_arc", "seconds_of_arc"], base=(arcminute.base / 60))
+degree = Unit(dimensions.angle, "°", ["deg", "degree", "degrees", "arcdegree", "arcdegrees", "degree_of_arc", "degrees_of_arc", "arc_degree", "arc_degrees"], metric=False, base=((_pi / 180) * radian.base))
+turn = Unit(dimensions.angle, "tr", ["pla", "turn", "turns"], metric=False, base=(2 * _pi * radian.base))
+gradian = Unit(dimensions.angle, "gon", ["ᵍ", "grad", "grade", "grads", "grades"], metric=False, base=((_pi / 200) * radian.base))
+square_degree = Unit(dimensions.solid_angle, "square_deg", ["sq_deg", "square_degree", "square_degrees"], metric=False, base=((_pi / 180) ** 2 * steradian.base))
+arcminute = Unit(dimensions.angle, "arcmin", ["arc_minute", "arc_minutes", "arcminute", "arcminutes", "minute_arc", "minutes_arc"], metric=False, base=(degree.base / 60))
+arcsecond = Unit(dimensions.angle, "as", ["arcsec", "asec", "arc_second", "arc_seconds", "arcsecond", "arcseconds", "second_of_arc", "seconds_of_arc"], base=(arcminute.base / 60))
 
 
 # Additional volume units
-litre = liter = Unit(volume, "L", ["l", "ℓ", "liter", "litre", "liters", "litres"], base=(10**-3 * metre.symbol))
-us_gallon = Unit(volume, "US_gal", ["US_gallon", "US_gallons"], metric=False, base=(231*inch.base**3))
-us_dry_gallon = Unit(volume, "US_dry_gal", ["US_dry_gallon", "US_dry_gallons"], metric=False, base=(268.8025*inch.base**3))
-imperial_gallon = Unit(volume, "imp_gal", ["imperial_gallon", "imp_gallon", "imperial_gallons", "imp_gallons"], metric=False, base=(4.54609*litre.base))
-us_quart = Unit(volume, "US_qt", ["US_quart", "US_quarts"], metric=False, base=(us_gallon.base / 4))
-us_dry_quart = Unit(volume, "US_dry_qt", ["US_dry_quarts", "US_dry_quart"], metric=False, base=(us_dry_gallon.base / 4))
-imperial_quart = Unit(volume, "imp_qt", ["imperial_quart", "imp_quart", "imperial_quarts", "imp_quarts"], metric=False, base=(imperial_gallon.base / 4))
+litre = liter = Unit(dimensions.volume, "L", ["l", "ℓ", "liter", "litre", "liters", "litres"], base=(10 ** -3 * metre.symbol))
+us_gallon = Unit(dimensions.volume, "US_gal", ["US_gallon", "US_gallons"], metric=False, base=(231 * inch.base ** 3))
+us_dry_gallon = Unit(dimensions.volume, "US_dry_gal", ["US_dry_gallon", "US_dry_gallons"], metric=False, base=(268.8025 * inch.base ** 3))
+imperial_gallon = Unit(dimensions.volume, "imp_gal", ["imperial_gallon", "imp_gallon", "imperial_gallons", "imp_gallons"], metric=False, base=(4.54609 * litre.base))
+us_quart = Unit(dimensions.volume, "US_qt", ["US_quart", "US_quarts"], metric=False, base=(us_gallon.base / 4))
+us_dry_quart = Unit(dimensions.volume, "US_dry_qt", ["US_dry_quarts", "US_dry_quart"], metric=False, base=(us_dry_gallon.base / 4))
+imperial_quart = Unit(dimensions.volume, "imp_qt", ["imperial_quart", "imp_quart", "imperial_quarts", "imp_quarts"], metric=False, base=(imperial_gallon.base / 4))
 # TODO cup https://en.wikipedia.org/wiki/Cup_(unit)
 # TODO tablespoon https://en.wikipedia.org/wiki/Tablespoon
 # TODO teaspoon https://en.wikipedia.org/wiki/Teaspoon
-us_fluid_ounce = Unit(volume, "US_fl_oz", ["US_fluid_ounce", "US_fluid_ounces"], metric=False, base=(us_gallon.base / 128))
-imperial_fluid_ounce = Unit(volume, "imp_fl_oz", ["imp_fluid_ounce", "imp_fluid_ounces", "imperial_fluid_ounce", "imperial_fluid_ounces"], metric=False, base=(imperial_gallon.base / 160))
-us_peck = Unit(volume, "US_peck", ["US_pecks"], metric=False, base=(2*us_gallon.base))
-imperial_peck = Unit(volume, "imp_peck", ["imp_pecks", "imperial_peck", "imperial_pecks"], metric=False, base=(2*imperial_gallon.base))
-us_bushel = Unit(volume, "US_bushel", ["US_bushels", "US_bu", "US_bsh"], metric=False, base=(8*us_gallon.base))
-imperial_bushel = Unit(volume, "imp_bushel", ["imp_bushels", "imperial_bushel", "imperial_bushels", "imp_bu", "imp_bsh"], metric=False, base=(8*imperial_gallon.base))
+us_fluid_ounce = Unit(dimensions.volume, "US_fl_oz", ["US_fluid_ounce", "US_fluid_ounces"], metric=False, base=(us_gallon.base / 128))
+imperial_fluid_ounce = Unit(dimensions.volume, "imp_fl_oz", ["imp_fluid_ounce", "imp_fluid_ounces", "imperial_fluid_ounce", "imperial_fluid_ounces"], metric=False, base=(imperial_gallon.base / 160))
+us_peck = Unit(dimensions.volume, "US_peck", ["US_pecks"], metric=False, base=(2 * us_gallon.base))
+imperial_peck = Unit(dimensions.volume, "imp_peck", ["imp_pecks", "imperial_peck", "imperial_pecks"], metric=False, base=(2 * imperial_gallon.base))
+us_bushel = Unit(dimensions.volume, "US_bushel", ["US_bushels", "US_bu", "US_bsh"], metric=False, base=(8 * us_gallon.base))
+imperial_bushel = Unit(dimensions.volume, "imp_bushel", ["imp_bushels", "imperial_bushel", "imperial_bushels", "imp_bu", "imp_bsh"], metric=False, base=(8 * imperial_gallon.base))
 
 # Additional velocity units
-mile_per_hour = Unit(velocity, "mph", ["miles_per_hour", "mile_per_hour"], metric=False, base=(mile.base / hour.base))
-knot = Unit(velocity, "kt", ["knots", "kn", "knot"], metric=False, base=(1852 * metre.symbol / hour.base))
+mile_per_hour = Unit(dimensions.velocity, "mph", ["miles_per_hour", "mile_per_hour"], metric=False, base=(mile.base / hour.base))
+knot = Unit(dimensions.velocity, "kt", ["knots", "kn", "knot"], metric=False, base=(1852 * metre.symbol / hour.base))
 
 # Additional area units
-acre = Unit(area, "acre", ["ac", "acres"], metric=False, base=(4840 * yard.base**2))
-hectare = Unit(area, "ha", ["hectare", "hectares"], metric=False, base=(10**4 * metre.symbol**2))
+acre = Unit(dimensions.area, "acre", ["ac", "acres"], metric=False, base=(4840 * yard.base ** 2))
+hectare = Unit(dimensions.area, "ha", ["hectare", "hectares"], metric=False, base=(10 ** 4 * metre.symbol ** 2))
 
 _units = [
     # Base Units
     metre, second, mole, ampere, kelvin, candela, gram,
 
     # Derived Units
     hertz, radian, steradian, newton, pascal, joule, watt, coulomb, volt, farad, ohm, siemens, weber, tesla, henry,
@@ -326,7 +328,23 @@
 
 library = UnitLibrary()
 library.add_all(_units)
 
 
 def lookup(unit_to_lookup):
     return library.lookup(unit_to_lookup)
+
+
+def to_base_units(expr):
+    changes = -1
+    while changes != 0:
+        changes = 0
+        for symbol in expr.free_symbols:
+            try:
+                _unit = library.lookup(symbol)
+                if _unit.base is True:
+                    continue
+                changes += 1
+                expr = expr.subs(symbol, _unit.base)
+            except KeyError:
+                continue
+    return expr
```

### Comparing `unitbrow-0.1.0/LICENSE` & `unitbrow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitbrow-0.1.0/pyproject.toml` & `unitbrow-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="uniTbrow"
-version="0.1.0"
+version="0.2.0"
 authors = [
     { name="Matthew Whitaker", email="sub6resources@gmail.com" },
 ]
 dependencies = [
     "sympy",
 ]
 description="Stop raising your brow at unit conversions"
```

### Comparing `unitbrow-0.1.0/PKG-INFO` & `unitbrow-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniTbrow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Stop raising your brow at unit conversions
 Project-URL: Homepage, https://github.com/Sub6Resources/uniTbrow
 Project-URL: Issues, https://github.com/Sub6Resources/uniTbrow/issues
 Author-email: Matthew Whitaker <sub6resources@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

