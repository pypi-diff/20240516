# Comparing `tmp/hdx_python_scraper-2.3.5.tar.gz` & `tmp/hdx_python_scraper-2.3.6.tar.gz`

## Comparing `hdx_python_scraper-2.3.5.tar` & `hdx_python_scraper-2.3.6.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     5781 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.config/coveragerc
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.config/pytest.ini
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    71985 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/documentation/main.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/_version.py
--rw-r--r--   0        0        0    15431 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/base_scraper.py
--rw-r--r--   0        0        0    53550 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/__init__.py
--rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/aggregator.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/resource_downloader.py
--rwxr-xr-x   0        0        0    14635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/rowparser.py
--rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/scraper.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/timeseries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/__init__.py
--rwxr-xr-x   0        0        0     2566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/base.py
--rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/excelfile.py
--rwxr-xr-x   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/googlesheets.py
--rwxr-xr-x   0        0        0     9498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/json.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/__init__.py
--rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/fallbacks.py
--rw-r--r--   0        0        0    22975 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/reader.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/region_lookup.py
--rw-r--r--   0        0        0    11511 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/sources.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/writer.py
--rwxr-xr-x   0        0        0    64265 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/config/project_configuration.yaml
--rwxr-xr-x   0        0        0     5328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/test_output.xlsx
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/test_scraper_all.json
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/test_scraper_other.json
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/test_scraper_population.json
--rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/additional-json.json
--rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/cbpf-allocations-and-contributions.json
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/cbpf2-allocations-and-contributions.json
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/cerf-covid-19-allocations.json
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/cerf2-covid-19-allocations.json
--rw-r--r--   0        0        0  8408437 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/cerf2_global_download-full-pfmb-allocations.csv
--rw-r--r--   0        0        0  8408437 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/cerf_global_download-full-pfmb-allocations.csv
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
--rw-r--r--   0        0        0   201089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/covidtests_data-owid-covid-data.xlsx
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/education_closures_broken.xls
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/education_closures_school_closures.csv
--rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/education_enrolment_enrollment_data.xlsx
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ethiopia-drought-related-key-figures.json
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ethiopia-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0        0        0    57148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ethiopia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/fallbacks.json
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rw-r--r--   0        0        0    12412 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/global-school-closures-covid19.json
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/hno_2017_sahel_nutrition.csv
--rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/hno_2017_sahel_people_in_need.xlsx
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/idmc-internally-displaced-persons-idps.json
--rw-r--r--   0        0        0    51259 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/idps_download-displacement-data.csv
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
--rw-r--r--   0        0        0  1371019 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/idps_somalia_som_unhcr_prmn_displacement_dataset.xlsx
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ipc_somalia_som_food_insecurity_oct_dec2022_projection.csv
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/kenya-drought-related-key-figures.json
--rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/kenya-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/kenya_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/oxcgrt_oxcgrt_csv.csv
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/oxford-covid-19-government-response-tracker.json
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/population.json
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/regions_tbl_regcov_2020_ocha.xlsx
--rw-r--r--   0        0        0    78566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/sadd-countries-to-include.csv
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/sadd_covid-data-dataset-fullvars-extype-csv.csv
--rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/sahel-humanitarian-needs-overview.json
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/sahel-humanitarian-needs-overview_prefix.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-acute-food-insecurity-country-data.json
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-drought-related-key-figures.json
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-internally-displaced-persons-idps.json
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/somalia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0    14415 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/total-covid-19-tests-performed-by-country.json
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ukraine-border-crossings.json
--rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/ukraine-who-does-what-where-3w.json
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/unocha-office-locations.json
--rwxr-xr-x   0        0        0    21331 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/who_national2_who-covid-19-global-data.csv
--rwxr-xr-x   0        0        0    21331 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/who_national3_who-covid-19-global-data.csv
--rwxr-xr-x   0        0        0    21331 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/who_national_who-covid-19-global-data.csv
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/whowhatwhere_afg_3w_data.csv
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/fixtures/input/whowhatwhere_notags_3w_data.csv
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/__init__.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/affected_targeted_reached.py
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/conftest.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/education_closures.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/education_enrolment.py
--rwxr-xr-x   0        0        0     7256 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_output.py
--rwxr-xr-x   0        0        0    14556 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_readers.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_regionlookup.py
--rw-r--r--   0        0        0    12610 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_runner.py
--rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_aggregation.py
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_appenddata.py
--rw-r--r--   0        0        0    46883 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_custom.py
--rwxr-xr-x   0        0        0    25498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_global.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_multipleurls.py
--rw-r--r--   0        0        0    29325 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_national.py
--rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_resource_downloaders.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_subnational.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_timeseries.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_sources.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/test_utils.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/tests/hdx/scraper/unhcr_myanmar_idps.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/LICENSE
--rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/README.md
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/pyproject.toml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     5899 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.config/coveragerc
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.config/pytest.ini
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    71985 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/documentation/main.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/_version.py
+-rw-r--r--   0        0        0    15433 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/base_scraper.py
+-rw-r--r--   0        0        0    53550 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/__init__.py
+-rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/aggregator.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/resource_downloader.py
+-rwxr-xr-x   0        0        0    14635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/rowparser.py
+-rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/scraper.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/timeseries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/__init__.py
+-rwxr-xr-x   0        0        0     2566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/base.py
+-rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/excelfile.py
+-rwxr-xr-x   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/googlesheets.py
+-rwxr-xr-x   0        0        0     9498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/json.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/__init__.py
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/fallbacks.py
+-rw-r--r--   0        0        0    26364 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/reader.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/region_lookup.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/sources.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/writer.py
+-rwxr-xr-x   0        0        0    64265 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0     5328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/test_output.xlsx
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/test_scraper_all.json
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/test_scraper_other.json
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/test_scraper_population.json
+-rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/additional-json.json
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/cbpf-allocations-and-contributions.json
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/cbpf2-allocations-and-contributions.json
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/cerf-covid-19-allocations.json
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/cerf2-covid-19-allocations.json
+-rw-r--r--   0        0        0  8408437 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/cerf2_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0        0        0  8408437 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/cerf_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
+-rw-r--r--   0        0        0   201089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/covidtests_data-owid-covid-data.xlsx
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/education_closures_broken.xls
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/education_closures_school_closures.csv
+-rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/education_enrolment_enrollment_data.xlsx
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ethiopia-drought-related-key-figures.json
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ethiopia-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0    57148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ethiopia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/fallbacks.json
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rw-r--r--   0        0        0    12412 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/global-school-closures-covid19.json
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/hno_2017_sahel_nutrition.csv
+-rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/hno_2017_sahel_people_in_need.xlsx
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/idmc-internally-displaced-persons-idps.json
+-rw-r--r--   0        0        0    51259 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/idps_download-displacement-data.csv
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
+-rw-r--r--   0        0        0  1371019 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/idps_somalia_som_unhcr_prmn_displacement_dataset.xlsx
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ipc_somalia_som_food_insecurity_oct_dec2022_projection.csv
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/kenya-drought-related-key-figures.json
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/kenya-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/kenya_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/oxcgrt_oxcgrt_csv.csv
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/oxford-covid-19-government-response-tracker.json
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/population.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/regions_tbl_regcov_2020_ocha.xlsx
+-rw-r--r--   0        0        0    78566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/sadd-countries-to-include.csv
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/sadd_covid-data-dataset-fullvars-extype-csv.csv
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/sahel-humanitarian-needs-overview.json
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/sahel-humanitarian-needs-overview_prefix.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-acute-food-insecurity-country-data.json
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-drought-related-key-figures.json
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-internally-displaced-persons-idps.json
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/somalia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0    14415 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/total-covid-19-tests-performed-by-country.json
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ukraine-border-crossings.json
+-rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/ukraine-who-does-what-where-3w.json
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/unocha-office-locations.json
+-rwxr-xr-x   0        0        0    21331 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/who_national2_who-covid-19-global-data.csv
+-rwxr-xr-x   0        0        0    21331 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/who_national3_who-covid-19-global-data.csv
+-rwxr-xr-x   0        0        0    21331 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/who_national_who-covid-19-global-data.csv
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/whowhatwhere_afg_3w_data.csv
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/fixtures/input/whowhatwhere_notags_3w_data.csv
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/__init__.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/affected_targeted_reached.py
+-rwxr-xr-x   0        0        0     4756 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/conftest.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/education_closures.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/education_enrolment.py
+-rwxr-xr-x   0        0        0     7256 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_output.py
+-rwxr-xr-x   0        0        0    17334 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_readers.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_regionlookup.py
+-rw-r--r--   0        0        0    12610 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_runner.py
+-rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_aggregation.py
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_appenddata.py
+-rw-r--r--   0        0        0    46885 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_custom.py
+-rwxr-xr-x   0        0        0    25498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_global.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_multipleurls.py
+-rw-r--r--   0        0        0    29325 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_national.py
+-rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_resource_downloaders.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_subnational.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_timeseries.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_sources.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/test_utils.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/tests/hdx/scraper/unhcr_myanmar_idps.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/LICENSE
+-rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/README.md
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 hdx_python_scraper-2.3.6/PKG-INFO
```

### Comparing `hdx_python_scraper-2.3.5/CONTRIBUTING.md` & `hdx_python_scraper-2.3.6/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,34 @@
 
 Also be sure to install `pre-commit`, which is run every time
 you make a git commit:
 
     pre-commit install
 
 The configuration file for this project is in a
-non-start location. Thus, you will need to edit your
+non-standard location. Thus, you will need to edit your
 `.git/hooks/pre-commit` file to reflect this. Change
 the line that begins with `ARGS` to:
 
     ARGS=(hook-impl --config=.config/pre-commit-config.yaml --hook-type=pre-commit)
 
 With pre-commit, all code is formatted according to
-[black]("https://github.com/psf/black") and
 [ruff]("https://github.com/charliermarsh/ruff") guidelines.
 
 To check if your changes pass pre-commit without committing, run:
 
     pre-commit run --all-files --config=.config/pre-commit-config.yaml
 
 ## Testing
 
 To run the tests and view coverage, execute:
 
     pytest -c .config/pytest.ini --cov hdx --cov-config .config/coveragerc
 
-Follow the example set out already in ``api.rst`` as you write the documentation.
+Follow the example set out already in ``documentation/main.md`` as you write the documentation.
 
 ## Packages
 
 [pip-tools](https://github.com/jazzband/pip-tools) is used for
 package management.  If you’ve introduced a new package to the
 source code (i.e.anywhere in `src/`), please add it to the
 `project.dependencies` section of
```

### Comparing `hdx_python_scraper-2.3.5/requirements.txt` & `hdx_python_scraper-2.3.6/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,289 +1,292 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --all-extras --output-file=requirements.txt pyproject.toml
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile pyproject.toml --resolver=backtracking --all-extras -o requirements.txt
 annotated-types==0.6.0
     # via pydantic
 attrs==23.2.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
-cachetools==5.3.2
+    #   referencing
+cachetools==5.3.3
     # via google-auth
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 cfgv==3.4.0
     # via pre-commit
 chardet==5.2.0
     # via frictionless
 charset-normalizer==3.3.2
     # via requests
-ckanapi==4.7
+ckanapi==4.8
     # via hdx-python-api
 click==8.1.7
     # via typer
-colorama==0.4.6
-    # via typer
-coverage[toml]==7.4.1
-    # via
-    #   coverage
-    #   pytest-cov
-cryptography==42.0.2
+coverage==7.5.1
+    # via pytest-cov
+cryptography==42.0.7
     # via pyopenssl
 defopt==6.4.0
     # via hdx-python-api
 distlib==0.3.8
     # via virtualenv
-dnspython==2.5.0
+dnspython==2.6.1
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
-docutils==0.20.1
+docutils==0.21.2
     # via defopt
-email-validator==2.1.0.post1
+email-validator==2.1.1
     # via hdx-python-api
 et-xmlfile==1.1.0
     # via openpyxl
-filelock==3.13.1
+filelock==3.14.0
     # via virtualenv
-frictionless==5.16.1
+frictionless==5.17.0
     # via hdx-python-utilities
-google-auth==2.27.0
+google-auth==2.29.0
     # via
     #   google-auth-oauthlib
     #   gspread
 google-auth-oauthlib==1.2.0
     # via gspread
-gspread==6.0.0
+gspread==6.1.1
     # via hdx-python-scraper (pyproject.toml)
-hdx-python-api==6.2.1
+hdx-python-api==6.2.8
     # via hdx-python-scraper (pyproject.toml)
-hdx-python-country==3.6.4
+hdx-python-country==3.7.0
     # via
-    #   hdx-python-api
     #   hdx-python-scraper (pyproject.toml)
-hdx-python-utilities==3.6.4
+    #   hdx-python-api
+hdx-python-utilities==3.6.8
     # via
     #   hdx-python-api
     #   hdx-python-country
 humanize==4.9.0
     # via frictionless
-identify==2.5.33
+identify==2.5.36
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   email-validator
     #   requests
 ijson==3.2.3
     # via hdx-python-utilities
-inflect==7.0.0
+inflect==7.2.1
     # via quantulum3
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
-jinja2==3.1.3
+jinja2==3.1.4
     # via frictionless
 jsonlines==4.0.0
     # via hdx-python-utilities
 jsonpath-ng==1.6.1
     # via libhxl
-jsonschema==4.17.3
+jsonschema==4.22.0
     # via
     #   frictionless
     #   tableschema-to-template
-libhxl==5.2
+jsonschema-specifications==2023.12.1
+    # via jsonschema
+libhxl==5.2.1
     # via
     #   hdx-python-api
     #   hdx-python-country
 loguru==0.7.2
     # via hdx-python-utilities
 makefun==1.15.2
     # via hdx-python-api
 markdown-it-py==3.0.0
     # via rich
-marko==2.0.2
+marko==2.0.3
     # via frictionless
-markupsafe==2.1.4
+markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
+more-itertools==10.2.0
+    # via inflect
 ndg-httpsclient==0.5.1
     # via hdx-python-api
 nodeenv==1.8.0
     # via pre-commit
 num2words==0.5.13
     # via quantulum3
-numpy==1.26.3
+numpy==1.26.4
     # via pandas
 oauthlib==3.2.2
     # via requests-oauthlib
 openpyxl==3.1.2
     # via hdx-python-utilities
-packaging==23.2
+packaging==24.0
     # via pytest
-pandas==2.2.0
+pandas==2.2.2
     # via hdx-python-scraper (pyproject.toml)
-petl==1.7.14
+petl==1.7.15
     # via frictionless
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
 pockets==0.9.1
     # via sphinxcontrib-napoleon
-pre-commit==3.6.0
+pre-commit==3.7.1
     # via hdx-python-scraper (pyproject.toml)
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
     #   pyasn1-modules
     #   rsa
-pyasn1-modules==0.3.0
+pyasn1-modules==0.4.0
     # via google-auth
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==2.6.0
-    # via
-    #   frictionless
-    #   inflect
-pydantic-core==2.16.1
+pydantic==2.7.1
+    # via frictionless
+pydantic-core==2.18.2
     # via pydantic
-pygments==2.17.2
+pygments==2.18.0
     # via rich
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
 pyphonetics==0.5.3
     # via hdx-python-country
-pyrsistent==0.20.0
-    # via jsonschema
-pytest==8.0.0
+pytest==8.2.0
     # via
     #   hdx-python-scraper (pyproject.toml)
     #   pytest-cov
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via hdx-python-scraper (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   frictionless
     #   hdx-python-utilities
     #   libhxl
     #   pandas
 python-io-wrapper==0.3.1
     # via libhxl
-python-slugify==8.0.3
+python-slugify==8.0.4
     # via
     #   ckanapi
     #   frictionless
-pytz==2023.4
+pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
-quantulum3==0.9.0
+quantulum3==0.9.1
     # via hdx-python-api
 ratelimit==2.2.1
     # via hdx-python-utilities
-regex==2023.12.25
+referencing==0.35.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+regex==2024.5.15
     # via hdx-python-scraper (pyproject.toml)
 requests==2.31.0
     # via
     #   ckanapi
     #   frictionless
     #   hdx-python-api
     #   libhxl
     #   requests-file
     #   requests-oauthlib
 requests-file==2.0.0
     # via hdx-python-utilities
-requests-oauthlib==1.3.1
+requests-oauthlib==2.0.0
     # via google-auth-oauthlib
 rfc3986==2.0.0
     # via frictionless
-rich==13.7.0
+rich==13.7.1
     # via typer
+rpds-py==0.18.1
+    # via
+    #   jsonschema
+    #   referencing
 rsa==4.9
     # via google-auth
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
+setuptools==69.5.1
+    # via
+    #   ckanapi
+    #   nodeenv
 shellingham==1.5.4
     # via typer
 simpleeval==0.9.13
     # via frictionless
+simplejson==3.19.2
+    # via ckanapi
 six==1.16.0
     # via
     #   ckanapi
     #   isodate
     #   pockets
     #   python-dateutil
     #   sphinxcontrib-napoleon
 sphinxcontrib-napoleon==0.7
     # via defopt
-strenum==0.4.15
-    # via gspread
 stringcase==1.2.0
     # via frictionless
 structlog==24.1.0
     # via libhxl
 tableschema-to-template==0.0.13
     # via hdx-python-utilities
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
-typer[all]==0.9.0
-    # via
-    #   frictionless
-    #   typer
-typing-extensions==4.9.0
+typeguard==4.2.1
+    # via inflect
+typer==0.12.3
+    # via frictionless
+typing-extensions==4.11.0
     # via
     #   frictionless
     #   inflect
     #   pydantic
     #   pydantic-core
+    #   typeguard
     #   typer
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 unidecode==1.3.8
     # via
     #   libhxl
     #   pyphonetics
-urllib3==2.2.0
+urllib3==2.2.1
     # via
     #   libhxl
     #   requests
-validators==0.22.0
+validators==0.28.1
     # via frictionless
-virtualenv==20.25.0
+virtualenv==20.26.2
     # via pre-commit
-wheel==0.42.0
+wheel==0.43.0
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
-xlsxwriter==3.1.9
+xlsxwriter==3.2.0
     # via tableschema-to-template
 xlwt==1.3.0
     # via hdx-python-utilities
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `hdx_python_scraper-2.3.5/.config/pre-commit-config.yaml` & `hdx_python_scraper-2.3.6/.config/pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,23 @@
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude: test_scraper_.*\.json
       - id: check-ast
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.4.4
     hooks:
       # Run the linter.
       - id: ruff
         args: [--config, .config/ruff.toml, --fix]
       # Run the formatter.
       - id: ruff-format
         args: [--config, .config/ruff.toml]
-  - repo: https://github.com/jazzband/pip-tools
-    rev: 7.3.0
+  - repo: https://github.com/astral-sh/uv-pre-commit
+    rev: 0.1.44
     hooks:
+      # Run the pip compile
       - id: pip-compile
         name: pip-compile requirements.txt
         files: pyproject.toml
-        args: [pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt]
+        args: [ pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt ]
```

### Comparing `hdx_python_scraper-2.3.5/.github/workflows/publish.yaml` & `hdx_python_scraper-2.3.6/.github/workflows/publish.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     types: [published]
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install --upgrade hatch
     - name: Build with hatch
```

### Comparing `hdx_python_scraper-2.3.5/documentation/main.md` & `hdx_python_scraper-2.3.6/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/documentation/pydoc-markdown.yaml` & `hdx_python_scraper-2.3.6/documentation/pydoc-markdown.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.scraper
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Scraper
-    theme: mkdocs
+    theme: material
     repo_url: "https://github.com/OCHA-DAP/hdx-python-scraper"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-scraper
   pages:
     - title: Home
```

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/base_scraper.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/base_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,17 +137,17 @@
             return
         if self.datasetinfo.get("no_sources", False):
             return
         should_overwrite_sources = self.datasetinfo.get(
             "should_overwrite_sources"
         )
         if should_overwrite_sources is not None:
-            self.source_configuration[
-                "should_overwrite_sources"
-            ] = should_overwrite_sources
+            self.source_configuration["should_overwrite_sources"] = (
+                should_overwrite_sources
+            )
         source = self.datasetinfo["source"]
         if isinstance(source, str):
             source = {"default_source": source}
         source_url = self.datasetinfo["source_url"]
         if isinstance(source_url, str):
             source_url = {"default_url": source_url}
         Sources.standardise_datasetinfo_source_date(self.datasetinfo)
```

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/runner.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/runner.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/aggregator.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/aggregator.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/resource_downloader.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/rowparser.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/rowparser.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/scraper.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/scraper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/configurable/timeseries.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/configurable/timeseries.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/base.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/base.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/excelfile.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/excelfile.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/googlesheets.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/googlesheets.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/outputs/json.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/outputs/json.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/__init__.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/fallbacks.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/fallbacks.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/reader.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import glob
 import logging
 from datetime import datetime
 from os.path import join
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 from urllib.parse import parse_qsl
 
 import hxl
 from hxl.input import InputOptions, munge_url
 from slugify import slugify
 
 from . import get_startend_dates_from_time_period, match_template
 from .sources import Sources
+from hdx.api.configuration import Configuration
 from hdx.data.dataset import Dataset
 from hdx.data.resource import Resource
 from hdx.utilities.dateparse import parse_date
 from hdx.utilities.downloader import Download
 from hdx.utilities.retriever import Retrieve
 from hdx.utilities.saver import save_json
 from hdx.utilities.typehint import ListTuple
@@ -234,37 +236,90 @@
         return self.get_tabular_rows(
             url,
             dict_form=True,
             has_hxl=datasetinfo.get("use_hxl", False),
             **kwargs,
         )
 
-    def read_dataset(self, dataset_name: str) -> Optional[Dataset]:
+    def read_dataset(
+        self, dataset_name: str, configuration: Optional[Configuration] = None
+    ) -> Optional[Dataset]:
         """Read HDX dataset
 
         Args:
             dataset_name (str): Dataset name
+            configuration (Optional[Configuration]): HDX configuration. Defaults to global configuration.
 
         Returns:
             Optional[Dataset]: The dataset that was read or None
         """
         saved_path = join(self.saved_dir, f"{dataset_name}.json")
         if self.use_saved:
             logger.info(f"Using saved dataset {dataset_name} in {saved_path}")
             dataset = Dataset.load_from_json(saved_path)
         else:
-            dataset = Dataset.read_from_hdx(dataset_name)
+            dataset = Dataset.read_from_hdx(dataset_name, configuration)
             if self.save:
                 logger.info(f"Saving dataset {dataset_name} in {saved_path}")
                 if dataset is None:
                     save_json(None, saved_path)
                 else:
                     dataset.save_to_json(saved_path, follow_urls=True)
         return dataset
 
+    def search_datasets(
+        self,
+        filename: str,
+        query: Optional[str] = "*:*",
+        configuration: Optional[Configuration] = None,
+        page_size: int = 1000,
+        **kwargs: Any,
+    ) -> List[Dataset]:
+        """Read HDX dataset
+
+        Args:
+            filename (str): Filename for saved files. Will be prefixed by underscore and a number.
+            query (Optional[str]): Query (in Solr format). Defaults to '*:*'.
+            configuration (Optional[Configuration]): HDX configuration. Defaults to global configuration.
+            page_size (int): Size of page to return. Defaults to 1000.
+            **kwargs: See below
+            fq (string): Any filter queries to apply
+            rows (int): Number of matching rows to return. Defaults to all datasets (sys.maxsize).
+            start (int): Offset in the complete result for where the set of returned datasets should begin
+            sort (string): Sorting of results. Defaults to 'relevance asc, metadata_modified desc' if rows<=page_size or 'metadata_modified asc' if rows>page_size.
+            facet (string): Whether to enable faceted results. Default to True.
+            facet.mincount (int): Minimum counts for facet fields should be included in the results
+            facet.limit (int): Maximum number of values the facet fields return (- = unlimited). Defaults to 50.
+            facet.field (List[str]): Fields to facet upon. Default is empty.
+            use_default_schema (bool): Use default package schema instead of custom schema. Defaults to False.
+
+        Returns:
+            List[Dataset]: list of datasets resulting from query
+        """
+
+        saved_path = join(self.saved_dir, filename)
+        if self.use_saved:
+            logger.info(
+                f"Using saved datasets in {filename}_n.json in {self.saved_dir}"
+            )
+            datasets = []
+            for file_path in glob.glob(f"{saved_path}_*.json"):
+                datasets.append(Dataset.load_from_json(file_path))
+        else:
+            datasets = Dataset.search_in_hdx(
+                query, configuration, page_size, **kwargs
+            )
+            if self.save:
+                for i, dataset in enumerate(datasets):
+                    file_path = f"{saved_path}_{i}.json"
+                    name = dataset["name"]
+                    logger.info(f"Saving dataset {name} in {file_path}")
+                    dataset.save_to_json(file_path, follow_urls=True)
+        return datasets
+
     @staticmethod
     def construct_filename(name: str, format: str):
         """Construct filename from name and format. The filename of the file
         comes from the name and format.
 
         Args:
             name (str): Name for the download
@@ -434,15 +489,18 @@
         """
         name = hapi_resource_metadata["name"]
         format = hapi_resource_metadata["format"]
         url = hapi_resource_metadata["download_url"]
         return self.hxl_info_file(name, format, url, **kwargs)
 
     def read_hdx_metadata(
-        self, datasetinfo: Dict, do_resource_check: bool = True
+        self,
+        datasetinfo: Dict,
+        do_resource_check: bool = True,
+        configuration: Optional[Configuration] = None,
     ) -> Optional[Resource]:
         """Read metadata from HDX dataset and add to input dictionary. If url
         is not supplied, will look through resources for one that matches
         specified format and use its url unless do_resource_check is False.
         The dataset key of the parameter datasetinfo will usually point to a
         string (single dataset) but where sources vary across HXL tags can be
         a dictionary that maps from HXL tags to datasets with the key
@@ -450,21 +508,22 @@
         the keys hapi_dataset_metadata and hapi_resource_metadata will be
         populated with more detailed dataset and resource information required
         by HAPI.
 
         Args:
             datasetinfo (Dict): Dictionary of information about dataset
             do_resource_check (bool): Whether to check resources. Defaults to False.
+            configuration (Optional[Configuration]): HDX configuration. Defaults to global configuration.
 
         Returns:
             Optional[Resource]: The resource if a url was not given
         """
         dataset_nameinfo = datasetinfo["dataset"]
         if isinstance(dataset_nameinfo, str):
-            dataset = self.read_dataset(dataset_nameinfo)
+            dataset = self.read_dataset(dataset_nameinfo, configuration)
             resource = None
             url = datasetinfo.get("url")
             resource_name = datasetinfo.get("resource")
             # Only loop through resources if do_resource_check is True and
             # either there is no url in the datasetinfo dictionary or a
             # resource name has been specified in there
             if do_resource_check and (not url or resource_name):
@@ -487,32 +546,32 @@
                     error.append(f"in {dataset_nameinfo}!")
                     raise ValueError(" ".join(error))
                 if url:  # if there is a url in the datasetinfo dictionary,
                     resource["url"] = url  # set the resource url to it
                 else:
                     url = resource["url"]  # otherwise set the url key in
                     # datasetinfo to the resource url (by setting url here)
-                datasetinfo[
-                    "hapi_resource_metadata"
-                ] = self.get_hapi_resource_metadata(resource)
+                datasetinfo["hapi_resource_metadata"] = (
+                    self.get_hapi_resource_metadata(resource)
+                )
                 datasetinfo["url"] = url
             if "source_date" not in datasetinfo:
-                datasetinfo[
-                    "source_date"
-                ] = get_startend_dates_from_time_period(
-                    dataset, today=self.today
+                datasetinfo["source_date"] = (
+                    get_startend_dates_from_time_period(
+                        dataset, today=self.today
+                    )
                 )
             if "source" not in datasetinfo:
                 datasetinfo["source"] = dataset["dataset_source"]
             if "source_url" not in datasetinfo:
                 datasetinfo["source_url"] = dataset.get_hdx_url()
             Sources.standardise_datasetinfo_source_date(datasetinfo)
-            datasetinfo[
-                "hapi_dataset_metadata"
-            ] = self.get_hapi_dataset_metadata(dataset, datasetinfo)
+            datasetinfo["hapi_dataset_metadata"] = (
+                self.get_hapi_dataset_metadata(dataset, datasetinfo)
+            )
             return resource
 
         if "source_date" not in datasetinfo:
             source_date = {}
         else:
             source_date = None
         if "source" not in datasetinfo:
@@ -523,15 +582,15 @@
             source_url = {}
         else:
             source_url = None
         datasets = {}
         for hxltag, dataset_name in dataset_nameinfo.items():
             dataset = datasets.get(dataset_name)
             if not dataset:
-                dataset = self.read_dataset(dataset_name)
+                dataset = self.read_dataset(dataset_name, configuration)
                 datasets[dataset_name] = dataset
             if source_date is not None:
                 if hxltag == "default_dataset":
                     key = "default_date"
                 else:
                     key = hxltag
                 source_date[key] = get_startend_dates_from_time_period(
@@ -557,26 +616,30 @@
             datasetinfo["source_url"] = source_url
         Sources.standardise_datasetinfo_source_date(datasetinfo)
         return None
 
     def read_hdx(
         self,
         datasetinfo: Dict,
+        configuration: Optional[Configuration] = None,
         **kwargs: Any,
     ) -> Tuple[List[str], Iterator[Dict]]:
         """Read data and metadata from HDX dataset
 
         Args:
             datasetinfo (Dict): Dictionary of information about dataset
+            configuration (Optional[Configuration]): HDX configuration. Defaults to global configuration.
             **kwargs: Parameters to pass to download_file call
 
         Returns:
             Tuple[List[str],Iterator[Dict]]: Tuple (headers, iterator where each row is a dictionary)
         """
-        resource = self.read_hdx_metadata(datasetinfo)
+        resource = self.read_hdx_metadata(
+            datasetinfo, configuration=configuration
+        )
         filename = kwargs.get("filename")
         if filename:
             del kwargs["filename"]
             datasetinfo["filename"] = filename
         filename = datasetinfo.get("filename")
         if resource and not filename:
             filename = self.construct_filename(
@@ -589,29 +652,33 @@
                 filename = f"{file_prefix}_{filename}"
             datasetinfo["filename"] = filename
         return self.read_tabular(datasetinfo, **kwargs)
 
     def read(
         self,
         datasetinfo: Dict,
+        configuration: Optional[Configuration] = None,
         **kwargs: Any,
     ) -> Tuple[List[str], Iterator[Dict]]:
         """Read data and metadata from HDX dataset
 
         Args:
             datasetinfo (Dict): Dictionary of information about dataset
+            configuration (Optional[Configuration]): HDX configuration. Defaults to global configuration.
             **kwargs: Parameters to pass to download_file call
 
         Returns:
             Tuple[List[str],Iterator[Dict]]: Tuple (headers, iterator where each row is a dictionary)
         """
         format = datasetinfo["format"]
         if format in ["json", "csv", "xls", "xlsx"]:
             if "dataset" in datasetinfo:
-                headers, iterator = self.read_hdx(datasetinfo, **kwargs)
+                headers, iterator = self.read_hdx(
+                    datasetinfo, configuration, **kwargs
+                )
             else:
                 headers, iterator = self.read_tabular(datasetinfo, **kwargs)
         else:
             raise ValueError(
                 f"Invalid format {format} for {datasetinfo['name']}!"
             )
         return headers, iterator
```

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/region_lookup.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/region_lookup.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/sources.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,17 +278,17 @@
         Returns:
              Optional[Dict]: Source configuration dictionary
         """
         source_configuration = {}
         if no_sources:
             source_configuration["no_sources"] = True
             return source_configuration
-        source_configuration[
-            "should_overwrite_sources"
-        ] = should_overwrite_sources
+        source_configuration["should_overwrite_sources"] = (
+            should_overwrite_sources
+        )
         if suffix_attribute:
             source_configuration["suffix_attribute"] = suffix_attribute
             return source_configuration
         admin_mapping = None
         if adminlevel:
             if isinstance(adminlevel, AdminLevel):
                 admin_mapping = adminlevel.pcode_to_iso3
```

### Comparing `hdx_python_scraper-2.3.5/src/hdx/scraper/utilities/writer.py` & `hdx_python_scraper-2.3.6/src/hdx/scraper/utilities/writer.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/config/project_configuration.yaml` & `hdx_python_scraper-2.3.6/tests/config/project_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/test_output.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/test_output.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/cbpf-allocations-and-contributions.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/cbpf-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/cbpf2-allocations-and-contributions.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/cbpf2-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/cerf-covid-19-allocations.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/cerf-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/cerf2-covid-19-allocations.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/cerf2-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/cerf2_global_download-full-pfmb-allocations.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/cerf2_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/cerf_global_download-full-pfmb-allocations.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/cerf_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/covidtests_data-owid-covid-data.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/covidtests_data-owid-covid-data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/education_enrolment_enrollment_data.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/education_enrolment_enrollment_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ethiopia-drought-related-key-figures.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ethiopia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ethiopia-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ethiopia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ethiopia_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ethiopia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/fallbacks.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/fallbacks.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/global-school-closures-covid19.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/global-school-closures-covid19.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/hno_2017_sahel_nutrition.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/hno_2017_sahel_nutrition.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/hno_2017_sahel_people_in_need.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/hno_2017_sahel_people_in_need.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/idmc-internally-displaced-persons-idps.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/idmc-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/idps_download-displacement-data.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/idps_download-displacement-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/idps_somalia_som_unhcr_prmn_displacement_dataset.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/idps_somalia_som_unhcr_prmn_displacement_dataset.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ipc_somalia_som_food_insecurity_oct_dec2022_projection.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ipc_somalia_som_food_insecurity_oct_dec2022_projection.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/kenya-drought-related-key-figures.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/kenya-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/kenya-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/kenya-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/kenya_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/kenya_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/oxcgrt_oxcgrt_csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/oxcgrt_oxcgrt_csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/oxford-covid-19-government-response-tracker.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/oxford-covid-19-government-response-tracker.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/population.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/population.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx_python_scraper-2.3.6/tests/fixtures/input/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx_python_scraper-2.3.6/tests/fixtures/input/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/regions_tbl_regcov_2020_ocha.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/regions_tbl_regcov_2020_ocha.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/resource_downloader_xlsx_ukr_border_crossings_090622.xlsx` & `hdx_python_scraper-2.3.6/tests/fixtures/input/resource_downloader_xlsx_ukr_border_crossings_090622.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/sadd_covid-data-dataset-fullvars-extype-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/sadd_covid-data-dataset-fullvars-extype-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/sahel-humanitarian-needs-overview.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/sahel-humanitarian-needs-overview.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/sahel-humanitarian-needs-overview_prefix.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/sahel-humanitarian-needs-overview_prefix.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-acute-food-insecurity-country-data.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-acute-food-insecurity-country-data.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-drought-related-key-figures.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-internally-displaced-persons-idps.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/somalia-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/somalia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/somalia_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/somalia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/total-covid-19-tests-performed-by-country.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/total-covid-19-tests-performed-by-country.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ukraine-border-crossings.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ukraine-border-crossings.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/ukraine-who-does-what-where-3w.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/ukraine-who-does-what-where-3w.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/unocha-office-locations.json` & `hdx_python_scraper-2.3.6/tests/fixtures/input/unocha-office-locations.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/who_national2_who-covid-19-global-data.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/who_national2_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/who_national3_who-covid-19-global-data.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/who_national3_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/who_national_who-covid-19-global-data.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/who_national_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/fixtures/input/whowhatwhere_afg_3w_data.csv` & `hdx_python_scraper-2.3.6/tests/fixtures/input/whowhatwhere_afg_3w_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/__init__.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/affected_targeted_reached.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/affected_targeted_reached.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/conftest.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Global fixtures"""
+
 from os.path import join
 
 import pytest
 
 from . import bool_assert
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
```

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/education_closures.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/education_closures.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/education_enrolment.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/education_enrolment.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_output.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_output.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_readers.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_readers.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 clone_reader = reader.clone(downloader)
                 for property, value in vars(reader).items():
                     if property == "downloader":
                         continue
                     assert getattr(clone_reader, property) == value
 
     def test_read_dataset(self, configuration, monkeypatch):
-        def test_read_from_hdx(dataset_name):
+        def test_read_from_hdx(dataset_name, _):
             if dataset_name == "None":
                 return None
             dataset = Dataset({"name": dataset_name})
             resource = Resource(
                 {
                     "name": "test",
                     "url": "https://docs.google.com/spreadsheets/d/1NjSI2LaS3SqbgYc0HdD8oIb7lofGtiHgoKKATCpwVdY/edit#gid=1088874596",
@@ -82,14 +82,83 @@
                     dataset = reader.read_dataset(dataset_name)
                     assert dataset is None
                     dataset_name = "Test Dataset"
                     dataset = reader.read_dataset(dataset_name)
                     assert dataset["name"] == dataset_name
                     assert dataset.get_resource()["url"] == munged_url
 
+    def test_search_datasets(self, configuration, monkeypatch):
+        filename = "TestDataset"
+
+        def test_search_in_hdx(*args, **kwargs):
+            datasets = []
+            for i in range(2):
+                dataset = Dataset({"name": f"{filename}_{i}"})
+                resource = Resource(
+                    {
+                        "name": "test",
+                        "url": f"{filename}_{i}.json",
+                    }
+                )
+                resource.set_format("csv")
+                dataset.add_update_resource(resource)
+                datasets.append(dataset)
+            return datasets
+
+        with temp_dir("TestReader") as temp_folder:
+            with Download(user_agent="test") as downloader:
+                with Read(
+                    downloader,
+                    temp_folder,
+                    temp_folder,
+                    temp_folder,
+                    save=True,
+                    use_saved=False,
+                    prefix="test",
+                    today=parse_date("2021-02-01"),
+                ) as reader:
+                    monkeypatch.setattr(
+                        Dataset, "search_in_hdx", test_search_in_hdx
+                    )
+                    datasets = reader.search_datasets(filename)
+                    assert len(datasets) == 2
+                    dataset = datasets[0]
+                    assert dataset["name"] == f"{filename}_0"
+                    assert (
+                        dataset.get_resource()["url"] == f"{filename}_0.json"
+                    )
+                    dataset = datasets[1]
+                    assert dataset["name"] == f"{filename}_1"
+                    assert (
+                        dataset.get_resource()["url"] == f"{filename}_1.json"
+                    )
+                    monkeypatch.delattr(Dataset, "search_in_hdx")
+                with Read(
+                    downloader,
+                    temp_folder,
+                    temp_folder,
+                    temp_folder,
+                    save=False,
+                    use_saved=True,
+                    prefix="test",
+                    today=parse_date("2021-02-01"),
+                ) as reader:
+                    datasets = reader.search_datasets(filename)
+                    assert len(datasets) == 2
+                    dataset = datasets[0]
+                    assert dataset["name"] == f"{filename}_0"
+                    assert (
+                        dataset.get_resource()["url"] == f"{filename}_0.json"
+                    )
+                    dataset = datasets[1]
+                    assert dataset["name"] == f"{filename}_1"
+                    assert (
+                        dataset.get_resource()["url"] == f"{filename}_1.json"
+                    )
+
     def test_read_hxl_resource(self, input_folder):
         with temp_dir("TestReader") as temp_folder:
             with Download(user_agent="test") as downloader:
                 with Read(
                     downloader,
                     temp_folder,
                     input_folder,
```

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_regionlookup.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_regionlookup.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_runner.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_runner.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_aggregation.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_aggregation.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_appenddata.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_appenddata.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_custom.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,17 +316,17 @@
         )
         # give it a unique name
         education_closures2.name = f"{education_closures2.name}2"
         runner.add_custom(education_closures2)
         runner.run_one(education_closures2.name)
         # give it a unique result
         del education_closures2.values["national"][0]["AFG"]
-        education_closures2.values["national"][0][
-            "SDN"
-        ] = "Closed due to COVID-19"
+        education_closures2.values["national"][0]["SDN"] = (
+            "Closed due to COVID-19"
+        )
         hapi_results = runner.get_hapi_results()
         hapi_values["results"]["national"]["values"] = [
             {"AFG": "Closed due to COVID-19", "SDN": "Closed due to COVID-19"},
             {"AFG": 38041754},
         ]
         assert next(iter(hapi_results.values())) == hapi_values
```

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_global.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_global.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_multipleurls.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_multipleurls.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_national.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_national.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_regionaltoplevel.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_regionaltoplevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_resource_downloaders.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_resource_downloaders.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_subnational.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_subnational.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_scrapers_timeseries.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_scrapers_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/test_sources.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/test_sources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/tests/hdx/scraper/unhcr_myanmar_idps.py` & `hdx_python_scraper-2.3.6/tests/hdx/scraper/unhcr_myanmar_idps.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/.gitignore` & `hdx_python_scraper-2.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/LICENSE` & `hdx_python_scraper-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/README.md` & `hdx_python_scraper-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/pyproject.toml` & `hdx_python_scraper-2.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.3.5/PKG-INFO` & `hdx_python_scraper-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hdx-python-scraper
-Version: 2.3.5
+Version: 2.3.6
 Summary: HDX Python scraper utilities to assemble data from multiple sources
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-scraper
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,data assembly,data transformation,scrapers,tabular data
 Classifier: Development Status :: 5 - Production/Stable
```

