# Comparing `tmp/peegy-1.5.4.tar.gz` & `tmp/peegy-1.5.5.tar.gz`

## Comparing `peegy-1.5.4.tar` & `peegy-1.5.5.tar`

### file list

```diff
@@ -1,190 +1,191 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/.gitattributes
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 peegy-1.5.4/.gitlab-ci.yml
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.5.4/CONTRIBUTING.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.5.4/MANIFEST.in
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 peegy-1.5.4/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 peegy-1.5.4/requirements.txt
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.5.4/setup.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/README.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/__init__.py
--rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_abr_peak_detection.py
--rw-r--r--   0        0        0    17206 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_eog_removal_template_.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_peak_detection.py
--rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_peak_detection_bootstrap.py
--rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_peak_detection_filters.py
--rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_video.py
--rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_weighted_average.py
--rw-r--r--   0        0        0    10533 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_acc_weighted_vs_standard_average.py
--rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_dss_frequency_domain_bias_test.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_dss_time_domain_bias_test.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_f_test.py
--rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_ht2_test.py
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_ht2_test_weighted_average.py
--rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_no_layout.py
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_assr_phase_locking_value_test.py
--rw-r--r--   0        0        0    12558 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_ffr_artifact_removal.py
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_using_own_data_trials.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 peegy-1.5.4/examples/example_using_own_raw_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/__init__.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/channel_definitions.py
--rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/edf_bdf_reader.py
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/eegReaderAbstractClasses.py
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/eeg_definitions.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/events.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/definitions/tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/directories/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/directories/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/__init__.py
--rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/edf_bdf_reader.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/elipse_tools.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/generic_csv_reader.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/synergy_reader.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/xml_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/eeg/__init__.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/eeg/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/__init__.py
--rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/file_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/aep_gui/__init__.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
--rw-r--r--   0        0        0    11640 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/aep_gui/dataReadingTools.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/aep_gui/extsys_tools.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/storage/__init__.py
--rw-r--r--   0        0        0    12445 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/storage/data_storage_reading_tools.py
--rw-r--r--   0        0        0    17199 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/storage/data_storage_tools.py
--rw-r--r--   0        0        0    40696 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/io/storage/plot_tools.py
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/KIT-160.lay
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/__init__.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi128.lay
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi16.lay
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi160.lay
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi256.lay
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi32.lay
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi32_2_EXT.lay
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi32_fnirs_MP.lay
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi32_fnirs_jaime.lay
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi64.lay
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi64_2_EXT.lay
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/biosemi64_3_EXT.lay
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/emotive14.lay
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/layouts.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/layouts/neuroscan64.lay
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/plot/__init__.py
--rw-r--r--   0        0        0    45613 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/plot/eeg_ave_epochs_plot_tools.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/plot/eeg_plot_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/events/__init__.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/events/event_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/__init__.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/attach.py
--rw-r--r--   0        0        0    28572 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/definitions.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/detection.py
--rw-r--r--   0        0        0    34770 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/epochs.py
--rw-r--r--   0        0        0    33907 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/general.py
--rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/interpolation.py
--rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/io.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/pipeline.py
--rw-r--r--   0        0        0    16137 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/plot.py
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/regression.py
--rw-r--r--   0        0        0    24431 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/simulate.py
--rw-r--r--   0        0        0    39109 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/spatial_filtering.py
--rw-r--r--   0        0        0    27334 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/statistics.py
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/storage.py
--rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/time_frequency.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/bootstrap/__init__.py
--rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/pipe/bootstrap/bootstrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/statistics/__init__.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/statistics/definitions.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/statistics/eeg_statistic_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/system/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/system/memory.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/system/progress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/__init__.py
--rw-r--r--   0        0        0    21075 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/eeg_epoch_operators.py
--rw-r--r--   0        0        0    63759 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/epochs_processing_tools.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/math_tools.py
--rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/weightedAverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/detection/__init__.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/detection/definitions.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/detection/time_domain_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/__init__.py
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/eegFiltering.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/resampling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/eog_tools/__init__.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/eog_tools/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/spatial_filtering/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/spatial_filtering/definitions.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/fitting/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/fitting/fitting_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/multiprocessing/__init__.py
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/template_generator/__init__.py
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/template_generator/auditory_waveforms.py
--rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/template_generator/h0.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/video/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/processing/tools/video/recording.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/dss_unit_tests.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/eeg_test_resampling.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/javerager_test.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/peegy_test_phase_detection_morlet.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/peegy_test_read_layout.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/read_data_eclipse_test.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/read_data_test.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_assr_moving_average.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_average_spectrogram_power.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_biosemi_class.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_biosemi_reader.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_bootstraping.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_edf_reader.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_eeg_notch_filter.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_eog_removal_correlation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_eog_template_removal.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_eog_template_valderrama_20118.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_et_tools.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_filter.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_fir_filter_mt.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_fir_filter_ols.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_fiter_mt.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_freq_noise_estimation.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_freq_noise_estimation_plots.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_frequency_average_epochs.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_generic_reader.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_hotelling_t2.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_ica_average_epochs.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_multiprocessing.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_noise_generator.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_norm_corr.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_parse_processing_chain.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_peakdetection.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_phase_detection.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_phase_locking_value.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_pooled_freq_noise_estimation.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_scrolling.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_spatial_filtering_example1.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_spatial_filtering_example6.py
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_spatial_filtering_freq_domain.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_spatial_filtering_freq_domain_2.py
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_w_average_epochs.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_xml_to_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/artifact_removal/__init__.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/artifact_removal/ir_test.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/artifact_removal/regression_artifact_removal.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/artifact_removal/xcorr_artifact_removal.py
--rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/tools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/tools/aep_gui/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/tools/signal_generator/__init__.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/tools/signal_generator/noise_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/tools/units/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.5.4/peegy/tools/units/unit_tools.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.5.4/.gitignore
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.5.4/LICENSE.txt
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 peegy-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 peegy-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/.gitattributes
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 peegy-1.5.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.5.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.5.5/MANIFEST.in
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 peegy-1.5.5/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 peegy-1.5.5/requirements.txt
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.5.5/setup.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/README.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/__init__.py
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_abr_peak_detection.py
+-rw-r--r--   0        0        0    17206 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_eog_removal_template_.py
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_peak_detection.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_peak_detection_bootstrap.py
+-rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_peak_detection_filters.py
+-rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_video.py
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_weighted_average.py
+-rw-r--r--   0        0        0    10533 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_acc_weighted_vs_standard_average.py
+-rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_dss_frequency_domain_bias_test.py
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_dss_time_domain_bias_test.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_f_test.py
+-rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_ht2_test.py
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_ht2_test_weighted_average.py
+-rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_no_layout.py
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_assr_phase_locking_value_test.py
+-rw-r--r--   0        0        0    12558 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_ffr_artifact_removal.py
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_using_own_data_trials.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 peegy-1.5.5/examples/example_using_own_raw_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/channel_definitions.py
+-rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/edf_bdf_reader.py
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/eegReaderAbstractClasses.py
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/eeg_definitions.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/events.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/definitions/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/directories/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/directories/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/__init__.py
+-rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/edf_bdf_reader.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/elipse_tools.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/generic_csv_reader.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/synergy_reader.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/xml_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/eeg/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/eeg/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/__init__.py
+-rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/file_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
+-rw-r--r--   0        0        0    11640 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/aep_gui/dataReadingTools.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/aep_gui/extsys_tools.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/storage/__init__.py
+-rw-r--r--   0        0        0    12445 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/storage/data_storage_reading_tools.py
+-rw-r--r--   0        0        0    17199 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/storage/data_storage_tools.py
+-rw-r--r--   0        0        0    40696 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/io/storage/plot_tools.py
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/KIT-160.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi128.lay
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi16.lay
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi160.lay
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi256.lay
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi32.lay
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi32_2_EXT.lay
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi32_fnirs_MP.lay
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi32_fnirs_jaime.lay
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi64.lay
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi64_2_EXT.lay
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/biosemi64_3_EXT.lay
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/brainvision64.bvef
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/emotive14.lay
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/layouts.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/layouts/neuroscan64.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/plot/__init__.py
+-rw-r--r--   0        0        0    45613 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/plot/eeg_ave_epochs_plot_tools.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/plot/eeg_plot_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/events/__init__.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/events/event_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/__init__.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/attach.py
+-rw-r--r--   0        0        0    29074 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/definitions.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/detection.py
+-rw-r--r--   0        0        0    34770 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/epochs.py
+-rw-r--r--   0        0        0    33907 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/general.py
+-rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/interpolation.py
+-rw-r--r--   0        0        0    16995 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/io.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/pipeline.py
+-rw-r--r--   0        0        0    16137 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/plot.py
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/regression.py
+-rw-r--r--   0        0        0    24431 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/simulate.py
+-rw-r--r--   0        0        0    39109 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/spatial_filtering.py
+-rw-r--r--   0        0        0    27334 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/statistics.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/storage.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/time_frequency.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/bootstrap/__init__.py
+-rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/pipe/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/statistics/__init__.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/statistics/definitions.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/statistics/eeg_statistic_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/system/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/system/memory.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/system/progress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/__init__.py
+-rw-r--r--   0        0        0    21075 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/eeg_epoch_operators.py
+-rw-r--r--   0        0        0    63759 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/epochs_processing_tools.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/math_tools.py
+-rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/weightedAverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/detection/__init__.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/detection/definitions.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/detection/time_domain_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/__init__.py
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/eegFiltering.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/resampling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/eog_tools/__init__.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/eog_tools/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/spatial_filtering/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/spatial_filtering/definitions.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/fitting/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/fitting/fitting_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/multiprocessing/__init__.py
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/template_generator/__init__.py
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/template_generator/auditory_waveforms.py
+-rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/template_generator/h0.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/video/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/processing/tools/video/recording.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/dss_unit_tests.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/eeg_test_resampling.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/javerager_test.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/peegy_test_phase_detection_morlet.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/peegy_test_read_layout.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/read_data_eclipse_test.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/read_data_test.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_assr_moving_average.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_average_spectrogram_power.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_biosemi_class.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_biosemi_reader.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_bootstraping.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_edf_reader.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_eeg_notch_filter.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_eog_removal_correlation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_eog_template_removal.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_eog_template_valderrama_20118.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_et_tools.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_filter.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_fir_filter_mt.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_fir_filter_ols.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_fiter_mt.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_freq_noise_estimation.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_freq_noise_estimation_plots.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_frequency_average_epochs.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_generic_reader.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_hotelling_t2.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_ica_average_epochs.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_multiprocessing.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_noise_generator.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_norm_corr.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_parse_processing_chain.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_peakdetection.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_phase_detection.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_phase_locking_value.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_pooled_freq_noise_estimation.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_scrolling.py
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_spatial_filtering_example1.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_spatial_filtering_example6.py
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_spatial_filtering_freq_domain.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_spatial_filtering_freq_domain_2.py
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_w_average_epochs.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_xml_to_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/artifact_removal/__init__.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/artifact_removal/ir_test.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/artifact_removal/regression_artifact_removal.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/artifact_removal/xcorr_artifact_removal.py
+-rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/tools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/tools/signal_generator/__init__.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/tools/signal_generator/noise_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/tools/units/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.5.5/peegy/tools/units/unit_tools.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.5.5/.gitignore
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.5.5/LICENSE.txt
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 peegy-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 peegy-1.5.5/PKG-INFO
```

### Comparing `peegy-1.5.4/.gitlab-ci.yml` & `peegy-1.5.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/CODE_OF_CONDUCT.md` & `peegy-1.5.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/CONTRIBUTING.md` & `peegy-1.5.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/Readme.md` & `peegy-1.5.5/Readme.md`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/requirements.txt` & `peegy-1.5.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/setup.py` & `peegy-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_abr_peak_detection.py` & `peegy-1.5.5/examples/example_abr_peak_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,16 @@
 # %%
 # Lets see the output of the filter
 # --------------------------------------
 # First we generate a target signal, in this example, and auditory brainstem response (ABR).
 
 pipeline['time_filtered_data'].plot(plot_input=True,
                                     plot_output=True,
-                                    interactive=False)
+                                    interactive=False,
+                                    show_events=False)
 
 # %%
 # Processing pipe continue
 # ------------------------------
 # First we generate a target signal, in this example, and auditory brainstem response (ABR).
```

### Comparing `peegy-1.5.4/examples/example_acc_eog_removal_template_.py` & `peegy-1.5.5/examples/example_acc_eog_removal_template_.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_acc_peak_detection.py` & `peegy-1.5.5/examples/example_acc_peak_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 template_waveform, _ = aep(fs=fs, time_length=0.6)
 event_times = np.arange(0, 400.0, 4.0) * u.s
 reader = GenerateInputData(template_waveform=template_waveform,
                            fs=fs,
                            n_channels=n_channels,
                            mixing_matrix=np.diag(np.arange(n_channels))/n_channels,
                            layout_file_name='biosemi32.lay',
-                           snr=0.1,
+                           snr=0.05,
                            event_times=event_times,
                            event_code=1.0,
                            figures_subset_folder='acc_test',
                            include_eog_events=True,
                            noise_attenuation=3,
                            )
 reader.run()
```

### Comparing `peegy-1.5.4/examples/example_acc_peak_detection_bootstrap.py` & `peegy-1.5.5/examples/example_acc_peak_detection_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 .. _tut-acc-bootstrapping-pipeline-sim:
 
 ##################################
 ACC Standard analysis (Simulated)
 ##################################
 
-In this example we simulate an ACC response and detect the peaks using n standard pipeline.
+In this example we simulate an ACC response and detect the peaks using standard and bootstrapping methods.
 
 """
 # Enable below for interactive backend
 # import matplotlib
 # if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
 #    matplotlib.use('Qt5Agg')
 from peegy.processing.pipe.pipeline import PipePool
```

### Comparing `peegy-1.5.4/examples/example_acc_peak_detection_filters.py` & `peegy-1.5.5/examples/example_acc_peak_detection_filters.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_acc_video.py` & `peegy-1.5.5/examples/example_acc_video.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_acc_weighted_average.py` & `peegy-1.5.5/examples/example_acc_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_acc_weighted_vs_standard_average.py` & `peegy-1.5.5/examples/example_acc_weighted_vs_standard_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_dss_frequency_domain_bias_test.py` & `peegy-1.5.5/examples/example_assr_dss_frequency_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_dss_time_domain_bias_test.py` & `peegy-1.5.5/examples/example_assr_dss_time_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_f_test.py` & `peegy-1.5.5/examples/example_assr_f_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_ht2_test.py` & `peegy-1.5.5/examples/example_assr_ht2_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_ht2_test_weighted_average.py` & `peegy-1.5.5/examples/example_assr_ht2_test_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py` & `peegy-1.5.5/examples/example_assr_ht2_test_wrong_bias_frequnecy.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_no_layout.py` & `peegy-1.5.5/examples/example_assr_no_layout.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_assr_phase_locking_value_test.py` & `peegy-1.5.5/examples/example_assr_phase_locking_value_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_ffr_artifact_removal.py` & `peegy-1.5.5/examples/example_ffr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_using_own_data_trials.py` & `peegy-1.5.5/examples/example_using_own_data_trials.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/examples/example_using_own_raw_data.py` & `peegy-1.5.5/examples/example_using_own_raw_data.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/definitions/channel_definitions.py` & `peegy-1.5.5/peegy/definitions/channel_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/definitions/edf_bdf_reader.py` & `peegy-1.5.5/peegy/definitions/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/definitions/eegReaderAbstractClasses.py` & `peegy-1.5.5/peegy/definitions/eegReaderAbstractClasses.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/definitions/eeg_definitions.py` & `peegy-1.5.5/peegy/definitions/eeg_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/definitions/events.py` & `peegy-1.5.5/peegy/definitions/events.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/definitions/tables.py` & `peegy-1.5.5/peegy/definitions/tables.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/directories/tools.py` & `peegy-1.5.5/peegy/directories/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/edf_bdf_reader.py` & `peegy-1.5.5/peegy/io/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/elipse_tools.py` & `peegy-1.5.5/peegy/io/elipse_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/generic_csv_reader.py` & `peegy-1.5.5/peegy/io/generic_csv_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/synergy_reader.py` & `peegy-1.5.5/peegy/io/synergy_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/xml_tools.py` & `peegy-1.5.5/peegy/io/xml_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/eeg/reader.py` & `peegy-1.5.5/peegy/io/eeg/reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/external_tools/file_tools.py` & `peegy-1.5.5/peegy/io/external_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py` & `peegy-1.5.5/peegy/io/external_tools/aep_gui/aep_matlab_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/external_tools/aep_gui/dataReadingTools.py` & `peegy-1.5.5/peegy/io/external_tools/aep_gui/dataReadingTools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/external_tools/aep_gui/extsys_tools.py` & `peegy-1.5.5/peegy/io/external_tools/aep_gui/extsys_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py` & `peegy-1.5.5/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/storage/data_storage_reading_tools.py` & `peegy-1.5.5/peegy/io/storage/data_storage_reading_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/storage/data_storage_tools.py` & `peegy-1.5.5/peegy/io/storage/data_storage_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/io/storage/plot_tools.py` & `peegy-1.5.5/peegy/io/storage/plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/KIT-160.lay` & `peegy-1.5.5/peegy/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi128.lay` & `peegy-1.5.5/peegy/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi16.lay` & `peegy-1.5.5/peegy/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi160.lay` & `peegy-1.5.5/peegy/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi256.lay` & `peegy-1.5.5/peegy/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi32.lay` & `peegy-1.5.5/peegy/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi32_2_EXT.lay` & `peegy-1.5.5/peegy/layouts/biosemi32_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi32_fnirs_MP.lay` & `peegy-1.5.5/peegy/layouts/biosemi32_fnirs_MP.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi32_fnirs_jaime.lay` & `peegy-1.5.5/peegy/layouts/biosemi32_fnirs_jaime.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi64.lay` & `peegy-1.5.5/peegy/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi64_2_EXT.lay` & `peegy-1.5.5/peegy/layouts/biosemi64_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/biosemi64_3_EXT.lay` & `peegy-1.5.5/peegy/layouts/biosemi64_3_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/emotive14.lay` & `peegy-1.5.5/peegy/layouts/emotive14.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/layouts.py` & `peegy-1.5.5/peegy/layouts/layouts.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/layouts/neuroscan64.lay` & `peegy-1.5.5/peegy/layouts/neuroscan64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/plot/eeg_ave_epochs_plot_tools.py` & `peegy-1.5.5/peegy/plot/eeg_ave_epochs_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/plot/eeg_plot_tools.py` & `peegy-1.5.5/peegy/plot/eeg_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/events/event_tools.py` & `peegy-1.5.5/peegy/processing/events/event_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/attach.py` & `peegy-1.5.5/peegy/processing/pipe/attach.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/definitions.py` & `peegy-1.5.5/peegy/processing/pipe/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import gc
 import astropy.units as u
 import abc
 import matplotlib.pyplot as plt
 import numpy as np
 from tqdm import tqdm
 import pyqtgraph as pg
+import pyqtgraph.exporters
 import time
 pg.setConfigOption('leftButtonPan', False)
 
 
 class DataNode(object):
     """
     Core data object used to keep data. During the creation, it requires the sampling rate and the actual data.
@@ -430,28 +431,32 @@
         return
 
     def plot(self,
              plot_input: bool = False,
              plot_output: bool = True,
              ch_to_plot: [str] = None,
              interactive: bool = True,
+             show_events: bool = True,
              channels_offset: u.Quantity = None):
         """
         This method will plot data in the input and/or the output node.
         :param plot_input: bool indicating if input_node data should be plotted
         :param plot_output: bool indicating if output_node data should be plotted
         :param ch_to_plot: list of strings indicating the labels of the channels to be shown. If empty, all channels
         will be shown.
         :param interactive: boolean indicating if plot should be interactive or not
+        :param show_events: if True, events will be shown
+        :param channels_offset: offset in vertical units to separate channels in figure
         """
         win = plot_input_output_process(input_output_process=self,
                                         plot_input=plot_input,
                                         plot_output=plot_output,
                                         ch_to_plot=ch_to_plot,
                                         channels_offset=channels_offset,
+                                        show_events=show_events
                                         )
         out = InputOutputQtFigure(figure=win)
         if interactive:
             win.show()
             pg.QtGui.QGuiApplication.instance().exec_()
         return out
 
@@ -466,23 +471,26 @@
 
 
 def plot_input_output_process(input_output_process: InputOutputProcess = None,
                               plot_input: bool = False,
                               plot_output: bool = True,
                               ch_to_plot: [str] = None,
                               de_mean: bool = False,
+                              show_events: bool = True,
                               channels_offset: u.Quantity = None):
     """
     This method will plot data in the input and/or the output node.
     :param input_output_process: InputOutputProcess for which plot will be generated.
     :param plot_input: bool indicating if input_node data should be plotted
     :param plot_output: bool indicating if output_node data should be plotted
     :param ch_to_plot: list of strings indicating the labels of the channels to be shown. If empty, all channels
     will be shown.
     :param de_mean: if True, lines will be centred around the mean and then offset
+    :param show_events: if True, events will be shown
+    :param channels_offset: offset in vertical units to separate channels in figure
     """
     if not plot_input and not plot_output:
         return
     data_in = None
     if input_output_process.input_node is not None:
         data_in = copy.copy(input_output_process.input_node.data)
         name_in = input_output_process.input_process.name
@@ -545,15 +553,15 @@
                 data_in[:, _i, :] = data_in[:, _i, :] + offset * _pos
                 for _t in tqdm(range(data_in.shape[2]),
                                desc='Generating input plot per epochs for channel {:}'.format(_label)):
                     ax.plot(x_in, data_in[:, _i, _t], pen=_color, name=_name if _t == 0 else None)
                     pg.QtCore.QCoreApplication.processEvents()
             ax.addItem(text_item)
 
-            if input_output_process.input_node.events is not None:
+            if show_events and input_output_process.input_node.events is not None:
                 _codes = np.unique(input_output_process.input_node.events.get_events_code(include_bad_events=True))
                 for _code in _codes:
                     _events = input_output_process.input_node.events.get_events(code=_code, include_bad_events=True)
                     _good_events = np.array([])
                     _bad_events = np.array([])
                     for _ev in _events:
                         if _ev.bad_event:
@@ -596,15 +604,15 @@
                 data_out[:, _i, :] = data_out[:, _i, :] + offset * _pos
                 for _t in tqdm(range(data_out.shape[2]),
                                desc='Generating output plot per epochs for channel {:}'.format(_label)):
                     ax.plot(x_out, data_out[:, _i, _t], pen=_color, name=_name if _t == 0 else None)
                     pg.QtCore.QCoreApplication.processEvents()
 
             ax.addItem(text_item)
-            if input_output_process.output_node.events is not None:
+            if show_events and input_output_process.output_node.events is not None:
                 _codes = np.unique(input_output_process.output_node.events.get_events_code())
                 for _code in _codes:
                     _events = input_output_process.output_node.events.get_events(code=_code, include_bad_events=True)
                     _good_events = np.array([])
                     _bad_events = np.array([])
                     for _ev in _events:
                         if _ev.bad_event:
```

### Comparing `peegy-1.5.4/peegy/processing/pipe/detection.py` & `peegy-1.5.5/peegy/processing/pipe/detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/epochs.py` & `peegy-1.5.5/peegy/processing/pipe/epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/general.py` & `peegy-1.5.5/peegy/processing/pipe/general.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/interpolation.py` & `peegy-1.5.5/peegy/processing/pipe/interpolation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/io.py` & `peegy-1.5.5/peegy/processing/pipe/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,23 +140,23 @@
         self.file_paths = file_paths
         self.channels_idx = channels_idx
         self.ini_time = 0 * u.s
         self.end_time = np.Inf * u.s
         self.output_node = None
         self.layout_file_name = layout_file_name
         self.figures_subset_folder = figures_subset_folder
-        self.input_node = DataNode(fs=self.readers[0].fs,
-                                   domain=Domain.time,
-                                   layout=self.readers[0].default_layout,
-                                   paths=DirectoryPaths(file_path=self.readers[0].file_name,
-                                                        delete_all=False, delete_figures=False,
-                                                        figures_subset_folder=figures_subset_folder)
-                                   )
+        self.output_node = DataNode(fs=self.readers[0].fs,
+                                    domain=Domain.time,
+                                    layout=self.readers[0].default_layout,
+                                    paths=DirectoryPaths(file_path=self.readers[0].file_name,
+                                                         delete_all=False, delete_figures=False,
+                                                         figures_subset_folder=figures_subset_folder)
+                                    )
 
-    def run(self):
+    def transform_data(self):
         all_data = None
         all_events = None
         # sort readers by time
         _date_format = "%d.%m.%y/%H.%M.%S"
         dates = np.array([_reader._header['start_date'] + '/' + _reader._header['start_time'] for
                           _reader in self.readers])
         sorted_idx = np.argsort([datetime.datetime.strptime(_date, _date_format) for _date in dates])
@@ -240,24 +240,24 @@
         n_channels = self.data.shape[1]
         if channel_labels is None:
             [_ch.append(ChannelItem(label='CH_{:}'.format(i), idx=i)) for i in range(n_channels)]
         else:
             [_ch.append(ChannelItem(label=_label, idx=i)) for i, _label in
              zip(range(n_channels), channel_labels)]
         layout = np.array(_ch)
-        self.input_node = DataNode(fs=fs,
-                                   domain=Domain.time,
-                                   layout=layout,
-                                   paths=DirectoryPaths(file_path=self.figures_path,
-                                                        delete_all=False,
-                                                        delete_figures=False,
-                                                        figures_subset_folder=figures_subset_folder),
-                                   )
+        self.output_node = DataNode(fs=fs,
+                                    domain=Domain.time,
+                                    layout=layout,
+                                    paths=DirectoryPaths(file_path=self.figures_path,
+                                                         delete_all=False,
+                                                         delete_figures=False,
+                                                         figures_subset_folder=figures_subset_folder),
+                                    )
 
-    def run(self):
+    def transform_data(self):
         events = np.array([])
         if self.event_times is not None:
             for _ev in self.event_times:
                 events = np.append(events, SingleEvent(code=self.event_code,
                                                        time_pos=_ev,
                                                        dur=0))
         events = Events(events=np.array(events))
@@ -290,24 +290,24 @@
         """
         super(EclipseReader, self).__init__()
         self.header = None
         self.output_node = None
         self.buffer = buffer
         self.file_path = file_path
         self.figures_subset_folder = figures_subset_folder
-        self.input_node = DataNode(fs=None,
-                                   domain=Domain.time,
-                                   layout=None,
-                                   paths=DirectoryPaths(file_path=str(file_path),
-                                                        delete_all=False,
-                                                        delete_figures=False,
-                                                        figures_subset_folder=figures_subset_folder)
-                                   )
+        self.output_node = DataNode(fs=None,
+                                    domain=Domain.time,
+                                    layout=None,
+                                    paths=DirectoryPaths(file_path=str(file_path),
+                                                         delete_all=False,
+                                                         delete_figures=False,
+                                                         figures_subset_folder=figures_subset_folder)
+                                    )
 
-    def run(self):
+    def transform_data(self):
         events = np.array([])
         events = Events(events=np.array(events))
         header, data, data_buffer_a, data_buffer_b = parse_eclipse_data(
             file_name=self.file_path)
         if self.buffer == 'A':
             _data = data_buffer_a
             _ch = [ChannelItem(label='Buffer_A')]
```

### Comparing `peegy-1.5.4/peegy/processing/pipe/pipeline.py` & `peegy-1.5.5/peegy/processing/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/plot.py` & `peegy-1.5.5/peegy/processing/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/regression.py` & `peegy-1.5.5/peegy/processing/pipe/regression.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/simulate.py` & `peegy-1.5.5/peegy/processing/pipe/simulate.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/spatial_filtering.py` & `peegy-1.5.5/peegy/processing/pipe/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/statistics.py` & `peegy-1.5.5/peegy/processing/pipe/statistics.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/storage.py` & `peegy-1.5.5/peegy/processing/pipe/storage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/time_frequency.py` & `peegy-1.5.5/peegy/processing/pipe/time_frequency.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,23 +111,23 @@
         self.sample_interval = sample_interval
         self.spec_thresh = spec_thresh
         self.average_mode = average_mode
         self.method = method
         self.wavelet_type = wavelet_type
 
     def transform_data(self):
-        power, freqs = self.time_frequency_transformation(epochs=self.input_node.data,
-                                                          fs=self.input_node.fs,
-                                                          time_window=self.time_window,
-                                                          sample_interval=self.sample_interval,
-                                                          average_mode=self.average_mode,
-                                                          method=self.method,
-                                                          wavelet_type=self.wavelet_type
-                                                          )
-        self.output_node.data = power
+        magnitude, freqs = self.time_frequency_transformation(epochs=self.input_node.data,
+                                                              fs=self.input_node.fs,
+                                                              time_window=self.time_window,
+                                                              sample_interval=self.sample_interval,
+                                                              average_mode=self.average_mode,
+                                                              method=self.method,
+                                                              wavelet_type=self.wavelet_type
+                                                              )
+        self.output_node.data = magnitude
         self.output_node.y = freqs
         self.output_node.x = self.input_node.x
         self.output_node.domain = Domain.time_frequency
 
     @staticmethod
     def time_frequency_transformation(epochs: np.array = np.array([]),
                                       method='spectrogram',
```

### Comparing `peegy-1.5.4/peegy/processing/pipe/transform.py` & `peegy-1.5.5/peegy/processing/pipe/transform.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/pipe/bootstrap/bootstrap.py` & `peegy-1.5.5/peegy/processing/pipe/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/statistics/definitions.py` & `peegy-1.5.5/peegy/processing/statistics/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/statistics/eeg_statistic_tools.py` & `peegy-1.5.5/peegy/processing/statistics/eeg_statistic_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/system/progress.py` & `peegy-1.5.5/peegy/processing/system/progress.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/eeg_epoch_operators.py` & `peegy-1.5.5/peegy/processing/tools/eeg_epoch_operators.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/epochs_processing_tools.py` & `peegy-1.5.5/peegy/processing/tools/epochs_processing_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/weightedAverage.py` & `peegy-1.5.5/peegy/processing/tools/weightedAverage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/detection/definitions.py` & `peegy-1.5.5/peegy/processing/tools/detection/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/detection/time_domain_tools.py` & `peegy-1.5.5/peegy/processing/tools/detection/time_domain_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/filters/eegFiltering.py` & `peegy-1.5.5/peegy/processing/tools/filters/eegFiltering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/filters/resampling.py` & `peegy-1.5.5/peegy/processing/tools/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/filters/eog_tools/tools.py` & `peegy-1.5.5/peegy/processing/tools/filters/eog_tools/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/filters/spatial_filtering/definitions.py` & `peegy-1.5.5/peegy/processing/tools/filters/spatial_filtering/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py` & `peegy-1.5.5/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py` & `peegy-1.5.5/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/template_generator/auditory_waveforms.py` & `peegy-1.5.5/peegy/processing/tools/template_generator/auditory_waveforms.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/template_generator/h0.json` & `peegy-1.5.5/peegy/processing/tools/template_generator/h0.json`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/processing/tools/video/recording.py` & `peegy-1.5.5/peegy/processing/tools/video/recording.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/dss_unit_tests.py` & `peegy-1.5.5/peegy/test/dss_unit_tests.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/eeg_test_resampling.py` & `peegy-1.5.5/peegy/test/eeg_test_resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/javerager_test.py` & `peegy-1.5.5/peegy/test/javerager_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/peegy_test_phase_detection_morlet.py` & `peegy-1.5.5/peegy/test/peegy_test_phase_detection_morlet.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/read_data_eclipse_test.py` & `peegy-1.5.5/peegy/test/read_data_eclipse_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/read_data_test.py` & `peegy-1.5.5/peegy/test/read_data_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_assr_moving_average.py` & `peegy-1.5.5/peegy/test/test_assr_moving_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_average_spectrogram_power.py` & `peegy-1.5.5/peegy/test/test_average_spectrogram_power.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_biosemi_class.py` & `peegy-1.5.5/peegy/test/test_biosemi_class.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_biosemi_reader.py` & `peegy-1.5.5/peegy/test/test_biosemi_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_bootstraping.py` & `peegy-1.5.5/peegy/test/test_bootstraping.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_edf_reader.py` & `peegy-1.5.5/peegy/test/test_edf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_eeg_notch_filter.py` & `peegy-1.5.5/peegy/test/test_eeg_notch_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_eog_removal_correlation.py` & `peegy-1.5.5/peegy/test/test_eog_removal_correlation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_eog_template_removal.py` & `peegy-1.5.5/peegy/test/test_eog_template_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_eog_template_valderrama_20118.py` & `peegy-1.5.5/peegy/test/test_eog_template_valderrama_20118.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_et_tools.py` & `peegy-1.5.5/peegy/test/test_et_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_filter.py` & `peegy-1.5.5/peegy/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_fir_filter_mt.py` & `peegy-1.5.5/peegy/test/test_fir_filter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_fir_filter_ols.py` & `peegy-1.5.5/peegy/test/test_fir_filter_ols.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_fiter_mt.py` & `peegy-1.5.5/peegy/test/test_fiter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_freq_noise_estimation.py` & `peegy-1.5.5/peegy/test/test_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_freq_noise_estimation_plots.py` & `peegy-1.5.5/peegy/test/test_freq_noise_estimation_plots.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_frequency_average_epochs.py` & `peegy-1.5.5/peegy/test/test_frequency_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_hotelling_t2.py` & `peegy-1.5.5/peegy/test/test_hotelling_t2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_ica_average_epochs.py` & `peegy-1.5.5/peegy/test/test_ica_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_multiprocessing.py` & `peegy-1.5.5/peegy/test/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_noise_generator.py` & `peegy-1.5.5/peegy/test/test_noise_generator.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_norm_corr.py` & `peegy-1.5.5/peegy/test/test_norm_corr.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_peakdetection.py` & `peegy-1.5.5/peegy/test/test_peakdetection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_phase_detection.py` & `peegy-1.5.5/peegy/test/test_phase_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_phase_locking_value.py` & `peegy-1.5.5/peegy/test/test_phase_locking_value.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_pooled_freq_noise_estimation.py` & `peegy-1.5.5/peegy/test/test_pooled_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_scrolling.py` & `peegy-1.5.5/peegy/test/test_scrolling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_spatial_filtering_example1.py` & `peegy-1.5.5/peegy/test/test_spatial_filtering_example1.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_spatial_filtering_example6.py` & `peegy-1.5.5/peegy/test/test_spatial_filtering_example6.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_spatial_filtering_freq_domain.py` & `peegy-1.5.5/peegy/test/test_spatial_filtering_freq_domain.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_spatial_filtering_freq_domain_2.py` & `peegy-1.5.5/peegy/test/test_spatial_filtering_freq_domain_2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_w_average_epochs.py` & `peegy-1.5.5/peegy/test/test_w_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/artifact_removal/ir_test.py` & `peegy-1.5.5/peegy/test/artifact_removal/ir_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/artifact_removal/regression_artifact_removal.py` & `peegy-1.5.5/peegy/test/artifact_removal/regression_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/artifact_removal/xcorr_artifact_removal.py` & `peegy-1.5.5/peegy/test/artifact_removal/xcorr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat` & `peegy-1.5.5/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/tools/signal_generator/noise_functions.py` & `peegy-1.5.5/peegy/tools/signal_generator/noise_functions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/peegy/tools/units/unit_tools.py` & `peegy-1.5.5/peegy/tools/units/unit_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/LICENSE.txt` & `peegy-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.5.4/pyproject.toml` & `peegy-1.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel", "hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 #build-backend = "setuptools.build_meta"
 
 [project]
 name = "peegy"
-version = "1.5.4"
+version = "1.5.5"
 authors = [{name = "Jaime Undurraga", email = "jaime.undurraga@gmail.com"},]
 description = "Tools to pipeline bulk analyses of EEG and other modalities."
 requires-python = ">=3.9"
 license = {text = "MIT"}
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Bio-Informatics"]
-
-dynamic = ["dependencies", "readme"]
+dynamic = ["dependencies"]
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"]}
 
+
 [project.urls]
 "Homepage" = "https://gitlab.com/open-source-brain/peegy/"
 "Examples" = "https://open-source-brain.gitlab.io/peegy/"
 
 
 [tool.setuptools]
 include-package-data = false
```

### Comparing `peegy-1.5.4/PKG-INFO` & `peegy-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: peegy
-Version: 1.5.4
+Version: 1.5.5
 Summary: Tools to pipeline bulk analyses of EEG and other modalities.
 Project-URL: Homepage, https://gitlab.com/open-source-brain/peegy/
 Project-URL: Examples, https://open-source-brain.gitlab.io/peegy/
 Author-email: Jaime Undurraga <jaime.undurraga@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
```

