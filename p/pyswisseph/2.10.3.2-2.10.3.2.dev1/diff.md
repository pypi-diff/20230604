# Comparing `tmp/pyswisseph-2.10.3.2.tar.gz` & `tmp/pyswisseph-2.10.3.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswisseph-2.10.3.2.tar", last modified: Sun Jun  4 16:49:22 2023, max compression
+gzip compressed data, was "pyswisseph-2.10.3.2.dev1.tar", last modified: Mon Sep 19 18:20:28 2022, max compression
```

## Comparing `pyswisseph-2.10.3.2.tar` & `pyswisseph-2.10.3.2.dev1.tar`

### file list

```diff
@@ -1,454 +1,454 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.392454 pyswisseph-2.10.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-04 16:49:22.392454 pyswisseph-2.10.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.296452 pyswisseph-2.10.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.296452 pyswisseph-2.10.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/_static/.placeholder
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.296452 pyswisseph-2.10.3.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/_templates/.placeholder
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/apparent_vs_true_planetary_positions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/delta_t.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.296452 pyswisseph-2.10.3.2/docs/ephemerides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.300452 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/asteroid_99942_apophis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/asteroid_ephemeris_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/ceres_an_application_for_asteroid_astrology.rst
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/ceres_pallas_juno_vesta.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/chiron.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/how_the_asteroids_were_computed.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/asteroids/pholus.rst
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/comets_and_interstellar_objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/fixed_stars_and_galactic_center.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.300452 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/harrington.rst
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/nibiru.rst
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/selena_white_moon.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/the_planets_x.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/transpluto_isis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/uranian_planets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/vulcan.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/waldemath_black_moon.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.300452 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/interpolated_or_natural_apogee_and_perigee.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/mean_lunar_node_and_mean_lunar_apogee.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/osculating_apogee.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/planetary_nodes_and_apsides.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/true_node.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.304453 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/comparisons_with_aa_and_jpl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/compression_mechanism.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/details_of_coordinate_transformation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/extension_of_de406_based_ephemerides.rst
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/solar_ephemeris_in_the_remote_past.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.304453 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/jpl_ephemeris.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/moshier_ephemeris.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/swiss_ephemeris.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/planetary_centers_of_body_and_planetary_moons.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.304453 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/ayanamshas_with_different_precession_rates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/babylonian_tradition_and_fagan_bradley_ayanamsha.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/conclusions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/defining_the_zodiac.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/hipparchan_tradition.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/image002.png
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/krishnamurti_ayanamshas.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/on_which_ecliptic_is_the_ayanamsha_measured.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/other_ayanamshas.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_center.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_equator.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/spica_citra_tradition_and_lahiri_ayanamsha.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/standard_equinoxes_and_precession_corrected_transits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/ephemerides/sidereal/suryasiddhanta_and_aryabhata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/geo_topo_helio_bary_and_planetocentric_positions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.308452 pyswisseph-2.10.3.2/docs/heliacal_events_eclipses_occultations_etc/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/heliacal_events_eclipses_occultations_etc/eclipses_occultations_risings_settings_etc.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/heliacal_events_eclipses_occultations_etc/heliacal_events_of_the_moon_planets_and_stars.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/heliacal_events_eclipses_occultations_etc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/image001.png
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.312453 pyswisseph-2.10.3.2/docs/programmers_manual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.312453 pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/apsides_nodes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/distances.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/kepler_elements.rst
--rw-r--r--   0 runner    (1001) docker     (123)    70777 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/cmake01.png
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/crossings_of_planets_over_positions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.312453 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/calendar_date_and_julian_day.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/datetime_example1.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/datetime_example2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/delta_t.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/handling_of_leap_seconds.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/mean_solar_time_vs_true_solar_time.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/seleapsec.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/swe_deltat.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/utc_and_julian_day.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/ephemeris_related_functions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.312453 pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/different_functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/fixed_stars_magnitude.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/fixed_stars_positions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   133990 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/sefstars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/house_cusp_calculation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/house_position_of_a_planet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/other_functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/placalc_functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planet_name.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.316453 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/attributes_of_lunar_eclipse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/attributes_of_occultation_by_the_moon.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/attributes_of_solar_eclipse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/ecliptical_or_equatorial_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/find_position_of_maximal_eclipse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/heliacal_details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/heliacal_risings_and_settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/horizontal_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/magnitude_limit_for_visibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_lunar_eclipse_for_given_position.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_lunar_eclipse_globally.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_occultation_by_the_moon_for_given_position.rst
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_occultation_by_the_moon_globally.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_solar_eclipse_for_given_position.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_solar_eclipse_globally.rst
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/phase_elongation_diameter_magnitude.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/refraction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/risings_settings_meridian_transits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/sunrise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.316453 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.320453 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/additional_asteroids.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/fictitious_planets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/obliquity_and_nutation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/planetary_moons_and_body_centers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/seorbel.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/call_parameters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/error_handling_and_return_values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.320453 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/coordinate_systems.rst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/ephemeris_flags.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/specialities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/speed_flags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/the_use_of_flag_bits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/position_and_speed.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/seasnam2_sample.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/seasnam_sample.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/sidereal_mode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/sidereal_time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/sign_of_geographical_longitudes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/steps_to_get_a_planets_position.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/swemini.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/programmers_manual/topocentric_planet_positions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.320453 pyswisseph-2.10.3.2/docs/sidereal_time_ascendant_mc_houses_vertex/
--rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/sidereal_time_ascendant_mc_houses_vertex/astrological_house_systems.rst
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/sidereal_time_ascendant_mc_houses_vertex/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/docs/sidereal_time_ascendant_mc_houses_vertex/sidereal_time.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.328453 pyswisseph-2.10.3.2/libswe/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 16:49:12.000000 pyswisseph-2.10.3.2/libswe/.git
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.328453 pyswisseph-2.10.3.2/libswe/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/contrib/mirror_ephedir.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.328453 pyswisseph-2.10.3.2/libswe/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.340453 pyswisseph-2.10.3.2/libswe/doc/media/
--rw-r--r--   0 runner    (1001) docker     (123)    78370 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image1.png
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image10.png
--rw-r--r--   0 runner    (1001) docker     (123)    42250 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image11.png
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image12.png
--rw-r--r--   0 runner    (1001) docker     (123)   150205 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image13.png
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image14.png
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image15.png
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image16.png
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image17.png
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image18.png
--rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image19.png
--rw-r--r--   0 runner    (1001) docker     (123)    36536 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image2.png
--rw-r--r--   0 runner    (1001) docker     (123)   105074 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image20.png
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image21.png
--rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image22.png
--rw-r--r--   0 runner    (1001) docker     (123)    42926 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image23.png
--rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image24.png
--rw-r--r--   0 runner    (1001) docker     (123)    26084 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image25.png
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image26.png
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image27.png
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image28.png
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image29.png
--rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image3.png
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image30.png
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image31.png
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image32.png
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image33.png
--rw-r--r--   0 runner    (1001) docker     (123)    20037 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image34.png
--rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image35.png
--rw-r--r--   0 runner    (1001) docker     (123)    61456 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image36.png
--rw-r--r--   0 runner    (1001) docker     (123)    54484 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image37.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   837343 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image38.png
--rw-r--r--   0 runner    (1001) docker     (123)    92198 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image39.png
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image4.png
--rw-r--r--   0 runner    (1001) docker     (123)    53347 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image40.png
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image5.png
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image6.png
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image7.png
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image8.png
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/media/image9.png
--rw-r--r--   0 runner    (1001) docker     (123)   267146 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/swephprg.md
--rw-r--r--   0 runner    (1001) docker     (123)   287589 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/doc/swisseph.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sedeltat.txt.inactive
--rw-r--r--   0 runner    (1001) docker     (123)   134182 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sefstars.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/seleapsec.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/seorbel.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.360454 pyswisseph-2.10.3.2/libswe/setest/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/checkpoints.c
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/checkpoints.h
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/cmd.gdb
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/constants.c
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/gen_fix_templ.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/generate_prepare_fix_m4.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1692 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/generate_prepare_fix_m4a.pl
--rw-r--r--   0 runner    (1001) docker     (123)    53872 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/generated_tests.c
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/globals.c
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/globals.h
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/globals_suite.c
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/multivalues.c
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/multivalues.h
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/mytest.fix
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/prepare_fix.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/reader.h
--rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/setest.c
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/setest.h
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/setest.help
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/setest.md
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_01_calc.c
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_02_fixstar.c
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_03_misc.c
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_04_ayanamsa.c
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_05_date_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_06_houses.c
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_07_apsides.c
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_08_eclipses.c
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_09_rise.c
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/suite_10_solcross.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.360454 pyswisseph-2.10.3.2/libswe/setest/t/
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t/test
--rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t/test.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t/test_dummy.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t/test_mytest_ok.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t/test_read_section.sh
--rw-r--r--   0 runner    (1001) docker     (123) 12977948 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t.exp
--rw-r--r--   0 runner    (1001) docker     (123)    21457 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/t.fix
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/test_one_per_process.pl
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testdata.c
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testdata.h
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testdata.s
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testsuite.m4
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testsuite_end.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testsuite_facade.h
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/setest/testsuite_final.h
--rw-r--r--   0 runner    (1001) docker     (123)    63177 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweasp.c
--rw-r--r--   0 runner    (1001) docker     (123)   225794 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swecl.c
--rw-r--r--   0 runner    (1001) docker     (123)    29880 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweclips.c
--rw-r--r--   0 runner    (1001) docker     (123)    20063 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swedate.c
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swedate.h
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swedll.h
--rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swedllst.c
--rw-r--r--   0 runner    (1001) docker     (123)    22587 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweephe4.c
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweephe4.h
--rw-r--r--   0 runner    (1001) docker     (123)   123264 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swehel.c
--rw-r--r--   0 runner    (1001) docker     (123)   112151 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swehouse.c
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swehouse.h
--rw-r--r--   0 runner    (1001) docker     (123)    33480 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swejpl.c
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swejpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swemini.c
--rw-r--r--   0 runner    (1001) docker     (123)    61388 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swemmoon.c
--rw-r--r--   0 runner    (1001) docker     (123)    27880 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swemplan.c
--rw-r--r--   0 runner    (1001) docker     (123)   311984 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swemptab.h
--rw-r--r--   0 runner    (1001) docker     (123)    68486 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swenut2000a.h
--rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweodef.h
--rw-r--r--   0 runner    (1001) docker     (123)   290642 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweph.c
--rw-r--r--   0 runner    (1001) docker     (123)    34361 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/sweph.h
--rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swephexp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swephgen4.c
--rw-r--r--   0 runner    (1001) docker     (123)   164395 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swephlib.c
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swephlib.h
--rw-r--r--   0 runner    (1001) docker     (123)   144165 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swetest.c
--rw-r--r--   0 runner    (1001) docker     (123)    93650 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swevents.c
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swevents.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.360454 pyswisseph-2.10.3.2/libswe/swewin/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swewin/resource.h
--rw-r--r--   0 runner    (1001) docker     (123)    42674 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swewin/swewin.c
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swewin/swewin.h
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/libswe/swewin/swewin.rc
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/libswe/swewin/swewin64.c
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/libswe/swewin/swewin64.h
--rw-r--r--   0 runner    (1001) docker     (123)   268390 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/pyswisseph.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.364454 pyswisseph-2.10.3.2/pyswisseph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-04 16:49:22.000000 pyswisseph-2.10.3.2/pyswisseph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15915 2023-06-04 16:49:22.000000 pyswisseph-2.10.3.2/pyswisseph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:49:22.000000 pyswisseph-2.10.3.2/pyswisseph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 16:49:22.000000 pyswisseph-2.10.3.2/pyswisseph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:49:22.392454 pyswisseph-2.10.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.368454 pyswisseph-2.10.3.2/swephelp/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-04 16:49:13.000000 pyswisseph-2.10.3.2/swephelp/.git
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/makeatlas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.380454 pyswisseph-2.10.3.2/swephelp/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/.git
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   734131 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/shell.c
--rw-r--r--   0 runner    (1001) docker     (123)  8546396 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/sqlite3.c
--rw-r--r--   0 runner    (1001) docker     (123)   613416 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/sqlite3.h
--rw-r--r--   0 runner    (1001) docker     (123)    37310 2023-06-04 16:49:15.000000 pyswisseph-2.10.3.2/swephelp/sqlite3/sqlite3ext.h
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swephelp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhaspect.c
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhaspect.h
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhatlas.c
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhatlas.h
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdatetime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdatetime.h
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdb.c
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdb.h
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdbxx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdbxx.h
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdbxx.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhdef.h
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhformat.c
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhformat.h
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhgeo.c
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhgeo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhmisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhmisc.h
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhraman.c
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhraman.h
--rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhsearch.h
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhtimezone.c
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhtimezone.h
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhwin.h
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhxx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhxx.h
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-04 16:49:14.000000 pyswisseph-2.10.3.2/swephelp/swhxx.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:22.392454 pyswisseph-2.10.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_azalt_refrac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_calc_pctr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_calc_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_close.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_cotrans.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_cotrans_sp.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_cs2degstr.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_cs2lonlatstr.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_cs2timestr.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_csnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_csroundsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_d2l.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_date_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_deg_midp.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_degnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_deltat.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_deltat_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_difcs2n.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_difcsn.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_difdeg2n.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_difdegn.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_difrad2n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_fixstar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_fixstar2.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_fixstar2_mag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_fixstar2_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_fixstar_mag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_fixstar_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_gauquelin_sector.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_ayanamsa.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_ayanamsa_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_ayanamsa_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_current_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_library_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_orbital_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_planet_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_get_tid_acc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_heliacal_pheno_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_heliacal_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_helio_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_helio_cross_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_house_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_house_pos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_houses.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_houses_armc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_houses_armc_ex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_houses_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_houses_ex2.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_jdet_to_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_jdut1_to_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_julday.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_lat_to_lmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_lmt_to_lat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_lun_eclipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_lun_occult.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_pheno.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_pheno_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_rad_midp.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_radnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_revjul.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_rise_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_rise_trans_true_hor.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_set_delta_t_userdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_set_ephe_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_set_jpl_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_set_sid_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_set_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_sidtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_sidtime0.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_sol_eclipse.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_solcross.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_solcross_ut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_split_deg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_tid_acc.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_time_equ.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_utc_time_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_utc_to_jd.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-04 16:49:11.000000 pyswisseph-2.10.3.2/tests/test_swe_vis_limit_mag.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.865535 pyswisseph-2.10.3.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-09-19 18:20:28.865535 pyswisseph-2.10.3.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.737535 pyswisseph-2.10.3.2.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.737535 pyswisseph-2.10.3.2.dev1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/_static/.placeholder
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.737535 pyswisseph-2.10.3.2.dev1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/_templates/.placeholder
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/apparent_vs_true_planetary_positions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11795 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/delta_t.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.741535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.741535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/asteroid_99942_apophis.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/asteroid_ephemeris_files.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/ceres_an_application_for_asteroid_astrology.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/ceres_pallas_juno_vesta.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/chiron.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/how_the_asteroids_were_computed.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/pholus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/comets_and_interstellar_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/fixed_stars_and_galactic_center.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.741535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/harrington.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/nibiru.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/selena_white_moon.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/the_planets_x.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/transpluto_isis.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/uranian_planets.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/vulcan.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/waldemath_black_moon.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.741535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/interpolated_or_natural_apogee_and_perigee.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3390 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/mean_lunar_node_and_mean_lunar_apogee.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/osculating_apogee.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12238 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/planetary_nodes_and_apsides.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/true_node.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.741535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/
+-rw-r--r--   0 runner    (1001) docker     (121)     5984 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/comparisons_with_aa_and_jpl.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/compression_mechanism.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/details_of_coordinate_transformation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4166 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/extension_of_de406_based_ephemerides.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/solar_ephemeris_in_the_remote_past.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.745535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5515 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/jpl_ephemeris.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/moshier_ephemeris.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7337 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/swiss_ephemeris.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_centers_of_body_and_planetary_moons.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.745535 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/
+-rw-r--r--   0 runner    (1001) docker     (121)    13229 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/ayanamshas_with_different_precession_rates.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/babylonian_tradition_and_fagan_bradley_ayanamsha.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/conclusions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/defining_the_zodiac.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5488 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/hipparchan_tradition.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21431 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/image002.png
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5042 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/krishnamurti_ayanamshas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    18857 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/on_which_ecliptic_is_the_ayanamsha_measured.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9026 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/other_ayanamshas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5945 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_center.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4521 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_equator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12026 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/spica_citra_tradition_and_lahiri_ayanamsha.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/standard_equinoxes_and_precession_corrected_transits.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5424 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/suryasiddhanta_and_aryabhata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/geo_topo_helio_bary_and_planetocentric_positions.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.745535 pyswisseph-2.10.3.2.dev1/docs/heliacal_events_eclipses_occultations_etc/
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/heliacal_events_eclipses_occultations_etc/eclipses_occultations_risings_settings_etc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/heliacal_events_eclipses_occultations_etc/heliacal_events_of_the_moon_planets_and_stars.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/heliacal_events_eclipses_occultations_etc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    43055 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/image001.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.749535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.753535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/apsides_nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/distances.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/kepler_elements.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    70777 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/cmake01.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/crossings_of_planets_over_positions.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.753535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/calendar_date_and_julian_day.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/datetime_example1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/datetime_example2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/delta_t.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/handling_of_leap_seconds.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/mean_solar_time_vs_true_solar_time.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/seleapsec.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/swe_deltat.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/utc_and_julian_day.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3726 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/ephemeris_related_functions.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.753535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/different_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/fixed_stars_magnitude.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/fixed_stars_positions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   133990 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/sefstars.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6282 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/house_cusp_calculation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/house_position_of_a_planet.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3594 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/other_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/placalc_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planet_name.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.753535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/attributes_of_lunar_eclipse.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/attributes_of_occultation_by_the_moon.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/attributes_of_solar_eclipse.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/ecliptical_or_equatorial_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/example.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/example.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/find_position_of_maximal_eclipse.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/heliacal_details.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/heliacal_risings_and_settings.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/horizontal_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/magnitude_limit_for_visibility.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_lunar_eclipse_for_given_position.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_lunar_eclipse_globally.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_occultation_by_the_moon_for_given_position.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_occultation_by_the_moon_globally.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_solar_eclipse_for_given_position.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_solar_eclipse_globally.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/phase_elongation_diameter_magnitude.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/refraction.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5486 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/risings_settings_meridian_transits.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/sunrise.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.753535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.757535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/
+-rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/additional_asteroids.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/fictitious_planets.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/obliquity_and_nutation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/planetary_moons_and_body_centers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/seorbel.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/call_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/error_handling_and_return_values.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.761535 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/coordinate_systems.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/ephemeris_flags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/specialities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/speed_flags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/the_use_of_flag_bits.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/position_and_speed.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/seasnam2_sample.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/seasnam_sample.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10043 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/sidereal_mode.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/sidereal_time.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/sign_of_geographical_longitudes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/steps_to_get_a_planets_position.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/swemini.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/programmers_manual/topocentric_planet_positions.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.761535 pyswisseph-2.10.3.2.dev1/docs/sidereal_time_ascendant_mc_houses_vertex/
+-rw-r--r--   0 runner    (1001) docker     (121)    31435 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/sidereal_time_ascendant_mc_houses_vertex/astrological_house_systems.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/sidereal_time_ascendant_mc_houses_vertex/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      857 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/docs/sidereal_time_ascendant_mc_houses_vertex/sidereal_time.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.769535 pyswisseph-2.10.3.2.dev1/libswe/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 18:20:21.000000 pyswisseph-2.10.3.2.dev1/libswe/.git
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.769535 pyswisseph-2.10.3.2.dev1/libswe/contrib/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      393 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/contrib/mirror_ephedir.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.769535 pyswisseph-2.10.3.2.dev1/libswe/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.781535 pyswisseph-2.10.3.2.dev1/libswe/doc/media/
+-rw-r--r--   0 runner    (1001) docker     (121)    78370 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image1.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6818 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image10.png
+-rw-r--r--   0 runner    (1001) docker     (121)    42250 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image11.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image12.png
+-rw-r--r--   0 runner    (1001) docker     (121)   150205 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image13.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8799 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image14.png
+-rw-r--r--   0 runner    (1001) docker     (121)    10943 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image15.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8384 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8192 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image17.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6037 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image18.png
+-rw-r--r--   0 runner    (1001) docker     (121)    26775 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image19.png
+-rw-r--r--   0 runner    (1001) docker     (121)    36536 2022-09-19 18:20:23.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image2.png
+-rw-r--r--   0 runner    (1001) docker     (121)   105074 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image20.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14555 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image21.png
+-rw-r--r--   0 runner    (1001) docker     (121)    48008 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image22.png
+-rw-r--r--   0 runner    (1001) docker     (121)    42926 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image23.png
+-rw-r--r--   0 runner    (1001) docker     (121)    25802 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image24.png
+-rw-r--r--   0 runner    (1001) docker     (121)    26084 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image25.png
+-rw-r--r--   0 runner    (1001) docker     (121)    10028 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image26.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image27.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image28.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image29.png
+-rw-r--r--   0 runner    (1001) docker     (121)    28809 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image3.png
+-rw-r--r--   0 runner    (1001) docker     (121)    10645 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image30.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5151 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image31.png
+-rw-r--r--   0 runner    (1001) docker     (121)    11269 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image32.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image33.png
+-rw-r--r--   0 runner    (1001) docker     (121)    20037 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image34.png
+-rw-r--r--   0 runner    (1001) docker     (121)    19800 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image35.png
+-rw-r--r--   0 runner    (1001) docker     (121)    61456 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image36.png
+-rw-r--r--   0 runner    (1001) docker     (121)    54484 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image37.jpeg
+-rw-r--r--   0 runner    (1001) docker     (121)   837343 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image38.png
+-rw-r--r--   0 runner    (1001) docker     (121)    92198 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image39.png
+-rw-r--r--   0 runner    (1001) docker     (121)    10922 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image4.png
+-rw-r--r--   0 runner    (1001) docker     (121)    53347 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image40.png
+-rw-r--r--   0 runner    (1001) docker     (121)    16609 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image5.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7339 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image6.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6869 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image7.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2930 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image8.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/media/image9.png
+-rw-r--r--   0 runner    (1001) docker     (121)   267146 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/swephprg.md
+-rw-r--r--   0 runner    (1001) docker     (121)   287589 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/doc/swisseph.md
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sedeltat.txt.inactive
+-rw-r--r--   0 runner    (1001) docker     (121)   134182 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sefstars.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/seleapsec.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5845 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/seorbel.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.809535 pyswisseph-2.10.3.2.dev1/libswe/setest/
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/checkpoints.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/checkpoints.h
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/cmd.gdb
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/constants.c
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/gen_fix_templ.m4
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/generate_prepare_fix_m4.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1692 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/generate_prepare_fix_m4a.pl
+-rw-r--r--   0 runner    (1001) docker     (121)    53872 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/generated_tests.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/globals.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/globals.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/globals_suite.c
+-rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/multivalues.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/multivalues.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8592 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/mytest.fix
+-rw-r--r--   0 runner    (1001) docker     (121)    11739 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/prepare_fix.m4
+-rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/reader.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/reader.h
+-rw-r--r--   0 runner    (1001) docker     (121)    15859 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/setest.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/setest.h
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/setest.help
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/setest.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_01_calc.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_02_fixstar.c
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_03_misc.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_04_ayanamsa.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_05_date_time.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_06_houses.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_07_apsides.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2901 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_08_eclipses.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_09_rise.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/suite_10_solcross.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.809535 pyswisseph-2.10.3.2.dev1/libswe/setest/t/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      363 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t/test
+-rwxr-xr-x   0 runner    (1001) docker     (121)      621 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t/test.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)      363 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t/test.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t/test_dummy.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1068 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t/test_mytest_ok.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      683 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t/test_read_section.sh
+-rw-r--r--   0 runner    (1001) docker     (121) 12977948 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t.exp
+-rw-r--r--   0 runner    (1001) docker     (121)    21457 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/t.fix
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/test_one_per_process.pl
+-rw-r--r--   0 runner    (1001) docker     (121)     5574 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testdata.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testdata.h
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testdata.s
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testsuite.m4
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testsuite_end.m4
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testsuite_facade.h
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/setest/testsuite_final.h
+-rw-r--r--   0 runner    (1001) docker     (121)    63177 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweasp.c
+-rw-r--r--   0 runner    (1001) docker     (121)   225794 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swecl.c
+-rw-r--r--   0 runner    (1001) docker     (121)    29880 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweclips.c
+-rw-r--r--   0 runner    (1001) docker     (121)    20063 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swedate.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swedate.h
+-rw-r--r--   0 runner    (1001) docker     (121)    17333 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swedll.h
+-rw-r--r--   0 runner    (1001) docker     (121)    20722 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swedllst.c
+-rw-r--r--   0 runner    (1001) docker     (121)    22587 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweephe4.c
+-rw-r--r--   0 runner    (1001) docker     (121)     9817 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweephe4.h
+-rw-r--r--   0 runner    (1001) docker     (121)   123264 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swehel.c
+-rw-r--r--   0 runner    (1001) docker     (121)   112151 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swehouse.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swehouse.h
+-rw-r--r--   0 runner    (1001) docker     (121)    33480 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swejpl.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swejpl.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swemini.c
+-rw-r--r--   0 runner    (1001) docker     (121)    61388 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swemmoon.c
+-rw-r--r--   0 runner    (1001) docker     (121)    27880 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swemplan.c
+-rw-r--r--   0 runner    (1001) docker     (121)   311984 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swemptab.h
+-rw-r--r--   0 runner    (1001) docker     (121)    68486 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swenut2000a.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10838 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweodef.h
+-rw-r--r--   0 runner    (1001) docker     (121)   290642 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweph.c
+-rw-r--r--   0 runner    (1001) docker     (121)    34361 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/sweph.h
+-rw-r--r--   0 runner    (1001) docker     (121)    40932 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swephexp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9413 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swephgen4.c
+-rw-r--r--   0 runner    (1001) docker     (121)   164395 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swephlib.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7786 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swephlib.h
+-rw-r--r--   0 runner    (1001) docker     (121)   144165 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swetest.c
+-rw-r--r--   0 runner    (1001) docker     (121)    93650 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swevents.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swevents.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.813535 pyswisseph-2.10.3.2.dev1/libswe/swewin/
+-rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swewin/resource.h
+-rw-r--r--   0 runner    (1001) docker     (121)    42674 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin.rc
+-rw-r--r--   0 runner    (1001) docker     (121)    42241 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin64.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin64.h
+-rw-r--r--   0 runner    (1001) docker     (121)   268390 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/pyswisseph.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.813535 pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-09-19 18:20:28.000000 pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15915 2022-09-19 18:20:28.000000 pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 18:20:28.000000 pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-19 18:20:28.000000 pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 18:20:28.865535 pyswisseph-2.10.3.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.829535 pyswisseph-2.10.3.2.dev1/swephelp/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-19 18:20:22.000000 pyswisseph-2.10.3.2.dev1/swephelp/.git
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13224 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/makeatlas.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.837535 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/.git
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)   734131 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/shell.c
+-rw-r--r--   0 runner    (1001) docker     (121)  8546396 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/sqlite3.c
+-rw-r--r--   0 runner    (1001) docker     (121)   613416 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/sqlite3.h
+-rw-r--r--   0 runner    (1001) docker     (121)    37310 2022-09-19 18:20:25.000000 pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/sqlite3ext.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swephelp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhaspect.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhaspect.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhatlas.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhatlas.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdatetime.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdatetime.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7310 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdb.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdb.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13513 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdbxx.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdbxx.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdbxx.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4026 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhdef.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhformat.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhformat.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5381 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhgeo.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhgeo.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhmisc.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhmisc.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7511 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhraman.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4788 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhraman.h
+-rw-r--r--   0 runner    (1001) docker     (121)    21980 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhsearch.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhsearch.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12959 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhtimezone.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhtimezone.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhwin.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhxx.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhxx.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-09-19 18:20:24.000000 pyswisseph-2.10.3.2.dev1/swephelp/swhxx.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:28.865535 pyswisseph-2.10.3.2.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_azalt_refrac.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_calc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_calc_pctr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_calc_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_close.py
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_cotrans.py
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_cotrans_sp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_cs2degstr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_cs2lonlatstr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_cs2timestr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_csnorm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_csroundsec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_d2l.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_date_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_deg_midp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_degnorm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_deltat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_deltat_ex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_difcs2n.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_difcsn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_difdeg2n.py
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_difdegn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_difrad2n.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar2_mag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar2_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar_mag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_gauquelin_sector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_ayanamsa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_ayanamsa_ex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_ayanamsa_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_current_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_library_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_orbital_elements.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_planet_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_get_tid_acc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_heliacal_pheno_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_heliacal_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_helio_cross.py
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_helio_cross_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_house_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_house_pos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_houses.py
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_armc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_armc_ex2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_ex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_ex2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_jdet_to_utc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_jdut1_to_utc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_julday.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_lat_to_lmt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_lmt_to_lat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_lun_eclipse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_lun_occult.py
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_pheno.py
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_pheno_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_rad_midp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_radnorm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_revjul.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_rise_trans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_rise_trans_true_hor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_set_delta_t_userdef.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_set_ephe_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_set_jpl_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_set_sid_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_set_topo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_sidtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_sidtime0.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_sol_eclipse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_solcross.py
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_solcross_ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_split_deg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_tid_acc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_time_equ.py
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_utc_time_zone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_utc_to_jd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-09-19 18:20:19.000000 pyswisseph-2.10.3.2.dev1/tests/test_swe_vis_limit_mag.py
```

### Comparing `pyswisseph-2.10.3.2/CMakeLists.txt` & `pyswisseph-2.10.3.2.dev1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/LICENSE.txt` & `pyswisseph-2.10.3.2.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/PKG-INFO` & `pyswisseph-2.10.3.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswisseph
-Version: 2.10.3.2
+Version: 2.10.3.2.dev1
 Summary: Python extension to the Swiss Ephemeris
 Home-page: https://astrorigin.com/pyswisseph
 Download-URL: https://pypi.org/project/pyswisseph
 Author: Stanislas Marquis
 Author-email: stan@astrorigin.com
 Keywords: Astrology Ephemeris Swisseph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyswisseph-2.10.3.2/README.rst` & `pyswisseph-2.10.3.2.dev1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     >>> print(xx[0])
     0.09843983166646618
 
 Links
 =====
 
 :Pyswisseph docs:       https://astrorigin.com/pyswisseph
+:Launchpad PPA:         https://launchpad.net/~astrorigin/+archive/ubuntu/python-swisseph
 :Python Package Index:  https://pypi.org/project/pyswisseph
 :AstroDienst:           https://www.astro.com/swisseph
 
 Source code
 ===========
 
 Clone the Github repository with command:
@@ -75,10 +76,10 @@
     env SE_EPHE_PATH="/usr/share/sweph/ephe" python3 setup.py test
 
 Credits
 =======
 
 Author: Stanislas Marquis <stan(at)astrorigin.com>
 
-PyPI/CI: Jonathan de Jong <jonathan(at)automatia.nl>
+PyPI maintainer (branch pypi): Jonathan de Jong <jonathan(at)automatia.nl>
 
 ..
```

### Comparing `pyswisseph-2.10.3.2/docs/Makefile` & `pyswisseph-2.10.3.2.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/apparent_vs_true_planetary_positions.rst` & `pyswisseph-2.10.3.2.dev1/docs/apparent_vs_true_planetary_positions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/conf.py` & `pyswisseph-2.10.3.2.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/delta_t.rst` & `pyswisseph-2.10.3.2.dev1/docs/delta_t.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/asteroids/asteroid_99942_apophis.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/asteroid_99942_apophis.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/asteroids/asteroid_ephemeris_files.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/asteroid_ephemeris_files.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/asteroids/ceres_an_application_for_asteroid_astrology.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/ceres_an_application_for_asteroid_astrology.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/asteroids/ceres_pallas_juno_vesta.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/ceres_pallas_juno_vesta.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/asteroids/how_the_asteroids_were_computed.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/asteroids/how_the_asteroids_were_computed.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/comets_and_interstellar_objects.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/comets_and_interstellar_objects.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/fixed_stars_and_galactic_center.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/fixed_stars_and_galactic_center.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/harrington.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/harrington.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/nibiru.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/nibiru.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/the_planets_x.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/the_planets_x.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/transpluto_isis.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/transpluto_isis.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/uranian_planets.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/uranian_planets.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/hypothetical_bodies/waldemath_black_moon.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/hypothetical_bodies/waldemath_black_moon.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/interpolated_or_natural_apogee_and_perigee.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/interpolated_or_natural_apogee_and_perigee.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/mean_lunar_node_and_mean_lunar_apogee.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/mean_lunar_node_and_mean_lunar_apogee.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/osculating_apogee.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/osculating_apogee.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/planetary_nodes_and_apsides.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/planetary_nodes_and_apsides.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/true_node.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/lunar_and_planetary_nodes_and_apsides/true_node.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/comparisons_with_aa_and_jpl.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/comparisons_with_aa_and_jpl.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/compression_mechanism.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/compression_mechanism.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/details_of_coordinate_transformation.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/details_of_coordinate_transformation.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/extension_of_de406_based_ephemerides.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/extension_of_de406_based_ephemerides.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/solar_ephemeris_in_the_remote_past.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/solar_ephemeris_in_the_remote_past.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/jpl_ephemeris.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/jpl_ephemeris.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/moshier_ephemeris.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/moshier_ephemeris.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_and_lunar/three_ephemerides/swiss_ephemeris.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_and_lunar/three_ephemerides/swiss_ephemeris.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/planetary_centers_of_body_and_planetary_moons.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/planetary_centers_of_body_and_planetary_moons.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/ayanamshas_with_different_precession_rates.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/ayanamshas_with_different_precession_rates.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/babylonian_tradition_and_fagan_bradley_ayanamsha.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/babylonian_tradition_and_fagan_bradley_ayanamsha.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/conclusions.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/conclusions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/defining_the_zodiac.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/defining_the_zodiac.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/hipparchan_tradition.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/hipparchan_tradition.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/image002.png` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/image002.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/krishnamurti_ayanamshas.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/krishnamurti_ayanamshas.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/on_which_ecliptic_is_the_ayanamsha_measured.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/on_which_ecliptic_is_the_ayanamsha_measured.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/other_ayanamshas.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/other_ayanamshas.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_center.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_center.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_equator.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/sidereal_zodiac_and_galactic_equator.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/spica_citra_tradition_and_lahiri_ayanamsha.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/spica_citra_tradition_and_lahiri_ayanamsha.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/standard_equinoxes_and_precession_corrected_transits.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/standard_equinoxes_and_precession_corrected_transits.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/ephemerides/sidereal/suryasiddhanta_and_aryabhata.rst` & `pyswisseph-2.10.3.2.dev1/docs/ephemerides/sidereal/suryasiddhanta_and_aryabhata.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/geo_topo_helio_bary_and_planetocentric_positions.rst` & `pyswisseph-2.10.3.2.dev1/docs/geo_topo_helio_bary_and_planetocentric_positions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/heliacal_events_eclipses_occultations_etc/eclipses_occultations_risings_settings_etc.rst` & `pyswisseph-2.10.3.2.dev1/docs/heliacal_events_eclipses_occultations_etc/eclipses_occultations_risings_settings_etc.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/heliacal_events_eclipses_occultations_etc/heliacal_events_of_the_moon_planets_and_stars.rst` & `pyswisseph-2.10.3.2.dev1/docs/heliacal_events_eclipses_occultations_etc/heliacal_events_of_the_moon_planets_and_stars.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/image001.png` & `pyswisseph-2.10.3.2.dev1/docs/image001.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/introduction.rst` & `pyswisseph-2.10.3.2.dev1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/make.bat` & `pyswisseph-2.10.3.2.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/apsides_nodes.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/apsides_nodes.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/distances.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/distances.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/kepler_elements.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/apsides_nodes_kepler_elements_orbital_periods/kepler_elements.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/cmake01.png` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/cmake01.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/crossings_of_planets_over_positions.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/crossings_of_planets_over_positions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/calendar_date_and_julian_day.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/calendar_date_and_julian_day.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/delta_t.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/delta_t.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/handling_of_leap_seconds.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/handling_of_leap_seconds.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/mean_solar_time_vs_true_solar_time.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/mean_solar_time_vs_true_solar_time.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/date_and_time/utc_and_julian_day.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/date_and_time/utc_and_julian_day.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/ephemeris_related_functions.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/ephemeris_related_functions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/different_functions.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/different_functions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/fixed_stars_magnitude.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/fixed_stars_magnitude.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/fixed_stars_positions.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/fixed_stars_positions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/fixed_stars/sefstars.txt` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/fixed_stars/sefstars.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/house_cusp_calculation.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/house_cusp_calculation.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/house_position_of_a_planet.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/house_position_of_a_planet.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/installation.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/installation.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/placalc_functions.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/placalc_functions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planet_name.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planet_name.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/attributes_of_occultation_by_the_moon.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/attributes_of_occultation_by_the_moon.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/example.py` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/example.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/find_position_of_maximal_eclipse.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/find_position_of_maximal_eclipse.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/heliacal_risings_and_settings.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/heliacal_risings_and_settings.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/next_solar_eclipse_globally.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/next_solar_eclipse_globally.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/phase_elongation_diameter_magnitude.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/phase_elongation_diameter_magnitude.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/refraction.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/refraction.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/risings_settings_meridian_transits.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/risings_settings_meridian_transits.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_phenomena/sunrise.py` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_phenomena/sunrise.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/additional_asteroids.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/additional_asteroids.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/fictitious_planets.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/fictitious_planets.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/obliquity_and_nutation.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/obliquity_and_nutation.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/planetary_moons_and_body_centers.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/planetary_moons_and_body_centers.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/bodies/seorbel.txt` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/bodies/seorbel.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/call_parameters.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/call_parameters.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/error_handling_and_return_values.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/error_handling_and_return_values.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/index.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/index.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/coordinate_systems.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/coordinate_systems.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/ephemeris_flags.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/ephemeris_flags.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/specialities.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/specialities.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/the_use_of_flag_bits.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/options_chosen_by_flag_bits/the_use_of_flag_bits.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/planetary_positions/position_and_speed.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/planetary_positions/position_and_speed.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/seasnam2_sample.txt` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/seasnam2_sample.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/seasnam_sample.txt` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/seasnam_sample.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/sidereal_mode.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/sidereal_mode.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/sidereal_time.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/sidereal_time.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/sign_of_geographical_longitudes.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/sign_of_geographical_longitudes.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/steps_to_get_a_planets_position.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/steps_to_get_a_planets_position.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/swemini.py` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/swemini.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/programmers_manual/topocentric_planet_positions.rst` & `pyswisseph-2.10.3.2.dev1/docs/programmers_manual/topocentric_planet_positions.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/sidereal_time_ascendant_mc_houses_vertex/astrological_house_systems.rst` & `pyswisseph-2.10.3.2.dev1/docs/sidereal_time_ascendant_mc_houses_vertex/astrological_house_systems.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/docs/sidereal_time_ascendant_mc_houses_vertex/sidereal_time.rst` & `pyswisseph-2.10.3.2.dev1/docs/sidereal_time_ascendant_mc_houses_vertex/sidereal_time.rst`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/CMakeLists.txt` & `pyswisseph-2.10.3.2.dev1/libswe/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/LICENSE` & `pyswisseph-2.10.3.2.dev1/libswe/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/Makefile` & `pyswisseph-2.10.3.2.dev1/libswe/Makefile`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/makefile` & `pyswisseph-2.10.3.2.dev1/libswe/doc/makefile`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image1.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image1.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image10.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image10.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image11.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image11.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image12.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image12.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image13.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image13.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image14.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image14.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image15.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image15.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image16.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image16.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image17.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image17.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image18.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image18.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image19.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image19.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image2.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image2.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image20.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image20.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image21.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image21.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image22.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image22.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image23.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image23.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image24.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image24.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image25.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image25.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image26.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image26.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image27.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image27.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image28.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image28.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image29.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image29.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image3.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image3.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image30.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image30.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image31.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image31.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image32.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image32.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image33.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image33.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image34.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image34.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image35.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image35.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image36.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image36.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image37.jpeg` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image37.jpeg`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image38.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image38.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image39.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image39.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image4.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image4.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image40.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image40.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image5.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image5.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image6.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image6.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image7.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image7.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image8.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image8.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/media/image9.png` & `pyswisseph-2.10.3.2.dev1/libswe/doc/media/image9.png`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/swephprg.md` & `pyswisseph-2.10.3.2.dev1/libswe/doc/swephprg.md`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/doc/swisseph.md` & `pyswisseph-2.10.3.2.dev1/libswe/doc/swisseph.md`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sefstars.txt` & `pyswisseph-2.10.3.2.dev1/libswe/sefstars.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/seorbel.txt` & `pyswisseph-2.10.3.2.dev1/libswe/seorbel.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/Makefile` & `pyswisseph-2.10.3.2.dev1/libswe/setest/Makefile`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/checkpoints.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/checkpoints.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/checkpoints.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/checkpoints.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/constants.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/constants.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/gen_fix_templ.m4` & `pyswisseph-2.10.3.2.dev1/libswe/setest/gen_fix_templ.m4`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/generate_prepare_fix_m4.pl` & `pyswisseph-2.10.3.2.dev1/libswe/setest/generate_prepare_fix_m4.pl`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/generate_prepare_fix_m4a.pl` & `pyswisseph-2.10.3.2.dev1/libswe/setest/generate_prepare_fix_m4a.pl`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/generated_tests.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/generated_tests.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/globals.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/globals.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/globals.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/globals.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/globals_suite.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/globals_suite.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/multivalues.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/multivalues.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/multivalues.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/multivalues.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/mytest.fix` & `pyswisseph-2.10.3.2.dev1/libswe/setest/mytest.fix`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/prepare_fix.m4` & `pyswisseph-2.10.3.2.dev1/libswe/setest/prepare_fix.m4`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/reader.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/reader.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/reader.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/reader.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/setest.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/setest.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/setest.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/setest.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/setest.help` & `pyswisseph-2.10.3.2.dev1/libswe/setest/setest.help`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/setest.md` & `pyswisseph-2.10.3.2.dev1/libswe/setest/setest.md`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_01_calc.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_01_calc.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_02_fixstar.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_02_fixstar.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_04_ayanamsa.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_04_ayanamsa.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_05_date_time.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_05_date_time.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_06_houses.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_06_houses.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_07_apsides.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_07_apsides.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_08_eclipses.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_08_eclipses.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_09_rise.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_09_rise.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/suite_10_solcross.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/suite_10_solcross.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/t/test.pl` & `pyswisseph-2.10.3.2.dev1/libswe/setest/t/test.pl`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/t/test_mytest_ok.sh` & `pyswisseph-2.10.3.2.dev1/libswe/setest/t/test_mytest_ok.sh`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/t/test_read_section.sh` & `pyswisseph-2.10.3.2.dev1/libswe/setest/t/test_read_section.sh`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/t.exp` & `pyswisseph-2.10.3.2.dev1/libswe/setest/t.exp`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/t.fix` & `pyswisseph-2.10.3.2.dev1/libswe/setest/t.fix`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/test_one_per_process.pl` & `pyswisseph-2.10.3.2.dev1/libswe/setest/test_one_per_process.pl`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/testdata.c` & `pyswisseph-2.10.3.2.dev1/libswe/setest/testdata.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/testdata.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/testdata.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/testsuite.m4` & `pyswisseph-2.10.3.2.dev1/libswe/setest/testsuite.m4`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/setest/testsuite_facade.h` & `pyswisseph-2.10.3.2.dev1/libswe/setest/testsuite_facade.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweasp.c` & `pyswisseph-2.10.3.2.dev1/libswe/sweasp.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swecl.c` & `pyswisseph-2.10.3.2.dev1/libswe/swecl.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweclips.c` & `pyswisseph-2.10.3.2.dev1/libswe/sweclips.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swedate.c` & `pyswisseph-2.10.3.2.dev1/libswe/swedate.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swedate.h` & `pyswisseph-2.10.3.2.dev1/libswe/swedate.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swedll.h` & `pyswisseph-2.10.3.2.dev1/libswe/swedll.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swedllst.c` & `pyswisseph-2.10.3.2.dev1/libswe/swedllst.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweephe4.c` & `pyswisseph-2.10.3.2.dev1/libswe/sweephe4.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweephe4.h` & `pyswisseph-2.10.3.2.dev1/libswe/sweephe4.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swehel.c` & `pyswisseph-2.10.3.2.dev1/libswe/swehel.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swehouse.c` & `pyswisseph-2.10.3.2.dev1/libswe/swehouse.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swehouse.h` & `pyswisseph-2.10.3.2.dev1/libswe/swehouse.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swejpl.c` & `pyswisseph-2.10.3.2.dev1/libswe/swejpl.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swejpl.h` & `pyswisseph-2.10.3.2.dev1/libswe/swejpl.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swemini.c` & `pyswisseph-2.10.3.2.dev1/libswe/swemini.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swemmoon.c` & `pyswisseph-2.10.3.2.dev1/libswe/swemmoon.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swemplan.c` & `pyswisseph-2.10.3.2.dev1/libswe/swemplan.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swemptab.h` & `pyswisseph-2.10.3.2.dev1/libswe/swemptab.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swenut2000a.h` & `pyswisseph-2.10.3.2.dev1/libswe/swenut2000a.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweodef.h` & `pyswisseph-2.10.3.2.dev1/libswe/sweodef.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweph.c` & `pyswisseph-2.10.3.2.dev1/libswe/sweph.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/sweph.h` & `pyswisseph-2.10.3.2.dev1/libswe/sweph.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swephexp.h` & `pyswisseph-2.10.3.2.dev1/libswe/swephexp.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swephgen4.c` & `pyswisseph-2.10.3.2.dev1/libswe/swephgen4.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swephlib.c` & `pyswisseph-2.10.3.2.dev1/libswe/swephlib.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swephlib.h` & `pyswisseph-2.10.3.2.dev1/libswe/swephlib.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swetest.c` & `pyswisseph-2.10.3.2.dev1/libswe/swetest.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swevents.c` & `pyswisseph-2.10.3.2.dev1/libswe/swevents.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swevents.h` & `pyswisseph-2.10.3.2.dev1/libswe/swevents.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swewin/resource.h` & `pyswisseph-2.10.3.2.dev1/libswe/swewin/resource.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swewin/swewin.c` & `pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swewin/swewin.h` & `pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swewin/swewin.rc` & `pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin.rc`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swewin/swewin64.c` & `pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin64.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/libswe/swewin/swewin64.h` & `pyswisseph-2.10.3.2.dev1/libswe/swewin/swewin64.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/pyswisseph.c` & `pyswisseph-2.10.3.2.dev1/pyswisseph.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 2f2a 0a20 2020 2054 6869 7320 6669 6c65  /*.    This file
 00000010: 2069 7320 7061 7274 206f 6620 5079 7377   is part of Pysw
 00000020: 6973 7365 7068 2e0a 0a20 2020 2043 6f70  isseph...    Cop
 00000030: 7972 6967 6874 2028 6329 2032 3030 372d  yright (c) 2007-
-00000040: 3230 3233 2053 7461 6e69 736c 6173 204d  2023 Stanislas M
+00000040: 3230 3232 2053 7461 6e69 736c 6173 204d  2022 Stanislas M
 00000050: 6172 7175 6973 203c 7374 616e 4061 7374  arquis <stan@ast
 00000060: 726f 7269 6769 6e2e 636f 6d3e 0a0a 2020  rorigin.com>..  
 00000070: 2020 5079 7377 6973 7365 7068 2069 7320    Pyswisseph is 
 00000080: 6672 6565 2073 6f66 7477 6172 653a 2079  free software: y
 00000090: 6f75 2063 616e 2072 6564 6973 7472 6962  ou can redistrib
 000000a0: 7574 6520 6974 2061 6e64 2f6f 7220 6d6f  ute it and/or mo
 000000b0: 6469 6679 0a20 2020 2069 7420 756e 6465  dify.    it unde
@@ -66,15 +66,15 @@
 00000410: 7365 7068 2068 6f6d 6570 6167 653a 2068  seph homepage: h
 00000420: 7474 7073 3a2f 2f77 7777 2e61 7374 726f  ttps://www.astro
 00000430: 2e63 6f6d 2f73 7769 7373 6570 680a 202a  .com/swisseph. *
 00000440: 0a20 2a20 2053 7769 7373 6570 6820 7665  . *  Swisseph ve
 00000450: 7273 696f 6e3a 2032 2e31 302e 3033 0a20  rsion: 2.10.03. 
 00000460: 2a2f 0a0a 2364 6566 696e 6520 5059 5357  */..#define PYSW
 00000470: 4953 5345 5048 5f56 4552 5349 4f4e 2020  ISSEPH_VERSION  
-00000480: 2020 2020 3230 3233 3036 3034 0a0a 2f2a      20230604../*
+00000480: 2020 2020 3230 3232 3039 3134 0a0a 2f2a      20220914../*
 00000490: 2053 6574 2074 6865 2064 6566 6175 6c74   Set the default
 000004a0: 2061 7267 756d 656e 7420 666f 7220 7365   argument for se
 000004b0: 745f 6570 6865 5f70 6174 6820 6675 6e63  t_ephe_path func
 000004c0: 7469 6f6e 202a 2f0a 2369 666e 6465 6620  tion */.#ifndef 
 000004d0: 5059 5357 455f 4445 4641 554c 545f 4550  PYSWE_DEFAULT_EP
 000004e0: 4845 5f50 4154 480a 2369 6664 6566 2057  HE_PATH.#ifdef W
 000004f0: 494e 3332 0a23 6465 6669 6e65 2050 5953  IN32.#define PYS
```

### Comparing `pyswisseph-2.10.3.2/pyswisseph.egg-info/PKG-INFO` & `pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswisseph
-Version: 2.10.3.2
+Version: 2.10.3.2.dev1
 Summary: Python extension to the Swiss Ephemeris
 Home-page: https://astrorigin.com/pyswisseph
 Download-URL: https://pypi.org/project/pyswisseph
 Author: Stanislas Marquis
 Author-email: stan@astrorigin.com
 Keywords: Astrology Ephemeris Swisseph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyswisseph-2.10.3.2/pyswisseph.egg-info/SOURCES.txt` & `pyswisseph-2.10.3.2.dev1/pyswisseph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/setup.py` & `pyswisseph-2.10.3.2.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #   This file is part of Pyswisseph.
 #
-#   Copyright (c) 2007-2023 Stanislas Marquis <stan@astrorigin.com>
+#   Copyright (c) 2007-2022 Stanislas Marquis <stan@astrorigin.com>
 #
 #   Pyswisseph is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU Affero General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   Pyswisseph is distributed in the hope that it will be useful,
@@ -63,15 +63,15 @@
 # and our increment as suffix (.X), plus an eventual pre-release tag (.devX).
 #
 # Note about Github Actions:
 # Each push tagged with vX.XX.XX.X triggers a stable release on PyPI.
 # Each push tagged with vX.XX.XX.X.devX triggers a pre-release on PyPI.
 # Do not forget to: increment version string right here, and modify file
 # pyswisseph.c (PYSWISSEPH_VERSION).
-VERSION = '2.10.03.2'
+VERSION = '2.10.03.2.dev1'
 
 # Corresponding swisseph version string (normalized for pkg-config)
 swe_version = '2.10.3'
 
 # Debian libswe-dev detection
 # Set to True to try and find libswe in system.
 # Set to False to use bundled libswe.
```

### Comparing `pyswisseph-2.10.3.2/swephelp/CMakeLists.txt` & `pyswisseph-2.10.3.2.dev1/swephelp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/LICENSE.txt` & `pyswisseph-2.10.3.2.dev1/swephelp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/Makefile` & `pyswisseph-2.10.3.2.dev1/swephelp/Makefile`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/makeatlas.py` & `pyswisseph-2.10.3.2.dev1/swephelp/makeatlas.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/sqlite3/CMakeLists.txt` & `pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/sqlite3/Makefile` & `pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/Makefile`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/sqlite3/shell.c` & `pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/shell.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/sqlite3/sqlite3.c` & `pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/sqlite3.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/sqlite3/sqlite3.h` & `pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/sqlite3.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/sqlite3/sqlite3ext.h` & `pyswisseph-2.10.3.2.dev1/swephelp/sqlite3/sqlite3ext.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swephelp.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swephelp.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhaspect.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhaspect.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhaspect.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhaspect.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhatlas.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhatlas.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhatlas.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhatlas.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdatetime.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdatetime.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdatetime.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdatetime.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdb.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdb.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdb.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdb.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdbxx.cpp` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdbxx.cpp`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdbxx.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdbxx.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdbxx.hpp` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdbxx.hpp`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhdef.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhdef.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhformat.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhformat.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhformat.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhformat.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhgeo.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhgeo.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhgeo.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhgeo.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhmisc.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhmisc.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhmisc.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhmisc.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhraman.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhraman.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhraman.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhraman.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhsearch.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhsearch.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhsearch.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhsearch.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhtimezone.c` & `pyswisseph-2.10.3.2.dev1/swephelp/swhtimezone.c`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhtimezone.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhtimezone.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhwin.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhwin.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhxx.cpp` & `pyswisseph-2.10.3.2.dev1/swephelp/swhxx.cpp`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhxx.h` & `pyswisseph-2.10.3.2.dev1/swephelp/swhxx.h`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/swephelp/swhxx.hpp` & `pyswisseph-2.10.3.2.dev1/swephelp/swhxx.hpp`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_azalt_refrac.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_azalt_refrac.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_calc.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_calc.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_calc_pctr.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_calc_pctr.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_calc_ut.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_calc_ut.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_cotrans.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_cotrans.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_cotrans_sp.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_cotrans_sp.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_cs2lonlatstr.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_cs2lonlatstr.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_cs2timestr.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_cs2timestr.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_csnorm.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_csnorm.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_date_conversion.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_date_conversion.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_fixstar.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_fixstar2.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar2.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_fixstar2_mag.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar2_mag.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_fixstar2_ut.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar2_ut.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_fixstar_mag.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar_mag.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_fixstar_ut.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_fixstar_ut.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_gauquelin_sector.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_gauquelin_sector.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_get_ayanamsa.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_get_ayanamsa.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_get_ayanamsa_ex.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_get_ayanamsa_ex.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_get_current_file_data.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_get_current_file_data.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_get_orbital_elements.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_get_orbital_elements.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_heliacal_pheno_ut.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_heliacal_pheno_ut.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_heliacal_ut.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_heliacal_ut.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_house_pos.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_house_pos.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_houses.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_houses.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_houses_armc.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_armc.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_houses_armc_ex2.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_armc_ex2.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_houses_ex.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_ex.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_houses_ex2.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_houses_ex2.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_jdut1_to_utc.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_jdut1_to_utc.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_lun_eclipse.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_lun_eclipse.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_lun_occult.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_lun_occult.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_pheno.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_pheno.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_pheno_ut.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_pheno_ut.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_rise_trans.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_rise_trans.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_rise_trans_true_hor.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_rise_trans_true_hor.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_set_delta_t_userdef.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_set_delta_t_userdef.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_set_sid_mode.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_set_sid_mode.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_set_topo.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_set_topo.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_sol_eclipse.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_sol_eclipse.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_split_deg.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_split_deg.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_tid_acc.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_tid_acc.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_version.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_version.py`

 * *Files identical despite different names*

### Comparing `pyswisseph-2.10.3.2/tests/test_swe_vis_limit_mag.py` & `pyswisseph-2.10.3.2.dev1/tests/test_swe_vis_limit_mag.py`

 * *Files identical despite different names*

