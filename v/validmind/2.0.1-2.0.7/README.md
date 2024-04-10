# Comparing `tmp/validmind-2.0.1.tar.gz` & `tmp/validmind-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validmind-2.0.1.tar", max compression
+gzip compressed data, was "validmind-2.0.7.tar", max compression
```

## Comparing `validmind-2.0.1.tar` & `validmind-2.0.7.tar`

### file list

```diff
@@ -1,259 +1,279 @@
--rw-r--r--   0        0        0    35772 2024-03-27 20:36:59.783765 validmind-2.0.1/LICENSE
--rw-r--r--   0        0        0      790 2024-03-27 20:36:59.783765 validmind-2.0.1/README.pypi.md
--rw-r--r--   0        0        0     2455 2024-03-27 20:37:00.191768 validmind-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3627 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/__init__.py
--rw-r--r--   0        0        0       22 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/__version__.py
--rw-r--r--   0        0        0    14990 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/api_client.py
--rw-r--r--   0        0        0    16059 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/client.py
--rw-r--r--   0        0        0     1611 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/client_config.py
--rw-r--r--   0        0        0      262 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/datasets/__init__.py
--rw-r--r--   0        0        0     1787 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/datasets/classification/__init__.py
--rw-r--r--   0        0        0     3771 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/datasets/classification/customer_churn.py
--rw-r--r--   0        0        0   545707 2024-03-27 20:37:00.195767 validmind-2.0.1/validmind/datasets/classification/datasets/bank_customer_churn.csv
--rw-r--r--   0        0        0  2897191 2024-03-27 20:37:00.211768 validmind-2.0.1/validmind/datasets/classification/datasets/taiwan_credit.csv
--rw-r--r--   0        0        0     1469 2024-03-27 20:37:00.211768 validmind-2.0.1/validmind/datasets/classification/taiwan_credit.py
--rw-r--r--   0        0        0     2097 2024-03-27 20:37:00.211768 validmind-2.0.1/validmind/datasets/cluster/digits.py
--rw-r--r--   0        0        0      262 2024-03-27 20:37:00.211768 validmind-2.0.1/validmind/datasets/nlp/__init__.py
--rw-r--r--   0        0        0 11545066 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/nlp/datasets/Covid_19.csv
--rw-r--r--   0        0        0      878 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/nlp/twitter_covid_19.py
--rw-r--r--   0        0        0     1653 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/__init__.py
--rw-r--r--   0        0        0     1046 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/california_housing.py
--rw-r--r--   0        0        0    15834 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/CPIAUCSL.csv
--rw-r--r--   0        0        0     9105 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/CSUSHPISA.csv
--rw-r--r--   0        0        0     2093 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/DRSFRMACBS.csv
--rw-r--r--   0        0        0    13274 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/FEDFUNDS.csv
--rw-r--r--   0        0        0     6061 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/GDP.csv
--rw-r--r--   0        0        0     6201 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/GDPC1.csv
--rw-r--r--   0        0        0    13538 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/GS10.csv
--rw-r--r--   0        0        0    13506 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/GS3.csv
--rw-r--r--   0        0        0    13514 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/GS5.csv
--rw-r--r--   0        0        0    44040 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/MORTGAGE30US.csv
--rw-r--r--   0        0        0    13572 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred/UNRATE.csv
--rw-r--r--   0        0        0   107835 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates.csv
--rw-r--r--   0        0        0     2634 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
--rw-r--r--   0        0        0     2634 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
--rw-r--r--   0        0        0     2736 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
--rw-r--r--   0        0        0     3355 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
--rw-r--r--   0        0        0     3866 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
--rw-r--r--   0        0        0    11624 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
--rw-r--r--   0        0        0     5707 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/fred.py
--rw-r--r--   0        0        0     2536 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/lending_club.py
--rw-r--r--   0        0        0    40067 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
--rw-r--r--   0        0        0    48314 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
--rw-r--r--   0        0        0    40063 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
--rw-r--r--   0        0        0    48292 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
--rw-r--r--   0        0        0    60343 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
--rw-r--r--   0        0        0     7763 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/errors.py
--rw-r--r--   0        0        0     1607 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/html_templates/content_blocks.py
--rw-r--r--   0        0        0      793 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/input_registry.py
--rw-r--r--   0        0        0     4808 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/logging.py
--rw-r--r--   0        0        0      623 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/__init__.py
--rw-r--r--   0        0        0     1036 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/catboost.py
--rw-r--r--   0        0        0     2269 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/foundation.py
--rw-r--r--   0        0        0     2863 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/huggingface.py
--rw-r--r--   0        0        0     2575 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/pytorch.py
--rw-r--r--   0        0        0     8344 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/r_model.py
--rw-r--r--   0        0        0     2284 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/sklearn.py
--rw-r--r--   0        0        0     1455 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/statsmodels.py
--rw-r--r--   0        0        0      951 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/models/xgboost.py
--rw-r--r--   0        0        0     7918 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/template.py
--rw-r--r--   0        0        0     7231 2024-03-27 20:37:00.267768 validmind-2.0.1/validmind/test_suites/__init__.py
--rw-r--r--   0        0        0     4003 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/classifier.py
--rw-r--r--   0        0        0     2276 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/cluster.py
--rw-r--r--   0        0        0     1949 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/embeddings.py
--rw-r--r--   0        0        0     2026 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/llm.py
--rw-r--r--   0        0        0     1344 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/nlp.py
--rw-r--r--   0        0        0      731 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/parameters_optimization.py
--rw-r--r--   0        0        0     2407 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/regression.py
--rw-r--r--   0        0        0      957 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/statsmodels_timeseries.py
--rw-r--r--   0        0        0      695 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/summarization.py
--rw-r--r--   0        0        0     1798 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/tabular_datasets.py
--rw-r--r--   0        0        0      739 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/text_data.py
--rw-r--r--   0        0        0     6724 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/test_suites/time_series.py
--rw-r--r--   0        0        0    12416 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/__init__.py
--rw-r--r--   0        0        0     1603 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/__types__.py
--rw-r--r--   0        0        0     4745 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/ACFandPACFPlot.py
--rw-r--r--   0        0        0     6026 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/ANOVAOneWayTable.py
--rw-r--r--   0        0        0     6676 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/AutoAR.py
--rw-r--r--   0        0        0     7119 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/AutoMA.py
--rw-r--r--   0        0        0     8085 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/AutoSeasonality.py
--rw-r--r--   0        0        0     7902 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/AutoStationarity.py
--rw-r--r--   0        0        0     5974 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/BivariateFeaturesBarPlots.py
--rw-r--r--   0        0        0     5018 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/BivariateHistograms.py
--rw-r--r--   0        0        0     5208 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/BivariateScatterPlots.py
--rw-r--r--   0        0        0     6048 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/ChiSquaredFeaturesTable.py
--rw-r--r--   0        0        0     6922 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/ClassImbalance.py
--rw-r--r--   0        0        0    11402 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/DatasetDescription.py
--rw-r--r--   0        0        0     5127 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/DatasetSplit.py
--rw-r--r--   0        0        0     4861 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/DefaultRatesbyRiskBandPlot.py
--rw-r--r--   0        0        0     6411 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/DescriptiveStatistics.py
--rw-r--r--   0        0        0     5639 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/Duplicates.py
--rw-r--r--   0        0        0     5580 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/EngleGrangerCoint.py
--rw-r--r--   0        0        0     5001 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/FeatureTargetCorrelationPlot.py
--rw-r--r--   0        0        0     5707 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/HeatmapFeatureCorrelations.py
--rw-r--r--   0        0        0     5111 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/HighCardinality.py
--rw-r--r--   0        0        0     5582 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/HighPearsonCorrelation.py
--rw-r--r--   0        0        0     6350 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/IQROutliersBarPlot.py
--rw-r--r--   0        0        0     5888 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/IQROutliersTable.py
--rw-r--r--   0        0        0     4872 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/IsolationForestOutliers.py
--rw-r--r--   0        0        0     6055 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/LaggedCorrelationHeatmap.py
--rw-r--r--   0        0        0     4292 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/MissingValues.py
--rw-r--r--   0        0        0     6226 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/MissingValuesBarPlot.py
--rw-r--r--   0        0        0     4110 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/MissingValuesRisk.py
--rw-r--r--   0        0        0     4747 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/PearsonCorrelationMatrix.py
--rw-r--r--   0        0        0     5639 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/PiTCreditScoresHistogram.py
--rw-r--r--   0        0        0     5950 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/PiTPDHistogram.py
--rw-r--r--   0        0        0     5901 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/RollingStatsPlot.py
--rw-r--r--   0        0        0     4047 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/ScatterPlot.py
--rw-r--r--   0        0        0     8903 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/SeasonalDecompose.py
--rw-r--r--   0        0        0     4935 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/Skewness.py
--rw-r--r--   0        0        0     4591 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/SpreadPlot.py
--rw-r--r--   0        0        0     4241 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TabularCategoricalBarPlots.py
--rw-r--r--   0        0        0     4211 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TabularDateTimeHistograms.py
--rw-r--r--   0        0        0     9281 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TabularDescriptionTables.py
--rw-r--r--   0        0        0     4170 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TabularNumericalHistograms.py
--rw-r--r--   0        0        0     5744 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TargetRateBarPlots.py
--rw-r--r--   0        0        0     7243 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TimeSeriesFrequency.py
--rw-r--r--   0        0        0     4188 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TimeSeriesHistogram.py
--rw-r--r--   0        0        0     4173 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TimeSeriesLinePlot.py
--rw-r--r--   0        0        0     7351 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TimeSeriesMissingValues.py
--rw-r--r--   0        0        0     9749 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TimeSeriesOutliers.py
--rw-r--r--   0        0        0     5875 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/TooManyZeroValues.py
--rw-r--r--   0        0        0     4516 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/UniqueRows.py
--rw-r--r--   0        0        0     6947 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/WOEBinPlots.py
--rw-r--r--   0        0        0     4711 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/WOEBinTable.py
--rw-r--r--   0        0        0        0 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/nlp/CommonWords.py
--rw-r--r--   0        0        0     4368 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/nlp/Hashtags.py
--rw-r--r--   0        0        0     4673 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/nlp/Mentions.py
--rw-r--r--   0        0        0     3867 2024-03-27 20:37:00.271768 validmind-2.0.1/validmind/tests/data_validation/nlp/Punctuations.py
--rw-r--r--   0        0        0     6353 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/data_validation/nlp/StopWords.py
--rw-r--r--   0        0        0     8109 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/data_validation/nlp/TextDescription.py
--rw-r--r--   0        0        0        0 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/data_validation/nlp/__init__.py
--rw-r--r--   0        0        0     4560 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/BertScore.py
--rw-r--r--   0        0        0     3781 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/BertScoreAggregate.py
--rw-r--r--   0        0        0     3848 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/BleuScore.py
--rw-r--r--   0        0        0     4164 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/ClusterSizeDistribution.py
--rw-r--r--   0        0        0     4801 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/ContextualRecall.py
--rw-r--r--   0        0        0     3733 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/ModelMetadata.py
--rw-r--r--   0        0        0     6330 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/RegardHistogram.py
--rw-r--r--   0        0        0     6339 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/RegardScore.py
--rw-r--r--   0        0        0     5694 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/RougeMetrics.py
--rw-r--r--   0        0        0     5213 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/RougeMetricsAggregate.py
--rw-r--r--   0        0        0     5465 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/TokenDisparity.py
--rw-r--r--   0        0        0     5108 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/ToxicityHistogram.py
--rw-r--r--   0        0        0     5571 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/ToxicityScore.py
--rw-r--r--   0        0        0        0 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/__init__.py
--rw-r--r--   0        0        0     3561 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/ClusterDistribution.py
--rw-r--r--   0        0        0     3490 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/CosineSimilarityDistribution.py
--rw-r--r--   0        0        0     4124 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/DescriptiveAnalytics.py
--rw-r--r--   0        0        0     4351 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/EmbeddingsVisualization2D.py
--rw-r--r--   0        0        0     4185 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysis.py
--rw-r--r--   0        0        0     3907 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisKeyword.py
--rw-r--r--   0        0        0     5672 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisRandomNoise.py
--rw-r--r--   0        0        0     4342 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisSynonyms.py
--rw-r--r--   0        0        0     4573 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisTranslation.py
--rw-r--r--   0        0        0     2892 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/AdjustedMutualInformation.py
--rw-r--r--   0        0        0     2767 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/AdjustedRandIndex.py
--rw-r--r--   0        0        0     5953 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ClassifierPerformance.py
--rw-r--r--   0        0        0     5494 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ClusterCosineSimilarity.py
--rw-r--r--   0        0        0     5387 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ClusterPerformance.py
--rw-r--r--   0        0        0     8604 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ClusterPerformanceMetrics.py
--rw-r--r--   0        0        0     2559 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/CompletenessScore.py
--rw-r--r--   0        0        0     5267 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ConfusionMatrix.py
--rw-r--r--   0        0        0     3049 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/FowlkesMallowsScore.py
--rw-r--r--   0        0        0     2753 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/HomogeneityScore.py
--rw-r--r--   0        0        0     4660 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/HyperParametersTuning.py
--rw-r--r--   0        0        0     5960 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/KMeansClustersOptimization.py
--rw-r--r--   0        0        0     5346 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/MinimumAccuracy.py
--rw-r--r--   0        0        0     4687 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/MinimumF1Score.py
--rw-r--r--   0        0        0     4900 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/MinimumROCAUCScore.py
--rw-r--r--   0        0        0     6303 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ModelsPerformanceComparison.py
--rw-r--r--   0        0        0    14174 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/OverfitDiagnosis.py
--rw-r--r--   0        0        0     5038 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/PermutationFeatureImportance.py
--rw-r--r--   0        0        0    10242 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/PopulationStabilityIndex.py
--rw-r--r--   0        0        0     4401 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/PrecisionRecallCurve.py
--rw-r--r--   0        0        0     5964 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/ROCCurve.py
--rw-r--r--   0        0        0     5998 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/RegressionErrors.py
--rw-r--r--   0        0        0     5522 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/RegressionModelsPerformanceComparison.py
--rw-r--r--   0        0        0     4987 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/RegressionR2Square.py
--rw-r--r--   0        0        0    13780 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/RobustnessDiagnosis.py
--rw-r--r--   0        0        0     6713 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/SHAPGlobalImportance.py
--rw-r--r--   0        0        0     6246 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/SilhouettePlot.py
--rw-r--r--   0        0        0     7078 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/TrainingTestDegradation.py
--rw-r--r--   0        0        0     2772 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/VMeasure.py
--rw-r--r--   0        0        0    14245 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/WeakspotsDiagnosis.py
--rw-r--r--   0        0        0        0 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/sklearn/__init__.py
--rw-r--r--   0        0        0     4042 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ADF.py
--rw-r--r--   0        0        0     4039 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ADFTest.py
--rw-r--r--   0        0        0     5172 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/AutoARIMA.py
--rw-r--r--   0        0        0     3581 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/BoxPierce.py
--rw-r--r--   0        0        0     3365 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/DFGLSArch.py
--rw-r--r--   0        0        0     2957 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/DurbinWatsonTest.py
--rw-r--r--   0        0        0     7199 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/FeatureImportanceAndSignificance.py
--rw-r--r--   0        0        0     6335 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/GINITable.py
--rw-r--r--   0        0        0     3362 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/JarqueBera.py
--rw-r--r--   0        0        0     3313 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/KPSS.py
--rw-r--r--   0        0        0     4371 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/KolmogorovSmirnov.py
--rw-r--r--   0        0        0     3309 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/LJungBox.py
--rw-r--r--   0        0        0     3997 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/Lilliefors.py
--rw-r--r--   0        0        0     5339 2024-03-27 20:37:00.275768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/LogRegressionConfusionMatrix.py
--rw-r--r--   0        0        0     7155 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/LogisticRegCumulativeProb.py
--rw-r--r--   0        0        0     6859 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/LogisticRegPredictionHistogram.py
--rw-r--r--   0        0        0     6064 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/PDRatingClassPlot.py
--rw-r--r--   0        0        0     3133 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/PhillipsPerronArch.py
--rw-r--r--   0        0        0     5657 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionCoeffsPlot.py
--rw-r--r--   0        0        0     5494 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionFeatureSignificance.py
--rw-r--r--   0        0        0     6598 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlot.py
--rw-r--r--   0        0        0     8346 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlotLevels.py
--rw-r--r--   0        0        0     6483 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelInsampleComparison.py
--rw-r--r--   0        0        0     6292 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelOutsampleComparison.py
--rw-r--r--   0        0        0     7320 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelSensitivityPlot.py
--rw-r--r--   0        0        0     4359 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelSummary.py
--rw-r--r--   0        0        0     4592 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelsCoeffs.py
--rw-r--r--   0        0        0     5454 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelsPerformance.py
--rw-r--r--   0        0        0     5771 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ResidualsVisualInspection.py
--rw-r--r--   0        0        0     3684 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/RunsTest.py
--rw-r--r--   0        0        0     6901 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ScorecardBucketHistogram.py
--rw-r--r--   0        0        0     7073 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ScorecardHistogram.py
--rw-r--r--   0        0        0     7140 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ScorecardProbabilitiesHistogram.py
--rw-r--r--   0        0        0     3243 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ShapiroWilk.py
--rw-r--r--   0        0        0     3291 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/ZivotAndrewsArch.py
--rw-r--r--   0        0        0        0 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/__init__.py
--rw-r--r--   0        0        0      495 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/model_validation/statsmodels/statsutils.py
--rw-r--r--   0        0        0     7060 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/Bias.py
--rw-r--r--   0        0        0     6256 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/Clarity.py
--rw-r--r--   0        0        0     6004 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/Conciseness.py
--rw-r--r--   0        0        0     5522 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/Delimitation.py
--rw-r--r--   0        0        0     6671 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/NegativeInstruction.py
--rw-r--r--   0        0        0     6826 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/Robustness.py
--rw-r--r--   0        0        0     6116 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/Specificity.py
--rw-r--r--   0        0        0        0 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/__init__.py
--rw-r--r--   0        0        0     2917 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/prompt_validation/ai_powered_test.py
--rw-r--r--   0        0        0     8280 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/tests/test_providers.py
--rw-r--r--   0        0        0     8257 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/unit_metrics/__init__.py
--rw-r--r--   0        0        0      610 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/unit_metrics/sklearn/classification/Accuracy.py
--rw-r--r--   0        0        0      615 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/unit_metrics/sklearn/classification/F1.py
--rw-r--r--   0        0        0      636 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/unit_metrics/sklearn/classification/Precision.py
--rw-r--r--   0        0        0      607 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/unit_metrics/sklearn/classification/ROC_AUC.py
--rw-r--r--   0        0        0      604 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/unit_metrics/sklearn/classification/Recall.py
--rw-r--r--   0        0        0    13179 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/utils.py
--rw-r--r--   0        0        0     1219 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/__init__.py
--rw-r--r--   0        0        0    22477 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/dataset.py
--rw-r--r--   0        0        0     5579 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/figure.py
--rw-r--r--   0        0        0     4823 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/model.py
--rw-r--r--   0        0        0     3848 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/metric.py
--rw-r--r--   0        0        0     1987 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/metric_result.py
--rw-r--r--   0        0        0     2369 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/output_template.py
--rw-r--r--   0        0        0     2028 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/result_summary.py
--rw-r--r--   0        0        0    12332 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/result_wrapper.py
--rw-r--r--   0        0        0     3028 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/test.py
--rw-r--r--   0        0        0     3934 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/threshold_test.py
--rw-r--r--   0        0        0     1954 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/threshold_test_result.py
--rw-r--r--   0        0        0     2556 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test/unit_metric.py
--rw-r--r--   0        0        0     8801 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test_context.py
--rw-r--r--   0        0        0     6748 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test_suite/runner.py
--rw-r--r--   0        0        0     4583 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test_suite/summary.py
--rw-r--r--   0        0        0     5279 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test_suite/test.py
--rw-r--r--   0        0        0     6244 2024-03-27 20:37:00.279768 validmind-2.0.1/validmind/vm_models/test_suite/test_suite.py
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 validmind-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35772 2024-04-10 21:45:32.607484 validmind-2.0.7/LICENSE
+-rw-r--r--   0        0        0      790 2024-04-10 21:45:32.607484 validmind-2.0.7/README.pypi.md
+-rw-r--r--   0        0        0     2514 2024-04-10 21:45:33.043485 validmind-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3699 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/__version__.py
+-rw-r--r--   0        0        0     6544 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/ai.py
+-rw-r--r--   0        0        0    15290 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/api_client.py
+-rw-r--r--   0        0        0    16618 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/client.py
+-rw-r--r--   0        0        0     1611 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/client_config.py
+-rw-r--r--   0        0        0      262 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/datasets/__init__.py
+-rw-r--r--   0        0        0     1787 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     3802 2024-04-10 21:45:33.047484 validmind-2.0.7/validmind/datasets/classification/customer_churn.py
+-rw-r--r--   0        0        0   545707 2024-04-10 21:45:33.051484 validmind-2.0.7/validmind/datasets/classification/datasets/bank_customer_churn.csv
+-rw-r--r--   0        0        0  2897191 2024-04-10 21:45:33.063485 validmind-2.0.7/validmind/datasets/classification/datasets/taiwan_credit.csv
+-rw-r--r--   0        0        0     1469 2024-04-10 21:45:33.063485 validmind-2.0.7/validmind/datasets/classification/taiwan_credit.py
+-rw-r--r--   0        0        0     2097 2024-04-10 21:45:33.063485 validmind-2.0.7/validmind/datasets/cluster/digits.py
+-rw-r--r--   0        0        0      323 2024-04-10 21:45:33.063485 validmind-2.0.7/validmind/datasets/nlp/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-10 21:45:33.063485 validmind-2.0.7/validmind/datasets/nlp/cnn_dailymail.py
+-rw-r--r--   0        0        0 11545066 2024-04-10 21:45:33.119485 validmind-2.0.7/validmind/datasets/nlp/datasets/Covid_19.csv
+-rw-r--r--   0        0        0   426676 2024-04-10 21:45:33.119485 validmind-2.0.7/validmind/datasets/nlp/datasets/cnn_dailymail_100_with_predictions.csv
+-rw-r--r--   0        0        0  2246787 2024-04-10 21:45:33.119485 validmind-2.0.7/validmind/datasets/nlp/datasets/cnn_dailymail_500_with_predictions.csv
+-rw-r--r--   0        0        0   754686 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/nlp/datasets/sentiments_with_predictions.csv
+-rw-r--r--   0        0        0      878 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/nlp/twitter_covid_19.py
+-rw-r--r--   0        0        0     1653 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/__init__.py
+-rw-r--r--   0        0        0     1046 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/california_housing.py
+-rw-r--r--   0        0        0    15834 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/CPIAUCSL.csv
+-rw-r--r--   0        0        0     9105 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/CSUSHPISA.csv
+-rw-r--r--   0        0        0     2093 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/DRSFRMACBS.csv
+-rw-r--r--   0        0        0    13274 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/FEDFUNDS.csv
+-rw-r--r--   0        0        0     6061 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/GDP.csv
+-rw-r--r--   0        0        0     6201 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/GDPC1.csv
+-rw-r--r--   0        0        0    13538 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/GS10.csv
+-rw-r--r--   0        0        0    13506 2024-04-10 21:45:33.123484 validmind-2.0.7/validmind/datasets/regression/datasets/fred/GS3.csv
+-rw-r--r--   0        0        0    13514 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred/GS5.csv
+-rw-r--r--   0        0        0    44040 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred/MORTGAGE30US.csv
+-rw-r--r--   0        0        0    13572 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred/UNRATE.csv
+-rw-r--r--   0        0        0   107835 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates.csv
+-rw-r--r--   0        0        0     2634 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
+-rw-r--r--   0        0        0     2634 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
+-rw-r--r--   0        0        0     2736 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
+-rw-r--r--   0        0        0     3355 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
+-rw-r--r--   0        0        0     3866 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
+-rw-r--r--   0        0        0    11624 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
+-rw-r--r--   0        0        0     5707 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/fred.py
+-rw-r--r--   0        0        0     2536 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/lending_club.py
+-rw-r--r--   0        0        0    40067 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
+-rw-r--r--   0        0        0    48314 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
+-rw-r--r--   0        0        0    40063 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
+-rw-r--r--   0        0        0    48292 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
+-rw-r--r--   0        0        0    60343 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
+-rw-r--r--   0        0        0     7993 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/errors.py
+-rw-r--r--   0        0        0     1607 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/html_templates/content_blocks.py
+-rw-r--r--   0        0        0      793 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/input_registry.py
+-rw-r--r--   0        0        0     4808 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/logging.py
+-rw-r--r--   0        0        0      623 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/__init__.py
+-rw-r--r--   0        0        0     1036 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/catboost.py
+-rw-r--r--   0        0        0     2269 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/foundation.py
+-rw-r--r--   0        0        0     2881 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/huggingface.py
+-rw-r--r--   0        0        0     2602 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/pytorch.py
+-rw-r--r--   0        0        0     8344 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/r_model.py
+-rw-r--r--   0        0        0     2405 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/sklearn.py
+-rw-r--r--   0        0        0     1455 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/statsmodels.py
+-rw-r--r--   0        0        0      951 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/models/xgboost.py
+-rw-r--r--   0        0        0     7918 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/template.py
+-rw-r--r--   0        0        0     7231 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/__init__.py
+-rw-r--r--   0        0        0     4003 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/classifier.py
+-rw-r--r--   0        0        0     2276 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/cluster.py
+-rw-r--r--   0        0        0     1949 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/embeddings.py
+-rw-r--r--   0        0        0     2026 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/llm.py
+-rw-r--r--   0        0        0     1344 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/nlp.py
+-rw-r--r--   0        0        0      731 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/parameters_optimization.py
+-rw-r--r--   0        0        0     2407 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/regression.py
+-rw-r--r--   0        0        0      957 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/statsmodels_timeseries.py
+-rw-r--r--   0        0        0      695 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/summarization.py
+-rw-r--r--   0        0        0     1798 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/tabular_datasets.py
+-rw-r--r--   0        0        0      739 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/text_data.py
+-rw-r--r--   0        0        0     6724 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/test_suites/time_series.py
+-rw-r--r--   0        0        0    13854 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/__init__.py
+-rw-r--r--   0        0        0     1603 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/__types__.py
+-rw-r--r--   0        0        0     4745 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/ACFandPACFPlot.py
+-rw-r--r--   0        0        0     6026 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/ANOVAOneWayTable.py
+-rw-r--r--   0        0        0     6676 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/AutoAR.py
+-rw-r--r--   0        0        0     7119 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/AutoMA.py
+-rw-r--r--   0        0        0     8085 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/AutoSeasonality.py
+-rw-r--r--   0        0        0     7902 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/AutoStationarity.py
+-rw-r--r--   0        0        0     5974 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/BivariateFeaturesBarPlots.py
+-rw-r--r--   0        0        0     5018 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/BivariateHistograms.py
+-rw-r--r--   0        0        0     5208 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/BivariateScatterPlots.py
+-rw-r--r--   0        0        0     6048 2024-04-10 21:45:33.127485 validmind-2.0.7/validmind/tests/data_validation/ChiSquaredFeaturesTable.py
+-rw-r--r--   0        0        0     6922 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/ClassImbalance.py
+-rw-r--r--   0        0        0    11401 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/DatasetDescription.py
+-rw-r--r--   0        0        0     5127 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/DatasetSplit.py
+-rw-r--r--   0        0        0     4861 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/DefaultRatesbyRiskBandPlot.py
+-rw-r--r--   0        0        0     6411 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/DescriptiveStatistics.py
+-rw-r--r--   0        0        0     5639 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/Duplicates.py
+-rw-r--r--   0        0        0     5580 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/EngleGrangerCoint.py
+-rw-r--r--   0        0        0     5001 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/FeatureTargetCorrelationPlot.py
+-rw-r--r--   0        0        0     5707 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/HeatmapFeatureCorrelations.py
+-rw-r--r--   0        0        0     5111 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/HighCardinality.py
+-rw-r--r--   0        0        0     5582 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/HighPearsonCorrelation.py
+-rw-r--r--   0        0        0     6350 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/IQROutliersBarPlot.py
+-rw-r--r--   0        0        0     5888 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/IQROutliersTable.py
+-rw-r--r--   0        0        0     4872 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/IsolationForestOutliers.py
+-rw-r--r--   0        0        0     6055 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/LaggedCorrelationHeatmap.py
+-rw-r--r--   0        0        0     4292 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/MissingValues.py
+-rw-r--r--   0        0        0     6226 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/MissingValuesBarPlot.py
+-rw-r--r--   0        0        0     4110 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/MissingValuesRisk.py
+-rw-r--r--   0        0        0     4747 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/PearsonCorrelationMatrix.py
+-rw-r--r--   0        0        0     5639 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/PiTCreditScoresHistogram.py
+-rw-r--r--   0        0        0     5950 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/PiTPDHistogram.py
+-rw-r--r--   0        0        0     5901 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/RollingStatsPlot.py
+-rw-r--r--   0        0        0     4047 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/ScatterPlot.py
+-rw-r--r--   0        0        0     8903 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/SeasonalDecompose.py
+-rw-r--r--   0        0        0     4935 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/Skewness.py
+-rw-r--r--   0        0        0     4591 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/SpreadPlot.py
+-rw-r--r--   0        0        0     4241 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TabularCategoricalBarPlots.py
+-rw-r--r--   0        0        0     4211 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TabularDateTimeHistograms.py
+-rw-r--r--   0        0        0     9281 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TabularDescriptionTables.py
+-rw-r--r--   0        0        0     4170 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TabularNumericalHistograms.py
+-rw-r--r--   0        0        0     5744 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TargetRateBarPlots.py
+-rw-r--r--   0        0        0     7243 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TimeSeriesFrequency.py
+-rw-r--r--   0        0        0     4188 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TimeSeriesHistogram.py
+-rw-r--r--   0        0        0     4173 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TimeSeriesLinePlot.py
+-rw-r--r--   0        0        0     7351 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TimeSeriesMissingValues.py
+-rw-r--r--   0        0        0     9749 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TimeSeriesOutliers.py
+-rw-r--r--   0        0        0     5875 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/TooManyZeroValues.py
+-rw-r--r--   0        0        0     4516 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/UniqueRows.py
+-rw-r--r--   0        0        0     6947 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/WOEBinPlots.py
+-rw-r--r--   0        0        0     4711 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/WOEBinTable.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/__init__.py
+-rw-r--r--   0        0        0     4204 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/CommonWords.py
+-rw-r--r--   0        0        0     4368 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/Hashtags.py
+-rw-r--r--   0        0        0     4673 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/Mentions.py
+-rw-r--r--   0        0        0     3867 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/Punctuations.py
+-rw-r--r--   0        0        0     6131 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/StopWords.py
+-rw-r--r--   0        0        0     8718 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/TextDescription.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/data_validation/nlp/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/decorator.py
+-rw-r--r--   0        0        0     4560 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/BertScore.py
+-rw-r--r--   0        0        0     3781 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/BertScoreAggregate.py
+-rw-r--r--   0        0        0     3848 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/BleuScore.py
+-rw-r--r--   0        0        0     4164 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/ClusterSizeDistribution.py
+-rw-r--r--   0        0        0     4801 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/ContextualRecall.py
+-rw-r--r--   0        0        0     4396 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/MeteorScore.py
+-rw-r--r--   0        0        0     3733 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/ModelMetadata.py
+-rw-r--r--   0        0        0     6160 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/RegardHistogram.py
+-rw-r--r--   0        0        0     6181 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/RegardScore.py
+-rw-r--r--   0        0        0     5802 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/RougeMetrics.py
+-rw-r--r--   0        0        0     5213 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/RougeMetricsAggregate.py
+-rw-r--r--   0        0        0     5486 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/SelfCheckNLIScore.py
+-rw-r--r--   0        0        0     5465 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/TokenDisparity.py
+-rw-r--r--   0        0        0     5108 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/ToxicityHistogram.py
+-rw-r--r--   0        0        0     5571 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/ToxicityScore.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/__init__.py
+-rw-r--r--   0        0        0     3561 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/embeddings/ClusterDistribution.py
+-rw-r--r--   0        0        0     3490 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/embeddings/CosineSimilarityDistribution.py
+-rw-r--r--   0        0        0     4256 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/embeddings/DescriptiveAnalytics.py
+-rw-r--r--   0        0        0     4351 2024-04-10 21:45:33.131485 validmind-2.0.7/validmind/tests/model_validation/embeddings/EmbeddingsVisualization2D.py
+-rw-r--r--   0        0        0     4185 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysis.py
+-rw-r--r--   0        0        0     3907 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisKeyword.py
+-rw-r--r--   0        0        0     5672 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisRandomNoise.py
+-rw-r--r--   0        0        0     4342 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisSynonyms.py
+-rw-r--r--   0        0        0     4573 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisTranslation.py
+-rw-r--r--   0        0        0     2892 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/AdjustedMutualInformation.py
+-rw-r--r--   0        0        0     2767 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/AdjustedRandIndex.py
+-rw-r--r--   0        0        0     5992 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ClassifierPerformance.py
+-rw-r--r--   0        0        0     5494 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ClusterCosineSimilarity.py
+-rw-r--r--   0        0        0     5387 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ClusterPerformance.py
+-rw-r--r--   0        0        0     8604 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ClusterPerformanceMetrics.py
+-rw-r--r--   0        0        0     2559 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/CompletenessScore.py
+-rw-r--r--   0        0        0     5267 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ConfusionMatrix.py
+-rw-r--r--   0        0        0     3049 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/FowlkesMallowsScore.py
+-rw-r--r--   0        0        0     2753 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/HomogeneityScore.py
+-rw-r--r--   0        0        0     4660 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/HyperParametersTuning.py
+-rw-r--r--   0        0        0     5960 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/KMeansClustersOptimization.py
+-rw-r--r--   0        0        0     5346 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/MinimumAccuracy.py
+-rw-r--r--   0        0        0     4687 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/MinimumF1Score.py
+-rw-r--r--   0        0        0     4900 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/MinimumROCAUCScore.py
+-rw-r--r--   0        0        0     6303 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ModelsPerformanceComparison.py
+-rw-r--r--   0        0        0    14174 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/OverfitDiagnosis.py
+-rw-r--r--   0        0        0     5038 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/PermutationFeatureImportance.py
+-rw-r--r--   0        0        0    10242 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/PopulationStabilityIndex.py
+-rw-r--r--   0        0        0     4401 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/PrecisionRecallCurve.py
+-rw-r--r--   0        0        0     5964 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/ROCCurve.py
+-rw-r--r--   0        0        0     5998 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/RegressionErrors.py
+-rw-r--r--   0        0        0     5522 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/RegressionModelsPerformanceComparison.py
+-rw-r--r--   0        0        0     4987 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/RegressionR2Square.py
+-rw-r--r--   0        0        0    13780 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/RobustnessDiagnosis.py
+-rw-r--r--   0        0        0     7655 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/SHAPGlobalImportance.py
+-rw-r--r--   0        0        0     6246 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/SilhouettePlot.py
+-rw-r--r--   0        0        0     7291 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/TrainingTestDegradation.py
+-rw-r--r--   0        0        0     2772 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/VMeasure.py
+-rw-r--r--   0        0        0    14245 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/WeakspotsDiagnosis.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/sklearn/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ADF.py
+-rw-r--r--   0        0        0     4039 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ADFTest.py
+-rw-r--r--   0        0        0     5172 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/AutoARIMA.py
+-rw-r--r--   0        0        0     3581 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/BoxPierce.py
+-rw-r--r--   0        0        0     3365 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/DFGLSArch.py
+-rw-r--r--   0        0        0     2957 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/DurbinWatsonTest.py
+-rw-r--r--   0        0        0     7199 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/FeatureImportanceAndSignificance.py
+-rw-r--r--   0        0        0     6335 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/GINITable.py
+-rw-r--r--   0        0        0     3362 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/JarqueBera.py
+-rw-r--r--   0        0        0     3313 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/KPSS.py
+-rw-r--r--   0        0        0     4371 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/KolmogorovSmirnov.py
+-rw-r--r--   0        0        0     3309 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/LJungBox.py
+-rw-r--r--   0        0        0     3997 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/Lilliefors.py
+-rw-r--r--   0        0        0     5339 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/LogRegressionConfusionMatrix.py
+-rw-r--r--   0        0        0     7155 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/LogisticRegCumulativeProb.py
+-rw-r--r--   0        0        0     6859 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/LogisticRegPredictionHistogram.py
+-rw-r--r--   0        0        0     6064 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/PDRatingClassPlot.py
+-rw-r--r--   0        0        0     3133 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/PhillipsPerronArch.py
+-rw-r--r--   0        0        0     5657 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionCoeffsPlot.py
+-rw-r--r--   0        0        0     5494 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionFeatureSignificance.py
+-rw-r--r--   0        0        0     6598 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlot.py
+-rw-r--r--   0        0        0     8346 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlotLevels.py
+-rw-r--r--   0        0        0     6483 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelInsampleComparison.py
+-rw-r--r--   0        0        0     6292 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelOutsampleComparison.py
+-rw-r--r--   0        0        0     7320 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelSensitivityPlot.py
+-rw-r--r--   0        0        0     4359 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelSummary.py
+-rw-r--r--   0        0        0     4592 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelsCoeffs.py
+-rw-r--r--   0        0        0     5452 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelsPerformance.py
+-rw-r--r--   0        0        0     5771 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ResidualsVisualInspection.py
+-rw-r--r--   0        0        0     3684 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/RunsTest.py
+-rw-r--r--   0        0        0     6901 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ScorecardBucketHistogram.py
+-rw-r--r--   0        0        0     7073 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ScorecardHistogram.py
+-rw-r--r--   0        0        0     7140 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ScorecardProbabilitiesHistogram.py
+-rw-r--r--   0        0        0     3243 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ShapiroWilk.py
+-rw-r--r--   0        0        0     3291 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/ZivotAndrewsArch.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-10 21:45:33.135485 validmind-2.0.7/validmind/tests/model_validation/statsmodels/statsutils.py
+-rw-r--r--   0        0        0     7060 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/Bias.py
+-rw-r--r--   0        0        0     6256 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/Clarity.py
+-rw-r--r--   0        0        0     6004 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/Conciseness.py
+-rw-r--r--   0        0        0     5522 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/Delimitation.py
+-rw-r--r--   0        0        0     6671 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/NegativeInstruction.py
+-rw-r--r--   0        0        0     6826 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/Robustness.py
+-rw-r--r--   0        0        0     6116 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/Specificity.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/__init__.py
+-rw-r--r--   0        0        0     2975 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/prompt_validation/ai_powered_test.py
+-rw-r--r--   0        0        0     8280 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/tests/test_providers.py
+-rw-r--r--   0        0        0     8192 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/__init__.py
+-rw-r--r--   0        0        0     9013 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/composite.py
+-rw-r--r--   0        0        0     1228 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/GiniCoefficient.py
+-rw-r--r--   0        0        0      880 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/HuberLoss.py
+-rw-r--r--   0        0        0     1221 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/KolmogorovSmirnovStatistic.py
+-rw-r--r--   0        0        0      653 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/MeanAbsolutePercentageError.py
+-rw-r--r--   0        0        0      618 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/MeanBiasDeviation.py
+-rw-r--r--   0        0        0      749 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/QuantileLoss.py
+-rw-r--r--   0        0        0      859 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/sklearn/AdjustedRSquaredScore.py
+-rw-r--r--   0        0        0      673 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/sklearn/MeanAbsoluteError.py
+-rw-r--r--   0        0        0      670 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/sklearn/MeanSquaredError.py
+-rw-r--r--   0        0        0      637 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/sklearn/RSquaredScore.py
+-rw-r--r--   0        0        0      702 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/regression/sklearn/RootMeanSquaredError.py
+-rw-r--r--   0        0        0      654 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/sklearn/classification/Accuracy.py
+-rw-r--r--   0        0        0      659 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/sklearn/classification/F1.py
+-rw-r--r--   0        0        0      680 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/sklearn/classification/Precision.py
+-rw-r--r--   0        0        0      651 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/sklearn/classification/ROC_AUC.py
+-rw-r--r--   0        0        0      648 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/unit_metrics/sklearn/classification/Recall.py
+-rw-r--r--   0        0        0    13757 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/utils.py
+-rw-r--r--   0        0        0     1219 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/__init__.py
+-rw-r--r--   0        0        0    33717 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/dataset.py
+-rw-r--r--   0        0        0     6651 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/figure.py
+-rw-r--r--   0        0        0     4823 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/model.py
+-rw-r--r--   0        0        0     3965 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/metric.py
+-rw-r--r--   0        0        0     1987 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/metric_result.py
+-rw-r--r--   0        0        0     1500 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/output_template.py
+-rw-r--r--   0        0        0     2028 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/result_summary.py
+-rw-r--r--   0        0        0    13970 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/result_wrapper.py
+-rw-r--r--   0        0        0     3077 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/test.py
+-rw-r--r--   0        0        0     4324 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/threshold_test.py
+-rw-r--r--   0        0        0     1954 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/threshold_test_result.py
+-rw-r--r--   0        0        0     2556 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test/unit_metric.py
+-rw-r--r--   0        0        0     9027 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test_context.py
+-rw-r--r--   0        0        0     6754 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test_suite/runner.py
+-rw-r--r--   0        0        0     4583 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test_suite/summary.py
+-rw-r--r--   0        0        0     5285 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test_suite/test.py
+-rw-r--r--   0        0        0     6244 2024-04-10 21:45:33.139485 validmind-2.0.7/validmind/vm_models/test_suite/test_suite.py
+-rw-r--r--   0        0        0     3463 1970-01-01 00:00:00.000000 validmind-2.0.7/PKG-INFO
```

### Comparing `validmind-2.0.1/LICENSE` & `validmind-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/README.pypi.md` & `validmind-2.0.7/README.pypi.md`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/pyproject.toml` & `validmind-2.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,76 +6,72 @@
   "Luis Pallares <luis@validmind.ai>",
   "John Halz <john@validmind.ai>",
 ]
 description = "ValidMind Developer Framework"
 license = "Commercial License"
 name = "validmind"
 readme = "README.pypi.md"
-version = "2.0.1"
+version = "2.0.7"
 
 [tool.poetry.dependencies]
 aiohttp = {extras = ["speedups"], version = "^3.8.4"}
 arch = "^5.4.0"
 bert-score = "^0.3.13"
 catboost = "^1.2"
 click = "^8.0.4"
-datasets = {version = "^2.14.5", optional = true}
-dython = "^0.7.1"
 evaluate = "^0.4.0"
-ipython = "7.34.0"
 ipywidgets = "^8.0.6"
-jupyter = "^1.0.0"
-kaleido = "0.2.1"
+kaleido = "^0.2.1,!=0.2.1.post1"
 langdetect = "^1.0.9"
 levenshtein = {version = "^0.21.1", optional = true}
 markdown = "^3.4.3"
-matplotlib = "<3.8"
+matplotlib = "<3.8.3"
 nltk = "^3.8.1"
+numba = "<0.59.0" # TODO: https://github.com/validmind/developer-framework/pull/28
 numpy = "^1.23.3"
 openai = {version = "^1.3.7", optional = true}
 pandas = "1.5.3"
-pandas-profiling = "^3.6.6"
-pdoc = "^13.1.1"
 plotly = "^5.14.1"
 plotly-express = "^0.4.1"
+polars = "^0.20.15"
 pycocoevalcap = {version = "^1.2", optional = true}
-pydantic = "^1.9.1"
 pypmml = "^0.9.17"
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 python-dotenv = "^0.20.0"
 requests = "^2.27.1"
 rouge = "^1.0.1"
 rpy2 = {version = "^3.5.10", optional = true}
 scikit-learn = "^1.0.2"
 scorecardpy = "^0.1.9.6"
 seaborn = "^0.11.2"
-sentencepiece = "^0.1.99"
+selfcheckgpt = "^0.1.7"
 sentry-sdk = "^1.24.0"
 shap = "^0.42.0"
 statsmodels = "^0.13.5"
 tabulate = "^0.8.9"
 textstat = "^0.7.3"
 torch = {version = ">=1.10.0", optional = true}
 torchmetrics = {version = "^1.1.1", optional = true}
 tqdm = "^4.64.0"
-transformers = "^4.32.0"
-wget = "^3.2"
+transformers = {version = "^4.32.0", optional = true}
 xgboost = "^1.5.2"
+ydata-profiling = "^4.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 click = "^8.1.3"
 cython = "^0.29.34"
 flake8 = "^4.0.1"
 gradio = "^3.43.2"
 ipykernel = "^6.22.0"
 isort = "^5.12.0"
-jupyterlab = "^3.6.3"
+jupyter = "^1.0.0"
 openai = "^1.3.7"
 papermill = "^2.4.0"
+pdoc = "^14.4.0"
 pre-commit = "^3.3.3"
 pytest = "^5.2"
 sphinx = "^6.1.3"
 sphinx-markdown-builder = "^0.5.5"
 sphinx-rtd-theme = "^1.2.0"
 twine = "^4.0.2"
 
@@ -84,29 +80,30 @@
   "openai",
   "rpy2",
   "torch",
   "transformers",
   "pycocoevalcap",
   "torchmetrics",
   "levenshtein",
-  "datasets",
 ]
 llm = [
   "torch",
   "transformers",
   "openai",
   "pycocoevalcap",
   "torchmetrics",
   "levenshtein",
-  "datasets",
 ]
 pytorch = ["torch"]
 r-support = ["rpy2"]
 transformers = ["transformers"]
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.isort]
 known_first_party = "validmind"
 profile = "black"
+
+[tool.poetry.scripts]
+vm-create-new-test = "scripts.create_new_test:generate_test"
```

### Comparing `validmind-2.0.1/validmind/__init__.py` & `validmind-2.0.7/validmind/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,24 +46,25 @@
 warnings.simplefilter("ignore", category=NumbaDeprecationWarning)
 warnings.simplefilter("ignore", category=NumbaPendingDeprecationWarning)
 
 from .__version__ import __version__  # noqa: E402
 from .api_client import init
 from .api_client import log_figure as _log_figure_async
 from .api_client import log_metrics as _log_metrics_async
-from .api_client import log_test_results
+from .api_client import log_test_results, reload
 from .client import (  # noqa: E402
     get_test_suite,
     init_dataset,
     init_model,
     init_r_model,
     preview_template,
     run_documentation_tests,
     run_test_suite,
 )
+from .tests.decorator import metric
 from .unit_metrics import run_metric
 from .utils import run_async  # noqa: E402
 
 
 def log_metrics(metrics, inputs=None):
     """Logs metrics to ValidMind API.
 
@@ -101,15 +102,17 @@
     "datasets",
     "errors",
     "get_test_suite",
     "init",
     "init_dataset",
     "init_model",
     "init_r_model",
+    "metric",
     "preview_template",
+    "reload",
     "run_documentation_tests",
     "run_test_suite",
     "tests",
     "test_suites",
     "vm_models",
     "unit_metrics",
     # Framework Logging API
```

### Comparing `validmind-2.0.1/validmind/api_client.py` & `validmind-2.0.7/validmind/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -167,14 +167,26 @@
 
     logger.info(
         f"Connected to ValidMind. Project: {client_config.project['name']}"
         f" ({client_config.project['cuid']})"
     )
 
 
+def reload():
+    """Reconnect to the ValidMind API and reload the project configuration"""
+
+    try:
+        __ping()
+    except Exception as e:
+        # if the api host is https, assume we're not in dev mode and send to sentry
+        if _api_host.startswith("https://"):
+            send_single_error(e)
+        raise e
+
+
 async def __get_url(endpoint: str, params: Optional[Dict[str, str]] = None) -> str:
     if not _run_cuid:
         start_run()
 
     params = params or {}
     params["run_cuid"] = _run_cuid
 
@@ -309,34 +321,34 @@
     else:
         return await asyncio.gather(*[log_figure(figure) for figure in figures])
 
 
 async def log_metadata(
     content_id: str,
     text: Optional[str] = None,
-    extra_json: Optional[Dict[str, Any]] = None,
+    _json: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
     """Logs free-form metadata to ValidMind API.
 
     Args:
         content_id (str): Unique content identifier for the metadata
         text (str, optional): Free-form text to assign to the metadata. Defaults to None.
-        extra_json (dict, optional): Free-form key-value pairs to assign to the metadata. Defaults to None.
+        _json (dict, optional): Free-form key-value pairs to assign to the metadata. Defaults to None.
 
     Raises:
         Exception: If the API call fails
 
     Returns:
         dict: The response from the API
     """
     metadata_dict = {"content_id": content_id}
     if text is not None:
         metadata_dict["text"] = text
-    if extra_json is not None:
-        metadata_dict["extra_json"] = extra_json
+    if _json is not None:
+        metadata_dict["json"] = _json
 
     try:
         return await _post(
             "log_metadata",
             data=json.dumps(metadata_dict, cls=NumpyEncoder, allow_nan=False),
         )
     except Exception as e:
```

### Comparing `validmind-2.0.1/validmind/client.py` & `validmind-2.0.7/validmind/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
 """
 Client interface for all data and model validation functions
 """
 
 import pandas as pd
+import polars as pl
 
 from .api_client import _log_input as log_input
 from .client_config import client_config
 from .errors import (
     GetTestSuiteError,
     InitializeTestSuiteError,
     MissingDocumentationTemplate,
@@ -22,15 +23,21 @@
 from .logging import get_logger
 from .models.r_model import RModel
 from .template import get_template_test_suite
 from .template import preview_template as _preview_template
 from .test_suites import get_by_id as get_test_suite_by_id
 from .utils import get_dataset_info, get_model_info
 from .vm_models import TestInput, TestSuite, TestSuiteRunner
-from .vm_models.dataset import DataFrameDataset, NumpyDataset, TorchDataset, VMDataset
+from .vm_models.dataset import (
+    DataFrameDataset,
+    NumpyDataset,
+    PolarsDataset,
+    TorchDataset,
+    VMDataset,
+)
 from .vm_models.model import VMModel, get_model_class
 
 pd.option_context("format.precision", 2)
 
 logger = get_logger(__name__)
 
 
@@ -54,15 +61,15 @@
     """
     Initializes a VM Dataset, which can then be passed to other functions
     that can perform additional analysis and tests on the data. This function
     also ensures we are reading a valid dataset type. We only support Pandas
     DataFrames at the moment.
 
     Args:
-        dataset (pd.DataFrame): We only support Pandas DataFrames at the moment
+        dataset : dataset from various python libraries
         model (VMModel): ValidMind model object
         options (dict): A dictionary of options for the dataset
         targets (vm.vm.DatasetTargets): A list of target variables
         target_column (str): The name of the target column in the dataset
         feature_columns (list): A list of names of feature columns in the dataset
         extra_columns (dictionary):  A dictionary containing the names of the
         prediction_column and group_by_columns in the dataset
@@ -85,24 +92,37 @@
             "The 'type' argument to init_dataset() argument is deprecated and no longer required."
         )
 
     dataset_class = dataset.__class__.__name__
     input_id = input_id or "dataset"
 
     # Instantiate supported dataset types here
-    if dataset_class == "DataFrame":
+    if isinstance(dataset, pd.DataFrame):
         logger.info("Pandas dataset detected. Initializing VM Dataset instance...")
         vm_dataset = DataFrameDataset(
             input_id=input_id,
             raw_dataset=dataset,
             model=model,
             target_column=target_column,
             feature_columns=feature_columns,
             text_column=text_column,
             extra_columns=extra_columns,
+            target_class_labels=class_labels,
+            date_time_index=date_time_index,
+        )
+    elif isinstance(dataset, pl.DataFrame):
+        logger.info("Polars dataset detected. Initializing VM Dataset instance...")
+        vm_dataset = PolarsDataset(
+            input_id=input_id,
+            raw_dataset=dataset,
+            model=model,
+            target_column=target_column,
+            feature_columns=feature_columns,
+            text_column=text_column,
+            extra_columns=extra_columns,
             target_class_labels=class_labels,
             date_time_index=date_time_index,
         )
     elif dataset_class == "ndarray":
         logger.info("Numpy ndarray detected. Initializing VM Dataset instance...")
         vm_dataset = NumpyDataset(
             input_id=input_id,
```

### Comparing `validmind-2.0.1/validmind/client_config.py` & `validmind-2.0.7/validmind/client_config.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/classification/__init__.py` & `validmind-2.0.7/validmind/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/classification/customer_churn.py` & `validmind-2.0.7/validmind/datasets/classification/customer_churn.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     # This guarantees a 60/20/20 split
     train_df, validation_df = train_test_split(train_val_df, test_size=0.25)
 
     return train_df, validation_df, test_df
 
 
-def get_demo_test_config():
+def get_demo_test_config(test_suite=None):
     """
     Returns input configuration for the default documentation
     template assigned to this demo model
 
     The default documentation template uses the following inputs:
     - raw_dataset
     - train_dataset
@@ -77,15 +77,15 @@
     - When a test expects a "dataset" we use the raw_dataset
     - When a tets expects "datasets" we use the train_dataset and test_dataset
     - When a test expects a "model" we use the model
     - When a test expects "model" and "dataset" we use the model and test_dataset
     - The only exception is ClassifierPerformance since that runs twice: once
         with the train_dataset (in sample) and once with the test_dataset (out of sample)
     """
-    default_config = vm.get_test_suite().get_default_config()
+    default_config = (test_suite or vm.get_test_suite()).get_default_config()
 
     for _, test_config in default_config.items():
         if "model" in test_config["inputs"]:
             test_config["inputs"]["model"] = "model"
         if "datasets" in test_config["inputs"]:
             test_config["inputs"]["datasets"] = [
                 "train_dataset",
```

### Comparing `validmind-2.0.1/validmind/datasets/classification/datasets/bank_customer_churn.csv` & `validmind-2.0.7/validmind/datasets/classification/datasets/bank_customer_churn.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/classification/datasets/taiwan_credit.csv` & `validmind-2.0.7/validmind/datasets/classification/datasets/taiwan_credit.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/classification/taiwan_credit.py` & `validmind-2.0.7/validmind/datasets/classification/taiwan_credit.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/cluster/digits.py` & `validmind-2.0.7/validmind/datasets/cluster/digits.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/nlp/datasets/Covid_19.csv` & `validmind-2.0.7/validmind/datasets/nlp/datasets/Covid_19.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/nlp/twitter_covid_19.py` & `validmind-2.0.7/validmind/datasets/nlp/twitter_covid_19.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/__init__.py` & `validmind-2.0.7/validmind/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/california_housing.py` & `validmind-2.0.7/validmind/datasets/regression/california_housing.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/CPIAUCSL.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/CPIAUCSL.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/CSUSHPISA.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/CSUSHPISA.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/DRSFRMACBS.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/DRSFRMACBS.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/FEDFUNDS.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/FEDFUNDS.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/GDP.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/GDP.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/GDPC1.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/GDPC1.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/GS10.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/GS10.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/GS3.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/GS3.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/GS5.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/GS5.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/MORTGAGE30US.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/MORTGAGE30US.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred/UNRATE.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred/UNRATE.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/datasets/lending_club_loan_rates.csv` & `validmind-2.0.7/validmind/datasets/regression/datasets/lending_club_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/fred.py` & `validmind-2.0.7/validmind/datasets/regression/fred.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/lending_club.py` & `validmind-2.0.7/validmind/datasets/regression/lending_club.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl` & `validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl` & `validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl` & `validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl` & `validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl` & `validmind-2.0.7/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/errors.py` & `validmind-2.0.7/validmind/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """
     When the cache_results function is missing arguments.
     """
 
     pass
 
 
-class MissingModelPredictFnError(BaseError):
+class MissingOrInvalidModelPredictFnError(BaseError):
     """
     When the pytorch model is missing a predict function or its predict
     method does not have the expected arguments.
     """
 
     pass
 
@@ -311,14 +311,22 @@
     """
     When an unsupported model is used.
     """
 
     pass
 
 
+class UnsupportedModelForSHAPError(BaseError):
+    """
+    When an unsupported model is used for SHAP importance.
+    """
+
+    pass
+
+
 class SkipTestError(BaseError):
     """
     Useful error to throw when a test cannot be executed.
     """
 
     pass
 
@@ -357,10 +365,12 @@
 
 def should_raise_on_fail_fast(error) -> bool:
     """
     Determine whether an error should be raised when fail_fast is True.
     """
     error_class = error.__class__.__name__
     return error_class not in [
+        "MissingOrInvalidModelPredictFnError",
         "MissingRequiredTestInputError",
         "SkipTestError",
+        "UnsupportedModelForSHAPError",
     ]
```

### Comparing `validmind-2.0.1/validmind/html_templates/content_blocks.py` & `validmind-2.0.7/validmind/html_templates/content_blocks.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/input_registry.py` & `validmind-2.0.7/validmind/input_registry.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/logging.py` & `validmind-2.0.7/validmind/logging.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/models/__init__.py` & `validmind-2.0.7/validmind/models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/models/catboost.py` & `validmind-2.0.7/validmind/models/catboost.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/models/foundation.py` & `validmind-2.0.7/validmind/models/foundation.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/models/huggingface.py` & `validmind-2.0.7/validmind/models/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See the LICENSE file in the root of this repository for details.
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
 from dataclasses import dataclass
 
 import pandas as pd
 
-from validmind.errors import MissingModelPredictFnError
+from validmind.errors import MissingOrInvalidModelPredictFnError
 from validmind.logging import get_logger
 from validmind.vm_models.model import (
     ModelAttributes,
     VMModel,
     has_method_with_arguments,
 )
 
@@ -40,15 +40,15 @@
         )
 
     def predict_proba(self, *args, **kwargs):
         """
         Invoke predict_proba from underline model
         """
         if not has_method_with_arguments(self.model, "predict_proba", 1):
-            raise MissingModelPredictFnError(
+            raise MissingOrInvalidModelPredictFnError(
                 "Model requires a implementation of predict_proba method with 1 argument"
                 + " that is tensor features matrix"
             )
 
         if callable(getattr(self.model, "predict_proba", None)):
             return self.model.predict_proba(*args, **kwargs)[:, 1]
```

### Comparing `validmind-2.0.1/validmind/models/pytorch.py` & `validmind-2.0.7/validmind/models/pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright © 2023-2024 ValidMind Inc. All rights reserved.
 # See the LICENSE file in the root of this repository for details.
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
-from validmind.errors import MissingModelPredictFnError
+from validmind.errors import MissingOrInvalidModelPredictFnError
 from validmind.logging import get_logger
 from validmind.vm_models.model import (
     ModelAttributes,
     VMModel,
     has_method_with_arguments,
 )
 
@@ -37,28 +37,28 @@
         self._device_type = next(self.model.parameters()).device
 
     def predict_proba(self, *args, **kwargs):
         """
         Invoke predict_proba from underline model
         """
         if not has_method_with_arguments(self.model, "predict_proba", 1):
-            raise MissingModelPredictFnError(
+            raise MissingOrInvalidModelPredictFnError(
                 "Model requires a implemention of predict_proba method with 1 argument"
                 + " that is tensor features matrix"
             )
 
         if callable(getattr(self.model, "predict_proba", None)):
             return self.model.predict_proba(*args, **kwargs)[:, 1]
 
     def predict(self, *args, **kwargs):
         """
         Predict method for the model. This is a wrapper around the model's
         """
         if not has_method_with_arguments(self.model, "predict", 1):
-            raise MissingModelPredictFnError(
+            raise MissingOrInvalidModelPredictFnError(
                 "Model requires a implemention of predict method with 1 argument"
                 + " that is tensor features matrix"
             )
         import torch
 
         return self.model.predict(torch.tensor(args[0]).to(self.device_type))
```

### Comparing `validmind-2.0.1/validmind/models/r_model.py` & `validmind-2.0.7/validmind/models/r_model.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/models/sklearn.py` & `validmind-2.0.7/validmind/models/sklearn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright © 2023-2024 ValidMind Inc. All rights reserved.
 # See the LICENSE file in the root of this repository for details.
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
-from validmind.errors import MissingModelPredictFnError
+from validmind.errors import MissingOrInvalidModelPredictFnError
 from validmind.logging import get_logger
 from validmind.vm_models.model import (
     ModelAttributes,
     VMModel,
     has_method_with_arguments,
 )
 
@@ -36,17 +36,17 @@
         )
 
     def predict_proba(self, *args, **kwargs):
         """
         predict_proba (for classification) or predict (for regression) method
         """
         if not has_method_with_arguments(self.model, "predict_proba", 1):
-            raise MissingModelPredictFnError(
-                "Model requires a implemention of predict_proba method with 1 argument"
-                + " that is features matrix"
+            raise MissingOrInvalidModelPredictFnError(
+                f"SKlearn model {self.model.__class__} Model does not have a compatible predict_proba implementation."
+                + " Please assign predictions directly with vm_dataset.assign_predictions(model, prediction_values)"
             )
         if callable(getattr(self.model, "predict_proba", None)):
             return self.model.predict_proba(*args, **kwargs)[:, 1]
         return None
 
     def predict(self, *args, **kwargs):
         """
```

### Comparing `validmind-2.0.1/validmind/models/statsmodels.py` & `validmind-2.0.7/validmind/models/statsmodels.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/models/xgboost.py` & `validmind-2.0.7/validmind/models/xgboost.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/template.py` & `validmind-2.0.7/validmind/template.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/__init__.py` & `validmind-2.0.7/validmind/test_suites/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/classifier.py` & `validmind-2.0.7/validmind/test_suites/classifier.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/cluster.py` & `validmind-2.0.7/validmind/test_suites/cluster.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/embeddings.py` & `validmind-2.0.7/validmind/test_suites/embeddings.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/llm.py` & `validmind-2.0.7/validmind/test_suites/llm.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/nlp.py` & `validmind-2.0.7/validmind/test_suites/nlp.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/parameters_optimization.py` & `validmind-2.0.7/validmind/test_suites/parameters_optimization.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/regression.py` & `validmind-2.0.7/validmind/test_suites/regression.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/statsmodels_timeseries.py` & `validmind-2.0.7/validmind/test_suites/statsmodels_timeseries.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/summarization.py` & `validmind-2.0.7/validmind/test_suites/summarization.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/tabular_datasets.py` & `validmind-2.0.7/validmind/test_suites/tabular_datasets.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/text_data.py` & `validmind-2.0.7/validmind/test_suites/text_data.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/test_suites/time_series.py` & `validmind-2.0.7/validmind/test_suites/time_series.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/__init__.py` & `validmind-2.0.7/validmind/tests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from IPython.display import display
 from ipywidgets import HTML
 from markdown import markdown
 
 from ..errors import LoadTestError
 from ..html_templates.content_blocks import test_content_block_html
 from ..logging import get_logger
+from ..unit_metrics.composite import load_composite_metric
 from ..utils import clean_docstring, format_dataframe, fuzzy_match, test_id_to_name
 from ..vm_models import TestContext, TestInput
 from .__types__ import ExternalTestProvider
 from .test_providers import GithubTestProvider, LocalTestProvider
 
 logger = get_logger(__name__)
 
@@ -39,14 +40,15 @@
     "LocalTestProvider",
 ]
 
 __tests = None
 __test_classes = None
 
 __test_providers: Dict[str, ExternalTestProvider] = {}
+__custom_tests: Dict[str, object] = {}
 
 
 def _test_description(test_class, truncate=True):
     if truncate and len(test_class.__doc__.split("\n")) > 5:
         return test_class.__doc__.strip().split("\n")[0] + "..."
 
     return test_class.__doc__
@@ -256,21 +258,21 @@
     # test ID "validmind.data_validation.ClassImbalance:data_id_1,"
     # where the test ID extension is "data_id_1".
     parts = test_id.split(":")[0].split(".")
 
     error = None
     namespace = parts[0]
 
-    if namespace != "validmind" and namespace not in __test_providers:
-        error = (
-            f"Unable to load test {test_id}. "
-            f"No Test Provider found for the namespace: {namespace}."
-        )
+    if test_id.split(":")[0] in __custom_tests:
+        test = __custom_tests[test_id.split(":")[0]]
 
-    if namespace == "validmind":
+    elif test_id.startswith("validmind.composite_metric"):
+        test = load_composite_metric(test_id)
+
+    elif namespace == "validmind":
         test_module = ".".join(parts[1:-1])
         test_class = parts[-1]
 
         try:
             full_path = f"validmind.tests.{test_module}.{test_class}"
 
             if reload and full_path in sys.modules:
@@ -280,14 +282,20 @@
 
             test = getattr(module, test_class)
         except ModuleNotFoundError as e:
             error = f"Unable to load test {test_id}. {e}"
         except AttributeError:
             error = f"Unable to load test {test_id}. Class not in module: {test_class}"
 
+    elif namespace != "validmind" and namespace not in __test_providers:
+        error = (
+            f"Unable to load test {test_id}. "
+            f"No Test Provider found for the namespace: {namespace}."
+        )
+
     elif namespace in __test_providers:
         try:
             test = __test_providers[namespace].load_test(test_id.split(".", 1)[1])
         except Exception as e:
             error = (
                 f"Unable to load test {test_id} from test  provider: "
                 f"{__test_providers[namespace]}\n Got Exception: {e}"
@@ -342,29 +350,55 @@
                 ),
                 table_display="table" if details["Params"] else "none",
             )
         )
     )
 
 
-def run_test(test_id, params: dict = None, inputs=None, output_template=None, **kwargs):
+def run_test(
+    test_id: str = None,
+    name: str = None,
+    unit_metrics: list = None,
+    params: dict = None,
+    inputs=None,
+    output_template=None,
+    **kwargs,
+):
     """Run a test by test ID
 
     Args:
-        test_id (str): The test ID
+        test_id (str, option): The test ID to run - required when running a single test
+            i.e. when not running multiple unit metrics
+        name (str, optional): The name of the test (used to create a composite metric
+            out of multiple unit metrics) - required when running multiple unit metrics
+        unit_metrics (list, optional): A list of unit metric IDs to run as a composite
+            metric - required when running multiple unit metrics
         params (dict, optional): A dictionary of params to override the default params
         inputs: A dictionary of test inputs to pass to the Test
         output_template (str, optional): A template to use for customizing the output
         **kwargs: Any extra arguments will be passed in via the TestInput object. i.e.:
             - dataset: A validmind Dataset object or a Pandas DataFrame
             - model: A model to use for the test
             - models: A list of models to use for the test
             other inputs can be accessed inside the test via `self.inputs["input_name"]`
     """
-    TestClass = load_test(test_id, reload=True)
+    if not test_id and not name and not unit_metrics:
+        raise ValueError(
+            "`test_id` or `name` and `unit_metrics` must be provided to run a test"
+        )
+
+    if (unit_metrics and not name) or (name and not unit_metrics):
+        raise ValueError("`name` and `unit_metrics` must be provided together")
+
+    if unit_metrics:
+        TestClass = load_composite_metric(unit_metrics=unit_metrics, metric_name=name)
+        test_id = f"validmind.composite_metric.{name}"
+    else:
+        TestClass = load_test(test_id, reload=True)
+
     test = TestClass(
         test_id=test_id,
         context=TestContext(),
         inputs=TestInput({**kwargs, **(inputs or {})}),
         output_template=output_template,
         params=params,
     )
@@ -379,7 +413,11 @@
     """Register an external test provider
 
     Args:
         namespace (str): The namespace of the test provider
         test_provider (ExternalTestProvider): The test provider
     """
     __test_providers[namespace] = test_provider
+
+
+def _register_custom_test(test_id: str, test_class: object):
+    __custom_tests[test_id] = test_class
```

### Comparing `validmind-2.0.1/validmind/tests/__types__.py` & `validmind-2.0.7/validmind/tests/__types__.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/ACFandPACFPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/ACFandPACFPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/ANOVAOneWayTable.py` & `validmind-2.0.7/validmind/tests/data_validation/ANOVAOneWayTable.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/AutoAR.py` & `validmind-2.0.7/validmind/tests/data_validation/AutoAR.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/AutoMA.py` & `validmind-2.0.7/validmind/tests/data_validation/AutoMA.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/AutoSeasonality.py` & `validmind-2.0.7/validmind/tests/data_validation/AutoSeasonality.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/AutoStationarity.py` & `validmind-2.0.7/validmind/tests/data_validation/AutoStationarity.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/BivariateFeaturesBarPlots.py` & `validmind-2.0.7/validmind/tests/data_validation/BivariateFeaturesBarPlots.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/BivariateHistograms.py` & `validmind-2.0.7/validmind/tests/data_validation/BivariateHistograms.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/BivariateScatterPlots.py` & `validmind-2.0.7/validmind/tests/data_validation/BivariateScatterPlots.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/ChiSquaredFeaturesTable.py` & `validmind-2.0.7/validmind/tests/data_validation/ChiSquaredFeaturesTable.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/ClassImbalance.py` & `validmind-2.0.7/validmind/tests/data_validation/ClassImbalance.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/DatasetDescription.py` & `validmind-2.0.7/validmind/tests/data_validation/DatasetDescription.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         results = []
         for ds_field in self.infer_datatype(self.inputs.dataset.df):
             self.describe_dataset_field(self.inputs.dataset.df, ds_field)
             results.append(ds_field)
         return self.cache_results(results)
 
     def infer_datatype(self, df):
-
         vm_dataset_variables = {}
         typeset = ProfilingTypeSet(Settings())
         variable_types = typeset.infer_type(df)
 
         for column, type in variable_types.items():
             if str(type) == "Unsupported":
                 if df[column].isnull().all():
```

### Comparing `validmind-2.0.1/validmind/tests/data_validation/DatasetSplit.py` & `validmind-2.0.7/validmind/tests/data_validation/DatasetSplit.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/DefaultRatesbyRiskBandPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/DefaultRatesbyRiskBandPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/DescriptiveStatistics.py` & `validmind-2.0.7/validmind/tests/data_validation/DescriptiveStatistics.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/Duplicates.py` & `validmind-2.0.7/validmind/tests/data_validation/Duplicates.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/EngleGrangerCoint.py` & `validmind-2.0.7/validmind/tests/data_validation/EngleGrangerCoint.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/FeatureTargetCorrelationPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/FeatureTargetCorrelationPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/HeatmapFeatureCorrelations.py` & `validmind-2.0.7/validmind/tests/data_validation/HeatmapFeatureCorrelations.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/HighCardinality.py` & `validmind-2.0.7/validmind/tests/data_validation/HighCardinality.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/HighPearsonCorrelation.py` & `validmind-2.0.7/validmind/tests/data_validation/HighPearsonCorrelation.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/IQROutliersBarPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/IQROutliersBarPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/IQROutliersTable.py` & `validmind-2.0.7/validmind/tests/data_validation/IQROutliersTable.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/IsolationForestOutliers.py` & `validmind-2.0.7/validmind/tests/data_validation/IsolationForestOutliers.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/LaggedCorrelationHeatmap.py` & `validmind-2.0.7/validmind/tests/data_validation/LaggedCorrelationHeatmap.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/MissingValues.py` & `validmind-2.0.7/validmind/tests/data_validation/MissingValues.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/MissingValuesBarPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/MissingValuesBarPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/MissingValuesRisk.py` & `validmind-2.0.7/validmind/tests/data_validation/MissingValuesRisk.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/PearsonCorrelationMatrix.py` & `validmind-2.0.7/validmind/tests/data_validation/PearsonCorrelationMatrix.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/PiTCreditScoresHistogram.py` & `validmind-2.0.7/validmind/tests/data_validation/PiTCreditScoresHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/PiTPDHistogram.py` & `validmind-2.0.7/validmind/tests/data_validation/PiTPDHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/RollingStatsPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/RollingStatsPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/ScatterPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/ScatterPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/SeasonalDecompose.py` & `validmind-2.0.7/validmind/tests/data_validation/SeasonalDecompose.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/Skewness.py` & `validmind-2.0.7/validmind/tests/data_validation/Skewness.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/SpreadPlot.py` & `validmind-2.0.7/validmind/tests/data_validation/SpreadPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TabularCategoricalBarPlots.py` & `validmind-2.0.7/validmind/tests/data_validation/TabularCategoricalBarPlots.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TabularDateTimeHistograms.py` & `validmind-2.0.7/validmind/tests/data_validation/TabularDateTimeHistograms.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TabularDescriptionTables.py` & `validmind-2.0.7/validmind/tests/data_validation/TabularDescriptionTables.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TabularNumericalHistograms.py` & `validmind-2.0.7/validmind/tests/data_validation/TabularNumericalHistograms.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TargetRateBarPlots.py` & `validmind-2.0.7/validmind/tests/data_validation/TargetRateBarPlots.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TimeSeriesFrequency.py` & `validmind-2.0.7/validmind/tests/data_validation/TimeSeriesFrequency.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TimeSeriesHistogram.py` & `validmind-2.0.7/validmind/tests/data_validation/TimeSeriesHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TimeSeriesLinePlot.py` & `validmind-2.0.7/validmind/tests/data_validation/TimeSeriesLinePlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TimeSeriesMissingValues.py` & `validmind-2.0.7/validmind/tests/data_validation/TimeSeriesMissingValues.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TimeSeriesOutliers.py` & `validmind-2.0.7/validmind/tests/data_validation/TimeSeriesOutliers.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/TooManyZeroValues.py` & `validmind-2.0.7/validmind/tests/data_validation/TooManyZeroValues.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/UniqueRows.py` & `validmind-2.0.7/validmind/tests/data_validation/UniqueRows.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/WOEBinPlots.py` & `validmind-2.0.7/validmind/tests/data_validation/WOEBinPlots.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/WOEBinTable.py` & `validmind-2.0.7/validmind/tests/data_validation/WOEBinTable.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/nlp/CommonWords.py` & `validmind-2.0.7/validmind/tests/data_validation/nlp/CommonWords.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/nlp/Hashtags.py` & `validmind-2.0.7/validmind/tests/data_validation/nlp/Hashtags.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/nlp/Mentions.py` & `validmind-2.0.7/validmind/tests/data_validation/nlp/Mentions.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/nlp/Punctuations.py` & `validmind-2.0.7/validmind/tests/data_validation/nlp/Punctuations.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/data_validation/nlp/StopWords.py` & `validmind-2.0.7/validmind/tests/data_validation/nlp/StopWords.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from validmind.vm_models import (
     Figure,
     ResultSummary,
     ResultTable,
     ResultTableMetadata,
     ThresholdTest,
     ThresholdTestResult,
-    VMDataset,
 )
 
 
 @dataclass
 class StopWords(ThresholdTest):
     """
     Evaluates and visualizes the frequency of English stop words in a text dataset against a defined threshold.
@@ -82,25 +81,21 @@
         df = pd.DataFrame(results[0].values, columns=["Word", "Percentage"])
 
         return ResultSummary(
             results=[
                 ResultTable(
                     data=df,
                     metadata=ResultTableMetadata(
-                        title=f"Class Imbalance Results for Column {self.inputs.dataset.target_column}"
+                        title=f"Stop words results for column '{self.inputs.dataset.target_column}'"
                     ),
                 )
             ]
         )
 
     def run(self):
-        # Can only run this test if we have a Dataset object
-        if not isinstance(self.inputs.dataset, VMDataset):
-            raise ValueError("ClassImbalance requires a validmind Dataset object")
-
         text_column = self.inputs.dataset.text_column
 
         def create_corpus(df, text_column):
             corpus = []
             for x in df[text_column].str.split():
                 for i in x:
                     corpus.append(i)
```

### Comparing `validmind-2.0.1/validmind/tests/data_validation/nlp/TextDescription.py` & `validmind-2.0.7/validmind/tests/data_validation/nlp/TextDescription.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,17 +88,20 @@
             sentences = nltk.sent_tokenize(text)
             words = nltk.word_tokenize(text)
             paragraphs = text.split("\n\n")
 
             total_words = len(words)
             total_sentences = len(sentences)
             avg_sentence_length = round(
-                sum(len(sentence.split()) for sentence in sentences) / total_sentences
-                if total_sentences
-                else 0,
+                (
+                    sum(len(sentence.split()) for sentence in sentences)
+                    / total_sentences
+                    if total_sentences
+                    else 0
+                ),
                 1,
             )
             total_paragraphs = len(paragraphs)
 
             results.append(
                 [total_words, total_sentences, avg_sentence_length, total_paragraphs]
             )
@@ -157,47 +160,55 @@
             df, text_column, unwanted_tokens, num_top_words, lang
         )
         combined_df = pd.concat([gen_metrics_df, vocab_metrics_df], axis=1)
 
         return combined_df
 
     def run(self):
+        # Enforce that text_column must be provided as part of the params
+        if self.inputs.dataset.text_column is None:
+            raise ValueError("A 'text_column' must be provided to run this test.")
+
         # Can only run this test if we have a Dataset object
         if not isinstance(self.inputs.dataset, VMDataset):
-            raise ValueError("TextDescretion requires a validmind Dataset object")
+            raise ValueError("TextDescription requires a validmind Dataset object")
 
         df_text_description = self.text_description_table(
             self.inputs.dataset.df, self.params
         )
 
         # Define the combinations you want to plot
         combinations_to_plot = [
             ("Total Words", "Total Sentences"),
             ("Total Words", "Total Unique Words"),
             ("Total Sentences", "Avg Sentence Length"),
             ("Total Unique Words", "Lexical Diversity"),
         ]
         params = {"combinations_to_plot": combinations_to_plot}
-        figures = self.text_description_scatter_plot(df_text_description, params)
+        figures = self.text_description_plots(df_text_description, params)
 
         return self.cache_results(
             figures=figures,
         )
 
     # Function to plot scatter plots for specified combinations using Plotly
-    def text_description_scatter_plot(self, df, params):
+    def text_description_plots(self, df, params):
         combinations_to_plot = params["combinations_to_plot"]
         figures = []
         # Create hist plots for each column
         for i, column in enumerate(df.columns):
             fig = px.histogram(df, x=column)
             fig.update_layout(bargap=0.2)
-            figures.append(Figure(for_object=self, key=self.key, figure=fig))
+            # Generate a unique key for each histogram using the column name and index
+            histogram_key = f"{self.name}_histogram_{column}_{i}"
+            figures.append(Figure(for_object=self, key=histogram_key, figure=fig))
 
-        for metric1, metric2 in combinations_to_plot:
+        for j, (metric1, metric2) in enumerate(combinations_to_plot):
             fig = px.scatter(
                 df, x=metric1, y=metric2, title=f"Scatter Plot: {metric1} vs {metric2}"
             )
-            figures.append(Figure(for_object=self, key=self.key, figure=fig))
+            # Generate a unique key for each scatter plot using the metric names and index
+            scatter_key = f"{self.name}_scatter_{metric1}_vs_{metric2}_{j}"
+            figures.append(Figure(for_object=self, key=scatter_key, figure=fig))
         plt.close("all")
 
         return figures
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/BertScore.py` & `validmind-2.0.7/validmind/tests/model_validation/BertScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/BertScoreAggregate.py` & `validmind-2.0.7/validmind/tests/model_validation/BertScoreAggregate.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/BleuScore.py` & `validmind-2.0.7/validmind/tests/model_validation/BleuScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/ClusterSizeDistribution.py` & `validmind-2.0.7/validmind/tests/model_validation/ClusterSizeDistribution.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/ContextualRecall.py` & `validmind-2.0.7/validmind/tests/model_validation/ContextualRecall.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/ModelMetadata.py` & `validmind-2.0.7/validmind/tests/model_validation/ModelMetadata.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/RegardHistogram.py` & `validmind-2.0.7/validmind/tests/model_validation/RegardHistogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,29 +54,27 @@
 
     def _get_datasets(self):
         if not hasattr(self, "model"):
             raise AttributeError("The 'model' attribute is missing.")
 
         y_true = list(itertools.chain.from_iterable(self.inputs.dataset.y))
         y_pred = self.inputs.dataset.y_pred(self.inputs.model.input_id)
-        input_text = self.inputs.dataset.df[self.inputs.dataset.text_column]
 
-        if not len(y_true) == len(y_pred) == len(input_text):
+        if not len(y_true) == len(y_pred):
             raise ValueError(
-                "Inconsistent lengths among input text, true summaries, and predicted summaries."
+                "Inconsistent lengths among true summaries and predicted summaries."
             )
 
-        return input_text, y_true, y_pred
+        return y_true, y_pred
 
     def regard_histogram(self):
         regard_tool = evaluate.load("regard")
-        input_text, y_true, y_pred = self._get_datasets()
+        y_true, y_pred = self._get_datasets()
 
         dataframes = {
-            "Input Text": input_text,
             "Target Text": y_true,
             "Predicted Summaries": y_pred,
         }
 
         total_text_columns = len(dataframes)
         total_rows = total_text_columns * 2
 
@@ -97,14 +95,15 @@
                 for cat in categories_order
             ],
             shared_xaxes=True,
             vertical_spacing=0.1,
         )
 
         row_offset = 0
+
         for column_name, column_data in dataframes.items():
             results = regard_tool.compute(data=column_data)["regard"]
             regard_dicts = [
                 dict((x["label"], x["score"]) for x in sublist) for sublist in results
             ]
 
             for idx, category in enumerate(categories_order, start=1):
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/RegardScore.py` & `validmind-2.0.7/validmind/tests/model_validation/RegardScore.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,27 @@
 
     def _get_datasets(self):
         if not hasattr(self, "model"):
             raise AttributeError("The 'model' attribute is missing.")
 
         y_true = list(itertools.chain.from_iterable(self.inputs.dataset.y))
         y_pred = self.inputs.dataset.y_pred(self.inputs.model.input_id)
-        input_text = self.inputs.dataset.df[self.inputs.dataset.text_column]
 
-        if not len(y_true) == len(y_pred) == len(input_text):
+        if not len(y_true) == len(y_pred):
             raise ValueError(
                 "Inconsistent lengths among input text, true summaries, and predicted summaries."
             )
 
-        return input_text, y_true, y_pred
+        return y_true, y_pred
 
     def regard_line_plot(self):
         regard_tool = evaluate.load("regard")
-        input_text, y_true, y_pred = self._get_datasets()
+        y_true, y_pred = self._get_datasets()
 
         dataframes = {
-            "Input Text": input_text,
             "Target Text": y_true,
             "Predicted Summaries": y_pred,
         }
 
         total_text_columns = len(dataframes)
         total_rows = total_text_columns * 2
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/RougeMetrics.py` & `validmind-2.0.7/validmind/tests/model_validation/RougeMetrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     }
 
     def run(self):
         r_metrics = self.params["rouge_metrics"]
         if r_metrics is None:
             raise ValueError("rouge_metrics must be provided in params")
 
-        # With all
         if not (
             set(self.default_params.get("rouge_metrics")).intersection(r_metrics)
             == set(r_metrics)
         ):
             raise ValueError(
                 f"Invalid metrics from {self.default_params.get('rouge_metrics')}"
             )
@@ -93,20 +92,21 @@
         score_list = []
         for y_t, y_p in zip(y_true, y_pred):
             scores = rouge.get_scores(y_p, y_t, avg=True)
             score_list.append(scores)
 
         metrics_df = pd.DataFrame(score_list)
         figures = []
+
         for m in metrics_df.columns:
             df_scores = pd.DataFrame(metrics_df[m].tolist())
             # Visualization part
             fig = go.Figure()
 
-            # Adding the line plots
+            # Adding the line plots for precision, recall, and F1-score with lines and markers
             fig.add_trace(
                 go.Scatter(
                     x=df_scores.index,
                     y=df_scores["p"],
                     mode="lines+markers",
                     name="Precision",
                 )
@@ -125,19 +125,21 @@
                     y=df_scores["f"],
                     mode="lines+markers",
                     name="F1 Score",
                 )
             )
 
             fig.update_layout(
-                title="ROUGE Scores for Each Row",
+                title=f"ROUGE Scores for {m}",
                 xaxis_title="Row Index",
                 yaxis_title="Score",
             )
-            k = m.replace("-", "")
+
+            # Ensure a unique key for each metric
+            k = f"{m.replace('-', '')}_{len(figures)}"
             figures.append(
                 Figure(
                     for_object=self,
                     key=k,
                     figure=fig,
                 )
             )
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/RougeMetricsAggregate.py` & `validmind-2.0.7/validmind/tests/model_validation/RougeMetricsAggregate.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/TokenDisparity.py` & `validmind-2.0.7/validmind/tests/model_validation/TokenDisparity.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/ToxicityHistogram.py` & `validmind-2.0.7/validmind/tests/model_validation/ToxicityHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/ToxicityScore.py` & `validmind-2.0.7/validmind/tests/model_validation/ToxicityScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/ClusterDistribution.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/ClusterDistribution.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/CosineSimilarityDistribution.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/CosineSimilarityDistribution.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/DescriptiveAnalytics.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/DescriptiveAnalytics.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,34 +55,29 @@
     required_inputs = ["model", "dataset"]
     metadata = {
         "task_types": ["feature_extraction"],
         "tags": ["llm", "text_data", "text_embeddings", "visualization"],
     }
 
     def run(self):
-        mean = np.mean(self.inputs.dataset.y_pred(self.inputs.model.input_id))
-        median = np.median(self.inputs.dataset.y_pred(self.inputs.model.input_id))
-        std = np.std(self.inputs.dataset.y_pred(self.inputs.model.input_id))
+        # Assuming y_pred returns a 2D array of embeddings [samples, features]
+        preds = self.inputs.dataset.y_pred(self.inputs.model.input_id)
+
+        # Calculate statistics across the embedding dimensions, not across all embeddings
+        means = np.mean(preds, axis=0)  # Mean of each feature across all samples
+        medians = np.median(preds, axis=0)  # Median of each feature across all samples
+        stds = np.std(preds, axis=0)  # Std. dev. of each feature across all samples
+
+        # Plot histograms of the calculated statistics
+        mean_fig = px.histogram(x=means, title="Distribution of Embedding Means")
+        median_fig = px.histogram(x=medians, title="Distribution of Embedding Medians")
+        std_fig = px.histogram(
+            x=stds, title="Distribution of Embedding Standard Deviations"
+        )
 
         return self.cache_results(
             figures=[
-                Figure(
-                    for_object=self,
-                    key=self.key,
-                    figure=px.histogram(mean, title="Distribution of Embedding Means"),
-                ),
-                Figure(
-                    for_object=self,
-                    key=self.key,
-                    figure=px.histogram(
-                        median, title="Distribution of Embedding Medians"
-                    ),
-                ),
-                Figure(
-                    for_object=self,
-                    key=self.key,
-                    figure=px.histogram(
-                        std, title="Distribution of Embedding Standard Deviations"
-                    ),
-                ),
+                Figure(for_object=self, key=f"{self.key}_mean", figure=mean_fig),
+                Figure(for_object=self, key=f"{self.key}_median", figure=median_fig),
+                Figure(for_object=self, key=f"{self.key}_std", figure=std_fig),
             ],
         )
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/EmbeddingsVisualization2D.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/EmbeddingsVisualization2D.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysis.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysis.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisKeyword.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisKeyword.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisRandomNoise.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisRandomNoise.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisSynonyms.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisSynonyms.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/embeddings/StabilityAnalysisTranslation.py` & `validmind-2.0.7/validmind/tests/model_validation/embeddings/StabilityAnalysisTranslation.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/AdjustedMutualInformation.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/AdjustedMutualInformation.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/AdjustedRandIndex.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/AdjustedRandIndex.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ClassifierPerformance.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ClassifierPerformance.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,11 +127,13 @@
     def y_pred(self):
         return self.inputs.dataset.y_pred(model_id=self.inputs.model.input_id)
 
     def run(self):
         y_true = self.y_true()
         class_pred = self.y_pred()
 
-        report = metrics.classification_report(y_true, class_pred, output_dict=True)
+        report = metrics.classification_report(
+            y_true, class_pred, output_dict=True, zero_division=0
+        )
         report["roc_auc"] = multiclass_roc_auc_score(y_true, class_pred)
 
         return self.cache_results(report)
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ClusterCosineSimilarity.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ClusterCosineSimilarity.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ClusterPerformance.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ClusterPerformance.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ClusterPerformanceMetrics.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ClusterPerformanceMetrics.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/CompletenessScore.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/CompletenessScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ConfusionMatrix.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/FowlkesMallowsScore.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/FowlkesMallowsScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/HomogeneityScore.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/HomogeneityScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/HyperParametersTuning.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/HyperParametersTuning.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/KMeansClustersOptimization.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/KMeansClustersOptimization.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/MinimumAccuracy.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/MinimumAccuracy.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/MinimumF1Score.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/MinimumF1Score.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/MinimumROCAUCScore.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/MinimumROCAUCScore.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ModelsPerformanceComparison.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ModelsPerformanceComparison.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/OverfitDiagnosis.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/OverfitDiagnosis.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/PermutationFeatureImportance.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/PermutationFeatureImportance.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/PopulationStabilityIndex.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/PopulationStabilityIndex.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/PrecisionRecallCurve.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/PrecisionRecallCurve.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/ROCCurve.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/ROCCurve.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/RegressionErrors.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/RegressionErrors.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/RegressionModelsPerformanceComparison.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/RegressionModelsPerformanceComparison.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/RegressionR2Square.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/RegressionR2Square.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/RobustnessDiagnosis.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/RobustnessDiagnosis.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/SHAPGlobalImportance.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/SHAPGlobalImportance.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import warnings
 from dataclasses import dataclass
 
 import matplotlib.pyplot as plt
 import shap
 
+from validmind.errors import UnsupportedModelForSHAPError
 from validmind.logging import get_logger
 from validmind.vm_models import Figure, Metric
 
 logger = get_logger(__name__)
 
 
 @dataclass
@@ -68,14 +69,17 @@
             "sklearn",
             "binary_classification",
             "multiclass_classification",
             "feature_importance",
             "visualization",
         ],
     }
+    default_params = {
+        "kernel_explainer_samples": 10,
+    }
 
     def _generate_shap_plot(self, type_, shap_values, x_test):
         """
         Plots two types of SHAP global importance (SHAP).
         :params type: mean, summary
         :params shap_values: a matrix
         :params x_test:
@@ -123,30 +127,52 @@
         warnings.filterwarnings("ignore", category=UserWarning)
 
         # Any tree based model can go here
         if (
             model_class == "XGBClassifier"
             or model_class == "RandomForestClassifier"
             or model_class == "CatBoostClassifier"
+            or model_class == "DecisionTreeClassifier"
         ):
             explainer = shap.TreeExplainer(trained_model)
         elif (
             model_class == "LogisticRegression"
             or model_class == "XGBRegressor"
             or model_class == "LinearRegression"
+            or model_class == "LinearSVC"
         ):
             explainer = shap.LinearExplainer(trained_model, self.inputs.dataset.x)
+        elif model_class == "SVC":
+            # KernelExplainer is slow so we use shap.sample to speed it up
+            explainer = shap.KernelExplainer(
+                trained_model.predict,
+                shap.sample(
+                    self.inputs.dataset.x,
+                    self.params["kernel_explainer_samples"],
+                ),
+            )
+        else:
+            raise UnsupportedModelForSHAPError(
+                f"Model {model_class} not supported for SHAP importance."
+            )
+
+        # KernelExplainer is slow so we use shap.sample to speed it up
+        if isinstance(explainer, shap.KernelExplainer):
+            shap_sample = shap.sample(
+                self.inputs.dataset.x,
+                self.params["kernel_explainer_samples"],
+            )
         else:
-            raise ValueError(f"Model {model_class} not supported for SHAP importance.")
+            shap_sample = self.inputs.dataset.x
 
-        shap_values = explainer.shap_values(self.inputs.dataset.x)
+        shap_values = explainer.shap_values(shap_sample)
 
         figures = [
-            self._generate_shap_plot("mean", shap_values, self.inputs.dataset.x),
-            self._generate_shap_plot("summary", shap_values, self.inputs.dataset.x),
+            self._generate_shap_plot("mean", shap_values, shap_sample),
+            self._generate_shap_plot("summary", shap_values, shap_sample),
         ]
 
         # restore warnings
         warnings.filterwarnings("default", category=UserWarning)
 
         return self.cache_results(figures=figures)
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/SilhouettePlot.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/SilhouettePlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/TrainingTestDegradation.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/TrainingTestDegradation.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,31 +125,37 @@
         y_train_true = y_train_true.astype(y_train_pred.dtype)
 
         y_test_true = self.inputs.datasets[1].y
         y_test_pred = self.inputs.datasets[1].y_pred(self.inputs.model.input_id)
         y_test_true = y_test_true.astype(y_test_pred.dtype)
 
         report_train = metrics.classification_report(
-            y_train_true, y_train_pred, output_dict=True
+            y_train_true, y_train_pred, output_dict=True, zero_division=0
         )
         report_train["roc_auc"] = multiclass_roc_auc_score(y_train_true, y_train_pred)
 
         report_test = metrics.classification_report(
-            y_test_true, y_test_pred, output_dict=True
+            y_test_true, y_test_pred, output_dict=True, zero_division=0
         )
         report_test["roc_auc"] = multiclass_roc_auc_score(y_test_true, y_test_pred)
 
         classes = {str(i) for i in unique(y_train_true)}
 
         test_results = []
         for class_name in classes:
             for metric_name in ["precision", "recall", "f1-score"]:
                 train_score = report_train[class_name][metric_name]
                 test_score = report_test[class_name][metric_name]
-                degradation = (train_score - test_score) / train_score
+
+                # If training score is 0, degradation is assumed to be 100%
+                if train_score == 0:
+                    degradation = 1.0
+                else:
+                    degradation = (train_score - test_score) / train_score
+
                 passed = degradation < self.params["max_threshold"]
                 test_results.append(
                     ThresholdTestResult(
                         test_name=metric_name,
                         passed=passed,
                         values={
                             "class": class_name,
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/VMeasure.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/VMeasure.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/sklearn/WeakspotsDiagnosis.py` & `validmind-2.0.7/validmind/tests/model_validation/sklearn/WeakspotsDiagnosis.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ADF.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ADF.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ADFTest.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ADFTest.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/AutoARIMA.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/AutoARIMA.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/BoxPierce.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/BoxPierce.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/DFGLSArch.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/DFGLSArch.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/DurbinWatsonTest.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/DurbinWatsonTest.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/FeatureImportanceAndSignificance.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/FeatureImportanceAndSignificance.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/GINITable.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/GINITable.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/JarqueBera.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/JarqueBera.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/KPSS.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/KPSS.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/KolmogorovSmirnov.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/KolmogorovSmirnov.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/LJungBox.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/LJungBox.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/Lilliefors.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/Lilliefors.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/LogRegressionConfusionMatrix.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/LogRegressionConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/LogisticRegCumulativeProb.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/LogisticRegCumulativeProb.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/LogisticRegPredictionHistogram.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/LogisticRegPredictionHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/PDRatingClassPlot.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/PDRatingClassPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/PhillipsPerronArch.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/PhillipsPerronArch.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionCoeffsPlot.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionCoeffsPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionFeatureSignificance.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionFeatureSignificance.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlot.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlotLevels.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelForecastPlotLevels.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelInsampleComparison.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelInsampleComparison.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelOutsampleComparison.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelOutsampleComparison.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelSensitivityPlot.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelSensitivityPlot.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelSummary.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelSummary.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelsCoeffs.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelsCoeffs.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RegressionModelsPerformance.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RegressionModelsPerformance.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 "out_of_sample_performance": out_of_sample_results,
             }
         )
 
     def sample_performance_ols(self, models, datasets):
         evaluation_results = []
 
-        for (model, dataset) in zip(models, datasets):
+        for model, dataset in zip(models, datasets):
             X_columns = dataset.get_features_columns()
             y_true = dataset.y
             y_pred = dataset.y_pred(model.input_id)
 
             # Extract R-squared and Adjusted R-squared
             r2 = r2_score(y_true, y_pred)
             mse = mean_squared_error(y_true, y_pred)
```

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ResidualsVisualInspection.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ResidualsVisualInspection.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/RunsTest.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/RunsTest.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ScorecardBucketHistogram.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ScorecardBucketHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ScorecardHistogram.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ScorecardHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ScorecardProbabilitiesHistogram.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ScorecardProbabilitiesHistogram.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ShapiroWilk.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ShapiroWilk.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/model_validation/statsmodels/ZivotAndrewsArch.py` & `validmind-2.0.7/validmind/tests/model_validation/statsmodels/ZivotAndrewsArch.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/Bias.py` & `validmind-2.0.7/validmind/tests/prompt_validation/Bias.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/Clarity.py` & `validmind-2.0.7/validmind/tests/prompt_validation/Clarity.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/Conciseness.py` & `validmind-2.0.7/validmind/tests/prompt_validation/Conciseness.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/Delimitation.py` & `validmind-2.0.7/validmind/tests/prompt_validation/Delimitation.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/NegativeInstruction.py` & `validmind-2.0.7/validmind/tests/prompt_validation/NegativeInstruction.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/Robustness.py` & `validmind-2.0.7/validmind/tests/prompt_validation/Robustness.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/Specificity.py` & `validmind-2.0.7/validmind/tests/prompt_validation/Specificity.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/tests/prompt_validation/ai_powered_test.py` & `validmind-2.0.7/validmind/tests/prompt_validation/ai_powered_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         return (
             self.client.chat.completions.create(
                 model=self.model_name,
                 messages=[
                     {"role": "system", "content": system_prompt},
                     {"role": "user", "content": user_prompt},
                 ],
+                temperature=0.0,
+                seed=42,
             )
             .choices[0]
             .message.content
         )
 
     def get_score(self, response: str):
         """
```

### Comparing `validmind-2.0.1/validmind/tests/test_providers.py` & `validmind-2.0.7/validmind/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/unit_metrics/__init__.py` & `validmind-2.0.7/validmind/unit_metrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,12 +233,10 @@
 
     # Initialize the metric
     metric = metric_class(test_id=metric_id, inputs=TestInput(inputs), params=params)
 
     # Run the metric
     result = metric.run()
 
-    cache_key = get_metric_cache_key(metric_id, params, inputs)
-
     unit_metric_results_cache[cache_key] = result
 
     return result
```

### Comparing `validmind-2.0.1/validmind/unit_metrics/sklearn/classification/F1.py` & `validmind-2.0.7/validmind/unit_metrics/sklearn/classification/F1.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from sklearn.metrics import f1_score
 
 from validmind.vm_models import UnitMetric
 
 
 @dataclass
 class F1(UnitMetric):
+    required_inputs = ["dataset", "model"]
+
     def run(self):
         y_true = self.inputs.dataset.y
         y_pred = self.inputs.dataset.y_pred(model_id=self.inputs.model.input_id)
 
         value = f1_score(y_true, y_pred, **self.params)
 
         return self.cache_results(
```

### Comparing `validmind-2.0.1/validmind/unit_metrics/sklearn/classification/Precision.py` & `validmind-2.0.7/validmind/unit_metrics/regression/sklearn/MeanAbsoluteError.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright © 2023-2024 ValidMind Inc. All rights reserved.
 # See the LICENSE file in the root of this repository for details.
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
 from dataclasses import dataclass
 
-from sklearn.metrics import precision_score
+from sklearn.metrics import mean_absolute_error
 
 from validmind.vm_models import UnitMetric
 
 
 @dataclass
-class Precision(UnitMetric):
+class MeanAbsoluteError(UnitMetric):
+    required_inputs = ["dataset", "model"]
+
     def run(self):
         y_true = self.inputs.dataset.y
         y_pred = self.inputs.dataset.y_pred(model_id=self.inputs.model.input_id)
 
-        value = precision_score(y_true, y_pred, **self.params)
+        value = mean_absolute_error(y_true, y_pred, **self.params)
 
-        return self.cache_results(
-            metric_value=value,
-        )
+        return self.cache_results(metric_value=value)
```

### Comparing `validmind-2.0.1/validmind/unit_metrics/sklearn/classification/ROC_AUC.py` & `validmind-2.0.7/validmind/unit_metrics/sklearn/classification/Accuracy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright © 2023-2024 ValidMind Inc. All rights reserved.
 # See the LICENSE file in the root of this repository for details.
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
 from dataclasses import dataclass
 
-from sklearn.metrics import roc_auc_score
+from sklearn.metrics import accuracy_score
 
 from validmind.vm_models import UnitMetric
 
 
 @dataclass
-class ROC_AUC(UnitMetric):
+class Accuracy(UnitMetric):
+    required_inputs = ["dataset", "model"]
+
     def run(self):
         y_true = self.inputs.dataset.y
         y_pred = self.inputs.dataset.y_pred(model_id=self.inputs.model.input_id)
 
-        value = roc_auc_score(y_true, y_pred, **self.params)
+        value = accuracy_score(y_true, y_pred, **self.params)
 
         return self.cache_results(metric_value=value)
```

### Comparing `validmind-2.0.1/validmind/unit_metrics/sklearn/classification/Recall.py` & `validmind-2.0.7/validmind/unit_metrics/sklearn/classification/Recall.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from sklearn.metrics import recall_score
 
 from validmind.vm_models import UnitMetric
 
 
 @dataclass
 class Recall(UnitMetric):
+    required_inputs = ["dataset", "model"]
+
     def run(self):
         y_true = self.inputs.dataset.y
         y_pred = self.inputs.dataset.y_pred(model_id=self.inputs.model.input_id)
 
         value = recall_score(y_true, y_pred, **self.params)
 
         return self.cache_results(metric_value=value)
```

### Comparing `validmind-2.0.1/validmind/utils.py` & `validmind-2.0.7/validmind/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,16 @@
     elif isinstance(obj, float) and (math.isnan(obj) or math.isinf(obj)):
         return None
     return obj
 
 
 class NumpyEncoder(json.JSONEncoder):
     def default(self, obj):
+        if isinstance(obj, pd.Interval):
+            return f"[{obj.left}, {obj.right}]"
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, np.bool_):
@@ -249,15 +251,29 @@
     ]
     paragraphs = [
         paragraph.replace(" - ", "\n- ") for paragraph in paragraphs
     ]  # Add newline before list items
     # Join paragraphs with double newlines for markdown
     description = "\n\n".join(paragraphs)
 
-    return description
+    lines = description.split("\n")
+    in_bullet_list = False
+    for i, line in enumerate([line for line in lines]):
+        if line.strip().startswith("-") and not in_bullet_list:
+            if lines[i - 1] != "":
+                lines[i] = "\n" + line
+
+            in_bullet_list = True
+            continue
+        elif line.strip().startswith("-") and in_bullet_list:
+            continue
+        elif line.strip() == "" and in_bullet_list:
+            in_bullet_list = False
+
+    return "\n".join(lines)
 
 
 def format_number(number):
     """
     Format a number for display purposes. If the number is a float, round it
     to 4 decimal places.
     """
```

### Comparing `validmind-2.0.1/validmind/vm_models/__init__.py` & `validmind-2.0.7/validmind/vm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/dataset.py` & `validmind-2.0.7/validmind/vm_models/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 
 import numpy as np
 import pandas as pd
+import polars as pl
 
 from validmind.logging import get_logger
 from validmind.vm_models.model import VMModel
 
 logger = get_logger(__name__)
 
 
@@ -31,17 +32,224 @@
     def raw_dataset(self):
         """
         Returns the raw dataset.
         """
         pass
 
     @abstractmethod
-    def serialize(self):
+    def assign_predictions(
+        self,
+        model,
+        prediction_values: list = None,
+        prediction_column=None,
+    ):
         """
-        Serializes the dataset to a dictionary.
+        Assigns predictions to the dataset for a given model or prediction values.
+        The dataset is updated with a new column containing the predictions.
+        """
+        pass
+
+    @abstractmethod
+    def get_extra_column(self, column_name):
+        """
+        Returns the values of the specified extra column.
+
+        Args:
+            column_name (str): The name of the extra column.
+
+        Returns:
+            np.ndarray: The values of the extra column.
+        """
+        pass
+
+    @abstractmethod
+    def add_extra_column(self, column_name, column_values=None):
+        """
+        Adds an extra column to the dataset without modifying the dataset `features` and `target` columns.
+
+        Args:
+            column_name (str): The name of the extra column.
+            column_values (np.ndarray, optional): The values of the extra column.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def input_id(self) -> str:
+        """
+        Returns input id of dataset.
+
+        Returns:
+            str: input_id.
+        """
+        return self.input_id
+
+    @property
+    @abstractmethod
+    def columns(self) -> list:
+        """
+        Returns the the list of columns in the dataset.
+
+        Returns:
+            List[str]: The columns list.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def target_column(self) -> str:
+        """
+        Returns the target column name of the dataset.
+
+        Returns:
+            str: The target column name.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def feature_columns(self) -> list:
+        """
+        Returns the feature columns of the dataset. If _feature_columns is None,
+        it returns all columns except the target column.
+
+        Returns:
+            list: The list of feature column names.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def text_column(self) -> str:
+        """
+        Returns the text column of the dataset.
+
+        Returns:
+            str: The text column name.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def x(self) -> np.ndarray:
+        """
+        Returns the input features (X) of the dataset.
+
+        Returns:
+            np.ndarray: The input features.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def y(self) -> np.ndarray:
+        """
+        Returns the target variables (y) of the dataset.
+
+        Returns:
+            np.ndarray: The target variables.
+        """
+        pass
+
+    @abstractmethod
+    def y_pred(self, model_id) -> np.ndarray:
+        """
+        Returns the prediction values (y_pred) of the dataset for a given model_id.
+
+        Returns:
+            np.ndarray: The prediction values.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def df(self):
+        """
+        Returns the dataset as a pandas DataFrame.
+
+        Returns:
+            pd.DataFrame: The dataset as a DataFrame.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def copy(self):
+        """
+        Returns a copy of the raw_dataset dataframe.
+        """
+        pass
+
+    @abstractmethod
+    def x_df(self):
+        """
+        Returns the non target and prediction columns.
+
+        Returns:
+            pd.DataFrame: The non target and prediction columns .
+        """
+        pass
+
+    @abstractmethod
+    def y_df(self):
+        """
+        Returns the target columns (y) of the dataset.
+
+        Returns:
+            pd.DataFrame: The target columns.
+        """
+        pass
+
+    @abstractmethod
+    def y_pred_df(self, model_id):
+        """
+        Returns the target columns (y) of the dataset.
+
+        Returns:
+            pd.DataFrame: The target columns.
+        """
+        pass
+
+    @abstractmethod
+    def prediction_column(self, model_id) -> str:
+        """
+        Returns the prediction column name of the dataset.
+
+        Returns:
+            str: The prediction column name.
+        """
+        pass
+
+    @abstractmethod
+    def get_features_columns(self):
+        """
+        Returns the column names of the feature variables.
+
+        Returns:
+            List[str]: The column names of the feature variables.
+        """
+        pass
+
+    @abstractmethod
+    def get_numeric_features_columns(self):
+        """
+        Returns the column names of the numeric feature variables.
+
+        Returns:
+            List[str]: The column names of the numeric feature variables.
+        """
+        pass
+
+    @abstractmethod
+    def get_categorical_features_columns(self):
+        """
+        Returns the column names of the categorical feature variables.
+
+        Returns:
+            List[str]: The column names of the categorical feature variables.
         """
         pass
 
 
 @dataclass
 class NumpyDataset(VMDataset):
     """
@@ -130,25 +338,25 @@
 
         # initialize dataframe
         self._df = df
 
         # initialize target column
         self._target_column = target_column
         # initialize extra columns
-        self.__set_extra_columns(extra_columns, model)
+        self.__set_extra_columns(extra_columns)
         # initialize feature columns
         self.__set_feature_columns(feature_columns)
         # initialize text column, target class labels and options
         self._text_column = text_column
         self._target_class_labels = target_class_labels
         self.options = options
         if model:
             self.assign_predictions(model)
 
-    def __set_extra_columns(self, extra_columns, model):
+    def __set_extra_columns(self, extra_columns):
         if extra_columns is None:
             extra_columns = {
                 "prediction_columns": {},
                 "group_by_column": None,
             }
         self._extra_columns = extra_columns
 
@@ -187,22 +395,37 @@
 
         return df
 
     def __model_id_in_prediction_columns(self, model, prediction_column):
         return model.input_id in self._extra_columns.get("prediction_columns", {})
 
     def __assign_prediction_values(self, model, pred_column, prediction_values):
+        # Link the prediction column with the model
         self._extra_columns.setdefault("prediction_columns", {})[
             model.input_id
         ] = pred_column
-        self._raw_dataset = np.hstack(
-            (self._raw_dataset, np.array(prediction_values).reshape(-1, 1))
+
+        # Check if the predictions are multi-dimensional (e.g., embeddings)
+        is_multi_dimensional = (
+            isinstance(prediction_values, np.ndarray) and prediction_values.ndim > 1
         )
-        self._columns.append(pred_column)
-        self._df[pred_column] = prediction_values
+
+        if is_multi_dimensional:
+            # For multi-dimensional outputs, convert to a list of lists to store in DataFrame
+            self._df[pred_column] = list(map(list, prediction_values))
+        else:
+            # If not multi-dimensional or a standard numpy array, reshape for compatibility
+            self._raw_dataset = np.hstack(
+                (self._raw_dataset, np.array(prediction_values).reshape(-1, 1))
+            )
+            self._df[pred_column] = prediction_values
+
+        # Update the dataset columns list
+        if pred_column not in self._columns:
+            self._columns.append(pred_column)
 
     def assign_predictions(  # noqa: C901 - we need to simplify this method
         self,
         model,
         prediction_values: list = None,
         prediction_column=None,
     ):
@@ -258,14 +481,67 @@
             prediction_values = np.array(model.predict(x_only))
             self.__assign_prediction_values(model, pred_column, prediction_values)
         else:
             logger.info(
                 f"Prediction column {self._extra_columns['prediction_columns'][model.input_id]} already linked to the {model.input_id}"
             )
 
+    def get_extra_column(self, column_name):
+        """
+        Returns the values of the specified extra column.
+
+        Args:
+            column_name (str): The name of the extra column.
+
+        Returns:
+            np.ndarray: The values of the extra column.
+        """
+        if column_name not in self.extra_columns:
+            raise ValueError(f"Column {column_name} is not an extra column")
+
+        return self._df[column_name]
+
+    def add_extra_column(self, column_name, column_values=None):
+        """
+        Adds an extra column to the dataset without modifying the dataset `features` and `target` columns.
+
+        Args:
+            column_name (str): The name of the extra column.
+            column_values (np.ndarray, optional): The values of the extra column.
+        """
+        if column_name in self.extra_columns:
+            logger.info(f"Column {column_name} already registered as an extra column")
+            return
+
+        # The column name already exists in the dataset so we just assign the extra column
+        if column_name in self.columns:
+            self._extra_columns[column_name] = column_name
+            logger.info(
+                f"Column {column_name} exists in the dataset, registering as an extra column"
+            )
+            return
+
+        if column_values is None:
+            raise ValueError(
+                "Column values must be provided when the column doesn't exist in the dataset"
+            )
+
+        if len(column_values) != self.df.shape[0]:
+            raise ValueError(
+                "Length of column values doesn't match number of rows of the dataset"
+            )
+
+        self._raw_dataset = np.hstack(
+            (self._raw_dataset, np.array(column_values).reshape(-1, 1))
+        )
+        self._columns.append(column_name)
+        self._df[column_name] = column_values
+        self._extra_columns[column_name] = column_name
+        logger.info(f"Column {column_name} added as an extra column")
+
     @property
     def raw_dataset(self) -> np.ndarray:
         """
         Returns the raw dataset.
 
         Returns:
             np.ndarray: The raw dataset.
@@ -395,27 +671,50 @@
                 for name in self.columns
                 if name == self.target_column
             ],
         ]
 
     def y_pred(self, model_id) -> np.ndarray:
         """
-        Returns the prediction variable (y_pred) of the dataset.
+        Returns the prediction variables for a given model_id, accommodating
+        both scalar predictions and multi-dimensional outputs such as embeddings.
+
+        Args:
+            model_id (str): The ID of the model whose predictions are sought.
 
         Returns:
-            np.ndarray: The prediction variables.
+            np.ndarray: The prediction variables, either as a flattened array for
+            scalar predictions or as an array of arrays for multi-dimensional outputs.
         """
-        return self.raw_dataset[
-            :,
-            [
-                self.columns.index(name)
-                for name in self.columns
-                if name == self.prediction_column(model_id=model_id)
-            ],
-        ].flatten()
+        pred_column = self.prediction_column(model_id)
+
+        # First, attempt to retrieve the prediction data from the DataFrame
+        if hasattr(self, "_df") and pred_column in self._df.columns:
+            predictions = self._df[pred_column].to_numpy()
+
+            # Check if the predictions are stored as objects (e.g., lists for embeddings)
+            if self._df[pred_column].dtype == object:
+                # Attempt to convert lists to a numpy array
+                try:
+                    predictions = np.stack(predictions)
+                except ValueError as e:
+                    # Handling cases where predictions cannot be directly stacked
+                    raise ValueError(f"Error stacking prediction arrays: {e}")
+        else:
+            # Fallback to using the raw numpy dataset if DataFrame is not available or suitable
+            try:
+                predictions = self.raw_dataset[
+                    :, self.columns.index(pred_column)
+                ].flatten()
+            except IndexError as e:
+                raise ValueError(
+                    f"Prediction column '{pred_column}' not found in raw dataset: {e}"
+                )
+
+        return predictions
 
     @property
     def type(self) -> str:
         """
         Returns the type of the dataset.
 
         Returns:
@@ -604,18 +903,23 @@
         date_time_index: bool = False,
     ):
         """
         Initializes a DataFrameDataset instance.
 
         Args:
             raw_dataset (pd.DataFrame): The raw dataset as a pandas DataFrame.
+            input_id (str, optional): Identifier for the dataset. Defaults to None.
+            model (VMModel, optional): Model associated with the dataset. Defaults to None.
             target_column (str, optional): The target column of the dataset. Defaults to None.
+            extra_columns (dict, optional): Extra columns to include in the dataset. Defaults to None.
             feature_columns (list, optional): The feature columns of the dataset. Defaults to None.
-            text_column (str, optional): The text column name of the dataset for nlp tasks. Defaults to None.
-            target_class_labels (Dict, optional): The class labels for the target columns. Defaults to None.
+            text_column (str, optional): The text column name of the dataset for NLP tasks. Defaults to None.
+            target_class_labels (dict, optional): The class labels for the target columns. Defaults to None.
+            options (dict, optional): Additional options for the dataset. Defaults to None.
+            date_time_index (bool, optional): Whether to use date-time index. Defaults to False.
         """
         index = None
         if isinstance(raw_dataset.index, pd.Index):
             index = raw_dataset.index.values
 
         super().__init__(
             raw_dataset=raw_dataset.values,
@@ -627,14 +931,65 @@
             target_column=target_column,
             extra_columns=extra_columns,
             feature_columns=feature_columns,
             text_column=text_column,
             target_class_labels=target_class_labels,
             options=options,
             date_time_index=date_time_index,
+        )
+
+
+@dataclass
+class PolarsDataset(NumpyDataset):
+    """
+    VM dataset implementation for Polars DataFrame.
+    """
+
+    def __init__(
+        self,
+        raw_dataset: pl.DataFrame,
+        input_id: str = None,
+        model: VMModel = None,
+        target_column: str = None,
+        extra_columns: dict = None,
+        feature_columns: list = None,
+        text_column: str = None,
+        target_class_labels: dict = None,
+        options: dict = None,
+        date_time_index: bool = False,
+    ):
+        """
+        Initializes a PolarsDataset instance.
+
+        Args:
+            raw_dataset (pl.DataFrame): The raw dataset as a Polars DataFrame.
+            input_id (str, optional): Identifier for the dataset. Defaults to None.
+            model (VMModel, optional): Model associated with the dataset. Defaults to None.
+            target_column (str, optional): The target column of the dataset. Defaults to None.
+            extra_columns (dict, optional): Extra columns to include in the dataset. Defaults to None.
+            feature_columns (list, optional): The feature columns of the dataset. Defaults to None.
+            text_column (str, optional): The text column name of the dataset for NLP tasks. Defaults to None.
+            target_class_labels (dict, optional): The class labels for the target columns. Defaults to None.
+            options (dict, optional): Additional options for the dataset. Defaults to None.
+            date_time_index (bool, optional): Whether to use date-time index. Defaults to False.
+        """
+        super().__init__(
+            raw_dataset=raw_dataset.to_numpy(),
+            input_id=input_id,
+            model=model,
+            index_name=None,
+            index=None,
+            columns=raw_dataset.columns,
+            target_column=target_column,
+            extra_columns=extra_columns,
+            feature_columns=feature_columns,
+            text_column=text_column,
+            target_class_labels=target_class_labels,
+            options=options,
+            date_time_index=date_time_index,
         )
 
 
 @dataclass
 class TorchDataset(NumpyDataset):
     """
     VM dataset implementation for PyTorch Datasets.
```

### Comparing `validmind-2.0.1/validmind/vm_models/figure.py` & `validmind-2.0.7/validmind/vm_models/figure.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,26 @@
 import plotly.graph_objs as go
 
 from ..client_config import client_config
 from ..errors import InvalidFigureForObjectError, UnsupportedFigureError
 from ..utils import get_full_typename
 
 
+def is_matplotlib_figure(figure) -> bool:
+    return isinstance(figure, matplotlib.figure.Figure)
+
+
+def is_plotly_figure(figure) -> bool:
+    return isinstance(figure, (go.Figure, go.FigureWidget))
+
+
+def is_png_image(figure) -> bool:
+    return isinstance(figure, bytes)
+
+
 @dataclass
 class Figure:
     """
     Figure objects track the schema supported by the ValidMind API
     """
 
     key: str
@@ -48,30 +60,18 @@
             self.metadata = metadata
 
         # Wrap around with FigureWidget so that we can display interactive Plotly
         # plots in regular Jupyter notebooks. This is not supported on Google Colab.
         if (
             not client_config.running_on_colab
             and self.figure
-            and self.is_plotly_figure()
+            and is_plotly_figure(self.figure)
         ):
             self.figure = go.FigureWidget(self.figure)
 
-    def is_matplotlib_figure(self) -> bool:
-        """
-        Returns True if the figure is a matplotlib figure
-        """
-        return isinstance(self.figure, matplotlib.figure.Figure)
-
-    def is_plotly_figure(self) -> bool:
-        """
-        Returns True if the figure is a plotly figure
-        """
-        return isinstance(self.figure, (go.Figure, go.FigureWidget))
-
     def _get_for_object_type(self):
         """
         Returns the type of the object this figure is for
         """
         # Avoid circular imports
         from .test.metric import Metric
         from .test.threshold_test import ThresholdTest
@@ -87,37 +87,46 @@
 
     def to_widget(self):
         """
         Returns the ipywidget compatible representation of the figure. Ideally
         we would render images as-is, but Plotly FigureWidgets don't work well
         on Google Colab when they are combined with ipywidgets.
         """
-        if self.is_matplotlib_figure():
+        if is_matplotlib_figure(self.figure):
             tmpfile = BytesIO()
             self.figure.savefig(tmpfile, format="png")
             encoded = base64.b64encode(tmpfile.getvalue()).decode("utf-8")
             return widgets.HTML(
                 value=f"""
                 <img style="width:100%; height: auto;" src="data:image/png;base64,{encoded}"/>
                 """
             )
 
-        elif self.is_plotly_figure():
+        elif is_plotly_figure(self.figure):
             # FigureWidget can be displayed as-is but not on Google Colab. In this case
             # we just return the image representation of the figure.
             if client_config.running_on_colab:
                 png_file = self.figure.to_image(format="png")
                 encoded = base64.b64encode(png_file).decode("utf-8")
                 return widgets.HTML(
                     value=f"""
                     <img style="width:100%; height: auto;" src="data:image/png;base64,{encoded}"/>
                     """
                 )
             else:
                 return self.figure
+
+        elif is_png_image(self.figure):
+            encoded = base64.b64encode(self.figure).decode("utf-8")
+            return widgets.HTML(
+                value=f"""
+                <img style="width:100%; height: auto;" src="data:image/png;base64,{encoded}"/>
+                """
+            )
+
         else:
             raise UnsupportedFigureError(
                 f"Figure type {type(self.figure)} not supported for plotting"
             )
 
     def serialize(self):
         """
@@ -125,23 +134,46 @@
         """
         return {
             "type": self._type,
             "key": self.key,
             "metadata": json.dumps(self.metadata, allow_nan=False),
         }
 
+    def _get_b64_url(self):
+        """
+        Returns a base64 encoded URL for the figure
+        """
+        if is_matplotlib_figure(self.figure):
+            buffer = BytesIO()
+            self.figure.savefig(buffer, format="png")
+            buffer.seek(0)
+
+            b64_data = base64.b64encode(buffer.read()).decode("utf-8")
+
+            return f"data:image/png;base64,{b64_data}"
+
+        elif is_plotly_figure(self.figure):
+            bytes = self.figure.to_image(format="png")
+            b64_data = base64.b64encode(bytes).decode("utf-8")
+
+            return f"data:image/png;base64,{b64_data}"
+
+        raise UnsupportedFigureError(
+            f"Unrecognized figure type: {get_full_typename(self.figure)}"
+        )
+
     def serialize_files(self):
         """Creates a `requests`-compatible files object to be sent to the API"""
-        if self.is_matplotlib_figure():
+        if is_matplotlib_figure(self.figure):
             buffer = BytesIO()
             self.figure.savefig(buffer, bbox_inches="tight")
             buffer.seek(0)
             return {"image": (f"{self.key}.png", buffer, "image/png")}
 
-        elif self.is_plotly_figure():
+        elif is_plotly_figure(self.figure):
             # When using plotly, we need to use we will produce two files:
             # - a JSON file that will be used to display the figure in the UI
             # - a PNG file that will be used to display the figure in documents
             return {
                 "image": (
                     f"{self.key}.png",
                     self.figure.to_image(format="png"),
@@ -150,10 +182,13 @@
                 "json_image": (
                     f"{self.key}.json",
                     self.figure.to_json(),
                     "application/json",
                 ),
             }
 
+        elif is_png_image(self.figure):
+            return {"image": (f"{self.key}.png", self.figure, "image/png")}
+
         raise UnsupportedFigureError(
             f"Unrecognized figure type: {get_full_typename(self.figure)}"
         )
```

### Comparing `validmind-2.0.1/validmind/vm_models/model.py` & `validmind-2.0.7/validmind/vm_models/model.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/test/metric.py` & `validmind-2.0.7/validmind/vm_models/test/metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # See the LICENSE file in the root of this repository for details.
 # SPDX-License-Identifier: AGPL-3.0 AND ValidMind Commercial
 
 """
 Class for storing ValidMind metric objects and associated
 data for display and reporting purposes
 """
+import os
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import ClassVar, List, Optional, Union
 
 import pandas as pd
 
+from ...ai import generate_description
 from ...errors import MissingCacheResultsArgumentsError
 from ...utils import clean_docstring
 from ..figure import Figure
 from .metric_result import MetricResult
 from .result_wrapper import MetricResultWrapper
 from .test import Test
 
@@ -70,45 +72,46 @@
             TestSuiteResult: The test suite result object
         """
         if metric_value is None and figures is None:
             raise MissingCacheResultsArgumentsError(
                 "Metric must provide a metric value or figures to cache_results"
             )
 
-        # At a minimum, send the metric description
-        result_metadata = [
-            {
-                "content_id": f"metric_description:{self.test_id}",
-                "text": clean_docstring(self.description()),
-            }
-        ]
-
-        result_summary = self.summary(metric_value)
-
-        result_wrapper = MetricResultWrapper(
-            result_id=self.test_id,
-            result_metadata=result_metadata,
-            inputs=self.get_accessed_inputs(),
-            output_template=self.output_template,
-        )
-
-        # We can send an empty result to push an empty metric with a summary and plots
-        metric_result_value = metric_value if metric_value is not None else {}
-
-        result_wrapper.metric = MetricResult(
-            # key=self.key,
-            # Now using the fully qualified test ID as `key`.
-            # Ideally the backend is updated to use `test_id` instead of `key`.
+        metric = MetricResult(
             key=self.test_id,
             ref_id=self._ref_id,
-            value=metric_result_value,
+            value=metric_value if metric_value is not None else {},
             value_formatter=self.value_formatter,
-            summary=result_summary,
+            summary=self.summary(metric_value),
         )
 
-        # Allow metrics to attach figures to the test suite result
-        if figures:
-            result_wrapper.figures = figures
+        if (
+            os.environ.get("VALIDMIND_LLM_DESCRIPTIONS_ENABLED", "false").lower()
+            == "true"
+        ):
+            revision_name = "Generated by ValidMind AI"
+            description = generate_description(
+                test_name=self.test_id,
+                test_description=self.description().splitlines()[0],
+                test_results=metric.serialize()["value"],
+                test_summary=metric.serialize()["summary"],
+                figures=figures,
+            )
+        else:
+            revision_name = "Default Description"
+            description = clean_docstring(self.description())
+
+        description_metadata = {
+            "content_id": f"metric_description:{self.test_id}::{revision_name}",
+            "text": description,
+        }
 
-        self.result = result_wrapper
+        self.result = MetricResultWrapper(
+            result_id=self.test_id,
+            result_metadata=[description_metadata],
+            metric=metric,
+            figures=figures,
+            inputs=self.get_accessed_inputs(),
+            output_template=self.output_template,
+        )
 
         return self.result
```

### Comparing `validmind-2.0.1/validmind/vm_models/test/metric_result.py` & `validmind-2.0.7/validmind/vm_models/test/metric_result.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/test/result_summary.py` & `validmind-2.0.7/validmind/vm_models/test/result_summary.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/test/result_wrapper.py` & `validmind-2.0.7/validmind/vm_models/test/result_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,48 +6,58 @@
 Result Wrappers for test and metric results
 """
 import asyncio
 import json
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import Dict, List, Optional, Union
 
 import ipywidgets as widgets
 import markdown
 import pandas as pd
 from IPython.display import display
 
 from ... import api_client
+from ...ai import DescriptionFuture
 from ...utils import NumpyEncoder, run_async, test_id_to_name
 from ..figure import Figure
 from .metric_result import MetricResult
 from .output_template import OutputTemplate
 from .result_summary import ResultSummary
 from .threshold_test_result import ThresholdTestResults
 
 
-async def update_metadata(content_id: str, text: str) -> None:
+async def update_metadata(content_id: str, text: str, _json: Union[Dict, List] = None):
     """
     Update the metadata of a content item. By default we don't
     override the existing metadata, but we can override it by
     setting the VM_OVERRIDE_METADATA environment variable to True
     """
-    VM_OVERRIDE_METADATA = os.environ.get("VM_OVERRIDE_METADATA", False)
-    try:
-        existing_metadata = await api_client.get_metadata(content_id)
-    except Exception:
-        existing_metadata = None  # TODO: handle this better
-
-    if (
-        existing_metadata is None
-        or VM_OVERRIDE_METADATA == "True"
-        or VM_OVERRIDE_METADATA is True
-    ):
-        await api_client.log_metadata(content_id, text)
+    should_update = False
+
+    # check if the env variable is set to force overwriting metadata
+    if os.environ.get("VM_OVERRIDE_METADATA", "false").lower() == "true":
+        should_update = True
+
+    # if not set, check if the content_id is a composite metric def
+    if not should_update and content_id.startswith("composite_metric_def:"):
+        # we always want composite metric definitions to be updated
+        should_update = True
+
+    # if not set, lets check if the metadata already exists
+    if not should_update:
+        try:
+            await api_client.get_metadata(content_id)
+        except Exception:  # TODO: this shouldn't be a catch-all
+            # if the metadata doesn't exist, we should create (update) it
+            should_update = True
+
+    if should_update:
+        await api_client.log_metadata(content_id, text, _json)
 
 
 def plot_figures(figures: List[Figure]) -> None:
     """
     Plot figures to a ipywidgets GridBox
     """
 
@@ -89,15 +99,14 @@
 
         return self.to_widget()
 
     def _markdown_description_to_html(self, description: str):
         """
         Convert a markdown string to html
         """
-
         return markdown.markdown(description, extensions=["markdown.extensions.tables"])
 
     def _summary_tables_to_widget(self, summary: ResultSummary):
         """
         Create an ipywdiget representation of the summary tables
         """
         tables = []
@@ -151,15 +160,15 @@
     @abstractmethod
     async def log_async(self):
         """Log the result... Must be overridden by subclasses"""
         raise NotImplementedError
 
     def log(self):
         """Log the result... May be overridden by subclasses"""
-        return run_async(self.log_async)
+        run_async(self.log_async)
 
 
 @dataclass
 class FailedResultWrapper(ResultWrapper):
     """
     Result wrapper for test suites that fail to load or run properly
     """
@@ -203,23 +212,27 @@
         else:
             return f"{self.__class__.__name__}(result_id={self.result_id}, figures)"
 
     def to_widget(self):
         if self.metric and self.metric.key == "dataset_description":
             return ""
 
-        vbox_children = []
+        vbox_children = [
+            widgets.HTML(value=f"<h1>{test_id_to_name(self.result_id)}</h1>")
+        ]
 
         if self.result_metadata:
-            metric_description = self.result_metadata[0]
+            metric_description = self.result_metadata[0].get("text", "")
+            if isinstance(metric_description, DescriptionFuture):
+                metric_description = metric_description.get_description()
+                self.result_metadata[0]["text"] = metric_description
+
             vbox_children.append(
                 widgets.HTML(
-                    value=self._markdown_description_to_html(
-                        metric_description.get("text", "")
-                    )
+                    value=self._markdown_description_to_html(metric_description)
                 )
             )
 
         if self.metric:
             if self.output_template:
                 rendered_output = OutputTemplate(self.output_template).render(
                     value=self.metric.value
@@ -293,16 +306,27 @@
                     inputs=self.inputs,
                     output_template=self.output_template,
                 )
             )
         if self.figures:
             tasks.append(api_client.log_figures(self.figures))
         if hasattr(self, "result_metadata") and self.result_metadata:
+            description = self.result_metadata[0].get("text", "")
+            if isinstance(description, DescriptionFuture):
+                description = description.get_description()
+                self.result_metadata[0]["text"] = description
+
             for metadata in self.result_metadata:
-                tasks.append(update_metadata(metadata["content_id"], metadata["text"]))
+                tasks.append(
+                    update_metadata(
+                        content_id=metadata["content_id"],
+                        text=metadata.get("text", ""),
+                        _json=metadata.get("json"),
+                    )
+                )
 
         await asyncio.gather(*tasks)
 
 
 @dataclass
 class ThresholdTestResultWrapper(ResultWrapper):
     """
@@ -335,22 +359,26 @@
         description_html = []
 
         test_params = json.dumps(self.test_results.params, cls=NumpyEncoder, indent=2)
 
         test_title = test_id_to_name(self.test_results.test_name)
         description_html.append(
             f"""
-            <h2>{test_title} {"✅" if self.test_results.passed else "❌"}</h2>
+            <h1>{test_title} {"✅" if self.test_results.passed else "❌"}</h1>
             """
         )
 
         if self.result_metadata:
-            metric_description = self.result_metadata[0]
+            metric_description = self.result_metadata[0].get("text", "")
+            if isinstance(metric_description, DescriptionFuture):
+                metric_description = metric_description.get_description()
+                self.result_metadata[0]["text"] = metric_description
+
             description_html.append(
-                self._markdown_description_to_html(metric_description.get("text", ""))
+                self._markdown_description_to_html(metric_description)
             )
 
         description_html.append(
             f"""
                 <h4>Test Parameters</h4>
                 <pre>{test_params}</pre>
             """
@@ -371,11 +399,16 @@
 
     async def log_async(self):
         tasks = [api_client.log_test_result(self.test_results, self.inputs)]
 
         if self.figures:
             tasks.append(api_client.log_figures(self.figures))
         if hasattr(self, "result_metadata") and self.result_metadata:
+            description = self.result_metadata[0].get("text", "")
+            if isinstance(description, DescriptionFuture):
+                description = description.get_description()
+                self.result_metadata[0]["text"] = description
+
             for metadata in self.result_metadata:
                 tasks.append(update_metadata(metadata["content_id"], metadata["text"]))
 
         await asyncio.gather(*tasks)
```

### Comparing `validmind-2.0.1/validmind/vm_models/test/test.py` & `validmind-2.0.7/validmind/vm_models/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import ClassVar, List, TypedDict
 from uuid import uuid4
 
 from ..test_context import TestUtils
+from .result_wrapper import ResultWrapper
 
 
 class TestMetadata(TypedDict):
     """
     TestMetadata is a custom dict type that allows us to add metadata to tests
     """
 
@@ -31,15 +32,15 @@
     required_inputs: ClassVar[List[str]] = None  # should be overridden by leaf classes
     default_params: ClassVar[dict] = None  # should be overridden by leaf classes
 
     # Instance Variables
     _ref_id: str = None  # unique identifier (populated at init)
     _section_id: str = None  # which section of template this test belongs to
     test_id: str = None  # populated when loading tests from suites
-    result: object = None  # type should be overridden by parent classes
+    result: ResultWrapper = None  # type should be overridden by parent classes
 
     params: dict = None  # populated by test suite from user-passed config
 
     output_template: str = None  # optional output template
 
     def __post_init__(self):
         """
```

### Comparing `validmind-2.0.1/validmind/vm_models/test/threshold_test.py` & `validmind-2.0.7/validmind/vm_models/test/threshold_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 """
 (Threshold)Test class wrapper. Our API exposes the concept of of a
 Test (as test_results) but we'll refer to it as a ThresholdTest to
 avoid confusion with the "tests" in the general data science/modeling sense.
 """
 
+import os
 from dataclasses import dataclass
 from typing import ClassVar, List, Optional
 
+from ...ai import generate_description
 from ...utils import clean_docstring
 from ..figure import Figure
 from .result_summary import ResultSummary, ResultTable
 from .result_wrapper import ThresholdTestResultWrapper
 from .test import Test
 from .threshold_test_result import ThresholdTestResult, ThresholdTestResults
 
@@ -72,33 +74,42 @@
         Args:
             result (List[ThresholdTestResult]): The results of the threshold test
             passed (bool): Whether the threshold test passed or failed
 
         Returns:
             TestSuiteResult: The test suite result object
         """
-        # Rename to self.result
-        # At a minimum, send the test description
-        result_metadata = [
-            {
-                "content_id": f"test_description:{self.test_id}",
-                "text": clean_docstring(self.description()),
-            }
-        ]
-
         result_summary = self.summary(test_results_list, passed)
 
+        if (
+            os.environ.get("VALIDMIND_LLM_DESCRIPTIONS_ENABLED", "false").lower()
+            == "true"
+        ):
+            revision_name = "Generated by ValidMind AI"
+            description = generate_description(
+                test_name=self.test_id,
+                test_description=self.description().splitlines()[0],
+                test_results=[result.serialize() for result in test_results_list],
+                test_summary=result_summary.serialize(),
+                figures=figures,
+            )
+        else:
+            revision_name = "Default Description"
+            description = clean_docstring(self.description())
+
+        description_metadata = {
+            "content_id": f"test_description:{self.test_id}::{revision_name}",
+            "text": description,
+        }
+
         self.result = ThresholdTestResultWrapper(
             result_id=self.test_id,
-            result_metadata=result_metadata,
+            result_metadata=[description_metadata],
             inputs=self.get_accessed_inputs(),
             test_results=ThresholdTestResults(
-                # test_name=self.name,
-                # Now using the fully qualified test ID as `test_name`.
-                # Ideally the backend is updated to use `test_id` instead of `test_name`.
                 test_name=self.test_id,
                 ref_id=self._ref_id,
                 params=self.params,
                 passed=passed,
                 results=test_results_list,
                 summary=result_summary,
             ),
```

### Comparing `validmind-2.0.1/validmind/vm_models/test/threshold_test_result.py` & `validmind-2.0.7/validmind/vm_models/test/threshold_test_result.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/test/unit_metric.py` & `validmind-2.0.7/validmind/vm_models/test/unit_metric.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/test_context.py` & `validmind-2.0.7/validmind/vm_models/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,21 @@
     def get_accessed_inputs(self):
         """Return a list of inputs that were accessed for this test"""
         if isinstance(self.inputs, InputAccessTrackerProxy):
             return self.inputs.get_accessed()
 
         return []
 
+    def _get_input_dict(self):
+        """Return a dictionary of all inputs"""
+        if isinstance(self.inputs, InputAccessTrackerProxy):
+            return self.inputs._inputs.__dict__
+
+        return self.inputs.__dict__
+
     def _get_legacy_input(self, key):
         """Retrieve an input from the Test Input or, for backwards compatibility,
         the Test Context
 
         We should remove this once we all tests (including customer tests) are
         using `self.inputs.<input_name>` instead of `self.<input_name>`.
         """
```

### Comparing `validmind-2.0.1/validmind/vm_models/test_suite/runner.py` & `validmind-2.0.7/validmind/vm_models/test_suite/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         # TODO: use asyncio.gather here for better performance
         for test in tests:
             self.pbar_description.value = (
                 f"Sending result to ValidMind: {test.test_id}..."
             )
 
             try:
-                await test.log()
+                await test.log_async()
             except Exception as e:
                 self.pbar_description.value = "Failed to send result to ValidMind"
                 logger.error(f"Failed to log result: {test.result}")
 
                 raise e
 
             self.pbar.value += 1
```

### Comparing `validmind-2.0.1/validmind/vm_models/test_suite/summary.py` & `validmind-2.0.7/validmind/vm_models/test_suite/summary.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/validmind/vm_models/test_suite/test.py` & `validmind-2.0.7/validmind/vm_models/test_suite/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,13 +147,13 @@
                 result_id=self._test_instance.name,
             )
 
             return
 
         self.result = self._test_instance.result
 
-    async def log(self):
+    async def log_async(self):
         """Log the result for this test to ValidMind"""
         if not self.result:
             raise ValueError("Cannot log test result before running the test")
 
         await self.result.log_async()
```

### Comparing `validmind-2.0.1/validmind/vm_models/test_suite/test_suite.py` & `validmind-2.0.7/validmind/vm_models/test_suite/test_suite.py`

 * *Files identical despite different names*

### Comparing `validmind-2.0.1/PKG-INFO` & `validmind-2.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,67 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 2.0.1
+Version: 2.0.7
 Summary: ValidMind Developer Framework
 License: Commercial License
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: llm
 Provides-Extra: pytorch
 Provides-Extra: r-support
 Provides-Extra: transformers
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
 Requires-Dist: arch (>=5.4.0,<6.0.0)
 Requires-Dist: bert-score (>=0.3.13,<0.4.0)
 Requires-Dist: catboost (>=1.2,<2.0)
 Requires-Dist: click (>=8.0.4,<9.0.0)
-Requires-Dist: datasets (>=2.14.5,<3.0.0) ; extra == "all" or extra == "llm"
-Requires-Dist: dython (>=0.7.1,<0.8.0)
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
-Requires-Dist: ipython (==7.34.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: kaleido (>=0.2.1,<0.3.0,!=0.2.1.post1)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0)
 Requires-Dist: levenshtein (>=0.21.1,<0.22.0) ; extra == "all" or extra == "llm"
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
-Requires-Dist: matplotlib (<3.8)
+Requires-Dist: matplotlib (<3.8.3)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
+Requires-Dist: numba (<0.59.0)
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
 Requires-Dist: openai (>=1.3.7,<2.0.0) ; extra == "all" or extra == "llm"
 Requires-Dist: pandas (==1.5.3)
-Requires-Dist: pandas-profiling (>=3.6.6,<4.0.0)
-Requires-Dist: pdoc (>=13.1.1,<14.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
+Requires-Dist: polars (>=0.20.15,<0.21.0)
 Requires-Dist: pycocoevalcap (>=1.2,<2.0) ; extra == "all" or extra == "llm"
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pypmml (>=0.9.17,<0.10.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rouge (>=1.0.1,<2.0.0)
 Requires-Dist: rpy2 (>=3.5.10,<4.0.0) ; extra == "all" or extra == "r-support"
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scorecardpy (>=0.1.9.6,<0.2.0.0)
 Requires-Dist: seaborn (>=0.11.2,<0.12.0)
-Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
+Requires-Dist: selfcheckgpt (>=0.1.7,<0.2.0)
 Requires-Dist: sentry-sdk (>=1.24.0,<2.0.0)
 Requires-Dist: shap (>=0.42.0,<0.43.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch (>=1.10.0) ; extra == "all" or extra == "llm" or extra == "pytorch"
 Requires-Dist: torchmetrics (>=1.1.1,<2.0.0) ; extra == "all" or extra == "llm"
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: transformers (>=4.32.0,<5.0.0) ; extra == "all" or extra == "llm" or extra == "transformers"
-Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xgboost (>=1.5.2,<2.0.0)
+Requires-Dist: ydata-profiling (>=4.7.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # ValidMind Developer Framework
 
 ValidMind’s Python Developer Framework is a library of developer tools and methods designed to automate
 the documentation and validation of your models.
```

