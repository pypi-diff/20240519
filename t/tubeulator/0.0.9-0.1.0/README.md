# Comparing `tmp/tubeulator-0.0.9.tar.gz` & `tmp/tubeulator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubeulator-0.0.9.tar", last modified: Sun Apr 28 17:47:13 2024, max compression
+gzip compressed data, was "tubeulator-0.1.0.tar", last modified: Sun May 19 21:44:22 2024, max compression
```

## Comparing `tubeulator-0.0.9.tar` & `tubeulator-0.1.0.tar`

### file list

```diff
@@ -1,898 +1,898 @@
--rw-r--r--   0        0        0     1069 2024-04-28 17:46:43.759245 tubeulator-0.0.9/LICENSE.txt
--rw-r--r--   0        0        0    12107 2024-04-28 17:46:43.759245 tubeulator-0.0.9/README.md
--rw-r--r--   0        0        0     1885 2024-04-28 17:47:13.986722 tubeulator-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      625 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/__init__.py
--rw-r--r--   0        0        0      169 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/__init__.py
--rw-r--r--   0        0        0       76 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/__init__.py
--rw-r--r--   0        0        0      541 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/names.py
--rw-r--r--   0        0        0     1225 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/__init__.py
--rw-r--r--   0        0        0      189 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/accident.py
--rw-r--r--   0        0        0      138 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/air.py
--rw-r--r--   0        0        0      877 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/bike.py
--rw-r--r--   0        0        0      357 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/crowding.py
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/disruption_lifts.py
--rw-r--r--   0        0        0      395 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/journey.py
--rw-r--r--   0        0        0     3015 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/line.py
--rw-r--r--   0        0        0      313 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/mode.py
--rw-r--r--   0        0        0      588 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/occupancy.py
--rw-r--r--   0        0        0     1331 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/place.py
--rw-r--r--   0        0        0      987 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/road.py
--rw-r--r--   0        0        0      674 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/search.py
--rw-r--r--   0        0        0     2941 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/stop.py
--rw-r--r--   0        0        0      415 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/types.py
--rw-r--r--   0        0        0      390 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/vehicle.py
--rw-r--r--   0        0        0      784 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/interface.py
--rw-r--r--   0        0        0    18440 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/api/request.py
--rw-r--r--   0        0        0     1920 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/cli.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/__init__.py
--rw-r--r--   0        0        0      120 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/gen/__init__.py
--rw-r--r--   0        0        0    13792 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/gen/dto.py
--rw-r--r--   0        0        0     2880 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/gen/emit.py
--rw-r--r--   0        0        0      566 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/gen/helpers.py
--rw-r--r--   0        0        0      735 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/gen/jsonschema.py
--rw-r--r--   0        0        0     2204 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/gen/resolution.py
--rw-r--r--   0        0        0      538 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/load_test.py
--rw-r--r--   0        0        0      658 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/codegen/populate.py
--rw-r--r--   0        0        0    10306 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json
--rw-r--r--   0        0        0      812 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json
--rw-r--r--   0        0        0      683 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/all.json
--rw-r--r--   0        0        0      344 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/casualty.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
--rw-r--r--   0        0        0      135 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/vehicle.json
--rw-r--r--   0        0        0     2473 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AirQuality/AirQuality.json
--rw-r--r--   0        0        0       67 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AirQuality/schemas/all.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/AirQuality/schemas/object.json
--rw-r--r--   0        0        0    12586 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/BikePoint.json
--rw-r--r--   0        0        0      359 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/additionalproperties.json
--rw-r--r--   0        0        0      788 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/all.json
--rw-r--r--   0        0        0     1491 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/place.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-1.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-2.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-3.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-4.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-5.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-6.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-7.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray.json
--rw-r--r--   0        0        0     3569 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json
--rw-r--r--   0        0        0      132 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/all.json
--rw-r--r--   0        0        0      120 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      828 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json
--rw-r--r--   0        0        0    64106 2024-04-28 17:46:43.763245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/Journey.json
--rw-r--r--   0        0        0     1988 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/all.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textxmlresponse.json
--rw-r--r--   0        0        0      873 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json
--rw-r--r--   0        0        0      620 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json
--rw-r--r--   0        0        0      350 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-12.json
--rw-r--r--   0        0        0      424 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-13.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-14.json
--rw-r--r--   0        0        0      243 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-15.json
--rw-r--r--   0        0        0      359 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-16.json
--rw-r--r--   0        0        0     1418 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json
--rw-r--r--   0        0        0     2645 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json
--rw-r--r--   0        0        0      218 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-19.json
--rw-r--r--   0        0        0      180 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-2.json
--rw-r--r--   0        0        0     1362 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json
--rw-r--r--   0        0        0     1892 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json
--rw-r--r--   0        0        0      355 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-22.json
--rw-r--r--   0        0        0     1294 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json
--rw-r--r--   0        0        0      464 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-24.json
--rw-r--r--   0        0        0      194 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-25.json
--rw-r--r--   0        0        0      711 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json
--rw-r--r--   0        0        0      179 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-27.json
--rw-r--r--   0        0        0      368 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-28.json
--rw-r--r--   0        0        0      561 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json
--rw-r--r--   0        0        0     1324 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json
--rw-r--r--   0        0        0      550 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json
--rw-r--r--   0        0        0      714 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json
--rw-r--r--   0        0        0     1335 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json
--rw-r--r--   0        0        0      178 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-33.json
--rw-r--r--   0        0        0      858 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json
--rw-r--r--   0        0        0      552 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json
--rw-r--r--   0        0        0      268 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-36.json
--rw-r--r--   0        0        0      297 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-37.json
--rw-r--r--   0        0        0      345 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-38.json
--rw-r--r--   0        0        0      263 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-39.json
--rw-r--r--   0        0        0      285 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-4.json
--rw-r--r--   0        0        0      743 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json
--rw-r--r--   0        0        0      302 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-5.json
--rw-r--r--   0        0        0      453 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-6.json
--rw-r--r--   0        0        0      378 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-7.json
--rw-r--r--   0        0        0     1062 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json
--rw-r--r--   0        0        0      511 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-9.json
--rw-r--r--   0        0        0      304 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl.json
--rw-r--r--   0        0        0   232588 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/Line.json
--rw-r--r--   0        0        0     7137 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/all.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metamodesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metamodesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.767245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textxmlresponse.json
--rw-r--r--   0        0        0     1417 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-10.json
--rw-r--r--   0        0        0     2641 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-11.json
--rw-r--r--   0        0        0      218 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-12.json
--rw-r--r--   0        0        0     1362 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-13.json
--rw-r--r--   0        0        0     1892 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-14.json
--rw-r--r--   0        0        0      550 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-15.json
--rw-r--r--   0        0        0      714 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-16.json
--rw-r--r--   0        0        0     1335 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-17.json
--rw-r--r--   0        0        0      178 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-18.json
--rw-r--r--   0        0        0      858 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-19.json
--rw-r--r--   0        0        0      269 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-2.json
--rw-r--r--   0        0        0     1221 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-20.json
--rw-r--r--   0        0        0     1232 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-21.json
--rw-r--r--   0        0        0      285 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-22.json
--rw-r--r--   0        0        0      762 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-23.json
--rw-r--r--   0        0        0      477 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-24.json
--rw-r--r--   0        0        0      159 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-25.json
--rw-r--r--   0        0        0      829 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-26.json
--rw-r--r--   0        0        0      244 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-27.json
--rw-r--r--   0        0        0      216 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-28.json
--rw-r--r--   0        0        0      237 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-29.json
--rw-r--r--   0        0        0      378 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-3.json
--rw-r--r--   0        0        0      257 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-30.json
--rw-r--r--   0        0        0      181 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-31.json
--rw-r--r--   0        0        0      254 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-32.json
--rw-r--r--   0        0        0      408 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-33.json
--rw-r--r--   0        0        0      458 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-34.json
--rw-r--r--   0        0        0      306 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-35.json
--rw-r--r--   0        0        0      247 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-36.json
--rw-r--r--   0        0        0      185 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-37.json
--rw-r--r--   0        0        0      207 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-38.json
--rw-r--r--   0        0        0      654 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-39.json
--rw-r--r--   0        0        0     1062 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-4.json
--rw-r--r--   0        0        0      529 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-40.json
--rw-r--r--   0        0        0     2708 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-41.json
--rw-r--r--   0        0        0      511 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-5.json
--rw-r--r--   0        0        0      873 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-6.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-7.json
--rw-r--r--   0        0        0      243 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-8.json
--rw-r--r--   0        0        0      359 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-9.json
--rw-r--r--   0        0        0      304 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl.json
--rw-r--r--   0        0        0    19274 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/Mode.json
--rw-r--r--   0        0        0      186 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/activeservicetype.json
--rw-r--r--   0        0        0      939 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/all.json
--rw-r--r--   0        0        0     2748 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/prediction.json
--rw-r--r--   0        0        0      529 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-4.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-5.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-6.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-7.json
--rw-r--r--   0        0        0    42059 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/Place.json
--rw-r--r--   0        0        0     2157 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/all.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse-1.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/id-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/id-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/id-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/id-get200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/searchget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/searchget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/searchget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/searchget200textxmlresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/system.json
--rw-r--r--   0        0        0     2640 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-10.json
--rw-r--r--   0        0        0      359 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-2.json
--rw-r--r--   0        0        0     1416 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-3.json
--rw-r--r--   0        0        0      378 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-4.json
--rw-r--r--   0        0        0     1062 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-5.json
--rw-r--r--   0        0        0      511 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-6.json
--rw-r--r--   0        0        0      873 2024-04-28 17:46:43.771245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-7.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-8.json
--rw-r--r--   0        0        0      243 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-9.json
--rw-r--r--   0        0        0      242 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/type-types-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/type-types-get200textxmlresponse.json
--rw-r--r--   0        0        0      822 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/README.md
--rw-r--r--   0        0        0   112822 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/Road.json
--rw-r--r--   0        0        0     2250 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/all.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/get200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/get200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationgeo-jsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textxmlresponse.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/system-2.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/system-3.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/system.json
--rw-r--r--   0        0        0      813 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-2.json
--rw-r--r--   0        0        0     1501 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-3.json
--rw-r--r--   0        0        0     1358 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-4.json
--rw-r--r--   0        0        0      579 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-5.json
--rw-r--r--   0        0        0      519 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-6.json
--rw-r--r--   0        0        0      245 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-7.json
--rw-r--r--   0        0        0     5927 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-8.json
--rw-r--r--   0        0        0      269 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-9.json
--rw-r--r--   0        0        0     1958 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl.json
--rw-r--r--   0        0        0    20177 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/Search.json
--rw-r--r--   0        0        0      985 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/all.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasortsget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/metasortsget200textxmlresponse.json
--rw-r--r--   0        0        0      642 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/tfl-2.json
--rw-r--r--   0        0        0      358 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/tfl.json
--rw-r--r--   0        0        0   137945 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/StopPoint.json
--rw-r--r--   0        0        0     6467 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/all.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textxmlresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationjsonresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationxmlresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textjsonresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.775245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      109 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textxmlresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/system.json
--rw-r--r--   0        0        0     1417 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json
--rw-r--r--   0        0        0     2641 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json
--rw-r--r--   0        0        0      178 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-12.json
--rw-r--r--   0        0        0      209 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-13.json
--rw-r--r--   0        0        0      258 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-14.json
--rw-r--r--   0        0        0      529 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json
--rw-r--r--   0        0        0     2708 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json
--rw-r--r--   0        0        0     1869 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json
--rw-r--r--   0        0        0      755 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json
--rw-r--r--   0        0        0      646 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json
--rw-r--r--   0        0        0      304 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-2.json
--rw-r--r--   0        0        0      967 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json
--rw-r--r--   0        0        0      358 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-21.json
--rw-r--r--   0        0        0      645 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json
--rw-r--r--   0        0        0      378 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-3.json
--rw-r--r--   0        0        0     1062 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json
--rw-r--r--   0        0        0      511 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-5.json
--rw-r--r--   0        0        0      873 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-7.json
--rw-r--r--   0        0        0      243 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-8.json
--rw-r--r--   0        0        0      359 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-9.json
--rw-r--r--   0        0        0      242 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textjsonresponse.json
--rw-r--r--   0        0        0      112 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textxmlresponse.json
--rw-r--r--   0        0        0    15378 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/Vehicle.json
--rw-r--r--   0        0        0      425 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/all.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textxmlresponse.json
--rw-r--r--   0        0        0     2705 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json
--rw-r--r--   0        0        0      495 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/tfl-3.json
--rw-r--r--   0        0        0      529 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json
--rw-r--r--   0        0        0     3579 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/crowding/crowding.json
--rw-r--r--   0        0        0     5361 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/error_inventory.md
--rw-r--r--   0        0        0    11496 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/namespace.json
--rw-r--r--   0        0        0     7685 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/naming.md
--rw-r--r--   0        0        0    24650 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/occupancy.json
--rw-r--r--   0        0        0     1365 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/all.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.779245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationxmlresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textjsonresponse.json
--rw-r--r--   0        0        0      111 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textxmlresponse.json
--rw-r--r--   0        0        0      330 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/tfl-2.json
--rw-r--r--   0        0        0      360 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/tfl-3.json
--rw-r--r--   0        0        0      697 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json
--rw-r--r--   0        0        0      356 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/tfl.json
--rw-r--r--   0        0        0     1503 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi/stationdata/stationdata.json
--rw-r--r--   0        0        0   676093 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json
--rw-r--r--   0        0        0      812 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json
--rw-r--r--   0        0        0      283 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentstatsorderedsummary.json
--rw-r--r--   0        0        0      186 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/activeservicetype.json
--rw-r--r--   0        0        0      359 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/additionalproperties.json
--rw-r--r--   0        0        0    29934 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json
--rw-r--r--   0        0        0      361 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/apiversioninfo.json
--rw-r--r--   0        0        0     1909 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json
--rw-r--r--   0        0        0      356 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bay.json
--rw-r--r--   0        0        0      697 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json
--rw-r--r--   0        0        0      360 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/carparkoccupancy.json
--rw-r--r--   0        0        0      344 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/casualty.json
--rw-r--r--   0        0        0      360 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/chargeconnectoroccupancy.json
--rw-r--r--   0        0        0      531 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json
--rw-r--r--   0        0        0      586 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json
--rw-r--r--   0        0        0     1378 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json
--rw-r--r--   0        0        0      245 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterange.json
--rw-r--r--   0        0        0      245 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterangenullable.json
--rw-r--r--   0        0        0      184 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeography.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeographywellknownvalue.json
--rw-r--r--   0        0        0      262 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguation.json
--rw-r--r--   0        0        0      185 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguationoption.json
--rw-r--r--   0        0        0      646 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json
--rw-r--r--   0        0        0     1961 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json
--rw-r--r--   0        0        0      757 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json
--rw-r--r--   0        0        0      860 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json
--rw-r--r--   0        0        0      179 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farecaveat.json
--rw-r--r--   0        0        0     1483 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json
--rw-r--r--   0        0        0      254 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresmode.json
--rw-r--r--   0        0        0      443 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresperiod.json
--rw-r--r--   0        0        0      571 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json
--rw-r--r--   0        0        0      364 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farestation.json
--rw-r--r--   0        0        0      247 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretap.json
--rw-r--r--   0        0        0      464 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretapdetails.json
--rw-r--r--   0        0        0      695 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json
--rw-r--r--   0        0        0      271 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geopoint.json
--rw-r--r--   0        0        0      877 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json
--rw-r--r--   0        0        0      325 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instruction.json
--rw-r--r--   0        0        0     1362 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json
--rw-r--r--   0        0        0      216 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/interval.json
--rw-r--r--   0        0        0     1002 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json
--rw-r--r--   0        0        0      653 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json
--rw-r--r--   0        0        0      460 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyfare.json
--rw-r--r--   0        0        0      552 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json
--rw-r--r--   0        0        0      263 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyvector.json
--rw-r--r--   0        0        0      620 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json
--rw-r--r--   0        0        0      257 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/knownjourney.json
--rw-r--r--   0        0        0     1649 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json
--rw-r--r--   0        0        0     1038 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json
--rw-r--r--   0        0        0      307 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linegroup.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textxmlresponse.json
--rw-r--r--   0        0        0      243 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemodegroup.json
--rw-r--r--   0        0        0      477 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineroutesection.json
--rw-r--r--   0        0        0      305 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetype.json
--rw-r--r--   0        0        0      178 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetypeinfo.json
--rw-r--r--   0        0        0      252 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linespecificservicetype.json
--rw-r--r--   0        0        0      786 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json
--rw-r--r--   0        0        0     1335 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json
--rw-r--r--   0        0        0      159 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroutesections.json
--rw-r--r--   0        0        0     1256 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json
--rw-r--r--   0        0        0      357 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/message.json
--rw-r--r--   0        0        0      304 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/mode.json
--rw-r--r--   0        0        0      361 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/networkstatus.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/object.json
--rw-r--r--   0        0        0      302 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/obstacle.json
--rw-r--r--   0        0        0      285 2024-04-28 17:46:43.783245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/orderedroute.json
--rw-r--r--   0        0        0      378 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengerflow.json
--rw-r--r--   0        0        0      315 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengertype.json
--rw-r--r--   0        0        0      419 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/path.json
--rw-r--r--   0        0        0      180 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/pathattribute.json
--rw-r--r--   0        0        0      542 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json
--rw-r--r--   0        0        0     1491 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json
--rw-r--r--   0        0        0      242 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placecategory.json
--rw-r--r--   0        0        0      513 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json
--rw-r--r--   0        0        0      262 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placepolygon.json
--rw-r--r--   0        0        0      355 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/plannedwork.json
--rw-r--r--   0        0        0      453 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/point.json
--rw-r--r--   0        0        0      403 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/postcodeinput.json
--rw-r--r--   0        0        0     2748 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json
--rw-r--r--   0        0        0      529 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json
--rw-r--r--   0        0        0     1340 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json
--rw-r--r--   0        0        0      245 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendationresponse.json
--rw-r--r--   0        0        0      233 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/redirect.json
--rw-r--r--   0        0        0     1958 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json
--rw-r--r--   0        0        0     6179 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json
--rw-r--r--   0        0        0      542 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json
--rw-r--r--   0        0        0      602 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json
--rw-r--r--   0        0        0      245 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionschedule.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0     1358 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json
--rw-r--r--   0        0        0      458 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routeoption.json
--rw-r--r--   0        0        0      948 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json
--rw-r--r--   0        0        0      284 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchresponse.json
--rw-r--r--   0        0        0     1417 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json
--rw-r--r--   0        0        0      251 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesectionnaptanentrysequence.json
--rw-r--r--   0        0        0      874 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json
--rw-r--r--   0        0        0      596 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json
--rw-r--r--   0        0        0      399 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchcriteria.json
--rw-r--r--   0        0        0      358 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmatch.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textxmlresponse.json
--rw-r--r--   0        0        0      680 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json
--rw-r--r--   0        0        0      254 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/servicefrequency.json
--rw-r--r--   0        0        0      269 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stationinterval.json
--rw-r--r--   0        0        0      269 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/statusseverity.json
--rw-r--r--   0        0        0     2822 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json
--rw-r--r--   0        0        0      242 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointcategory.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationjsonresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationxmlresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textjsonresponse.json
--rw-r--r--   0        0        0       69 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationxmlresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textjsonresponse.json
--rw-r--r--   0        0        0      107 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textxmlresponse.json
--rw-r--r--   0        0        0      755 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json
--rw-r--r--   0        0        0     1267 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json
--rw-r--r--   0        0        0     1000 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json
--rw-r--r--   0        0        0     1539 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json
--rw-r--r--   0        0        0      813 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
--rw-r--r--   0        0        0      164 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-1.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-2.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-3.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray.json
--rw-r--r--   0        0        0      154 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-1.json
--rw-r--r--   0        0        0      154 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-2.json
--rw-r--r--   0        0        0      154 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-3.json
--rw-r--r--   0        0        0      154 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-1.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-2.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-3.json
--rw-r--r--   0        0        0      152 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-1.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-2.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-3.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-4.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-5.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-6.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-7.json
--rw-r--r--   0        0        0      160 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-1.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-2.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-3.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-4.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-5.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-6.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-7.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-1.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-2.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-3.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-4.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-5.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-6.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-7.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-1.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-10.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-11.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-12.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-13.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-14.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-15.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.787245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-16.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-17.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-18.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-19.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-2.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-20.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-21.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-22.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-23.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-24.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-25.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-26.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-27.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-28.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-29.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-3.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-30.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-31.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-32.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-33.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-34.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-35.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-4.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-5.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-6.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-7.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-8.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-9.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray.json
--rw-r--r--   0        0        0      151 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-1.json
--rw-r--r--   0        0        0      151 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-2.json
--rw-r--r--   0        0        0      151 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-3.json
--rw-r--r--   0        0        0      151 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-1.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-10.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-11.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-2.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-3.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-4.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-5.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-6.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-7.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-8.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-9.json
--rw-r--r--   0        0        0      140 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-1.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-10.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-11.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-12.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-13.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-14.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-15.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-16.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-17.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-18.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-19.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-2.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-20.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-21.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-22.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-23.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-24.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-25.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-26.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-27.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-28.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-29.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-3.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-30.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-31.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-4.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-5.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-6.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-7.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-8.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-9.json
--rw-r--r--   0        0        0      141 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-1.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-2.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-3.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-4.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-5.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-6.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-7.json
--rw-r--r--   0        0        0      149 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-1.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-10.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-11.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-12.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-13.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-14.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-15.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-2.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-3.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-4.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-5.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-6.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-7.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-8.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-9.json
--rw-r--r--   0        0        0      146 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-1.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-10.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-11.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-2.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-3.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-4.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-5.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-6.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-7.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-8.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-9.json
--rw-r--r--   0        0        0      148 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-1.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-2.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-3.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-4.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-1.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-2.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-3.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-4.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-5.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-6.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.791245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-7.json
--rw-r--r--   0        0        0      150 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-1.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-10.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-11.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-12.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-13.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-14.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-15.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-16.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-17.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-18.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-19.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-2.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-20.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-21.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-22.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-23.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-24.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-25.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-26.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-27.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-3.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-4.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-5.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-6.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-7.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-8.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-9.json
--rw-r--r--   0        0        0      145 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-1.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-2.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-3.json
--rw-r--r--   0        0        0      153 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray.json
--rw-r--r--   0        0        0      157 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-1.json
--rw-r--r--   0        0        0      157 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-2.json
--rw-r--r--   0        0        0      157 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-3.json
--rw-r--r--   0        0        0      157 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray.json
--rw-r--r--   0        0        0      685 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json
--rw-r--r--   0        0        0      186 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettime.json
--rw-r--r--   0        0        0      186 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettype.json
--rw-r--r--   0        0        0      268 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustment.json
--rw-r--r--   0        0        0      509 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustments.json
--rw-r--r--   0        0        0      285 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetable.json
--rw-r--r--   0        0        0      806 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json
--rw-r--r--   0        0        0      377 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableroute.json
--rw-r--r--   0        0        0     1062 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json
--rw-r--r--   0        0        0      181 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/twentyfourhourclocktime.json
--rw-r--r--   0        0        0      550 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json
--rw-r--r--   0        0        0      135 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehicle.json
--rw-r--r--   0        0        0      495 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehiclematch.json
--rw-r--r--   0        0        0      126 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/FeedInfo.csv
--rw-r--r--   0        0        0    54508 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Lifts.csv
--rw-r--r--   0        0        0      347 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/ModesAndLines.csv
--rw-r--r--   0        0        0   168607 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/PlatformServices.csv
--rw-r--r--   0        0        0   145838 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Platforms.csv
--rw-r--r--   0        0        0    20909 2024-04-28 17:46:43.795245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/RampRoutes.csv
--rw-r--r--   0        0        0   389058 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv
--rw-r--r--   0        0        0   273465 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/StationPoints.csv
--rw-r--r--   0        0        0    37832 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Stations.csv
--rw-r--r--   0        0        0     8344 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv
--rw-r--r--   0        0        0    28533 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Toilets.csv
--rw-r--r--   0        0        0      119 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/gtfs/feed_info.txt
--rw-r--r--   0        0        0      135 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/gtfs/levels.txt
--rw-r--r--   0        0        0   548638 2024-04-28 17:46:43.799245 tubeulator-0.0.9/src/tubeulator/data/stationdata/gtfs/pathways.txt
--rw-r--r--   0        0        0   430539 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/data/stationdata/gtfs/stops.txt
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/db/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/db/mongod.py
--rw-r--r--   0        0        0     1332 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/db/store_creds.py
--rw-r--r--   0        0        0      722 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/exc.py
--rw-r--r--   0        0        0     2937 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/AccidentStats.py
--rw-r--r--   0        0        0      699 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/AirQuality.py
--rw-r--r--   0        0        0     2217 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/BikePoint.py
--rw-r--r--   0        0        0     1469 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/DisruptionsLiftsv2.py
--rw-r--r--   0        0        0    25751 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Journey.py
--rw-r--r--   0        0        0    36477 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Line.py
--rw-r--r--   0        0        0     3711 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Mode.py
--rw-r--r--   0        0        0    10641 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Place.py
--rw-r--r--   0        0        0    11678 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Road.py
--rw-r--r--   0        0        0     2960 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Search.py
--rw-r--r--   0        0        0    16550 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/StopPoint.py
--rw-r--r--   0        0        0     3067 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/Vehicle.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/crowding.py
--rw-r--r--   0        0        0     2803 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/occupancy.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/generated/stationdata.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/__init__.py
--rw-r--r--   0        0        0     1116 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/_types.py
--rw-r--r--   0        0        0     3063 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/dataclass_generator.py
--rw-r--r--   0        0        0     1643 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/fetch.py
--rw-r--r--   0        0        0     2028 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/reference.py
--rw-r--r--   0        0        0     1971 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/scan.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/schema/__init__.py
--rw-r--r--   0        0        0    13251 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/schema/aliased.py
--rw-r--r--   0        0        0     1201 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/schema/base.py
--rw-r--r--   0        0        0      489 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/openapi/schema/unified.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/py.typed
--rw-r--r--   0        0        0      655 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/topology/__init__.py
--rw-r--r--   0        0        0     2013 2024-04-28 17:47:05.374871 tubeulator-0.0.9/src/tubeulator/topology/combine.py
--rw-r--r--   0        0        0     1934 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/topology/data_model.py
--rw-r--r--   0        0        0      592 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/topology/gtfs_data_model.py
--rw-r--r--   0        0        0     1117 2024-04-28 17:47:05.374871 tubeulator-0.0.9/src/tubeulator/topology/load.py
--rw-r--r--   0        0        0     1206 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/topology/load_gtfs.py
--rw-r--r--   0        0        0     2110 2024-04-28 17:47:05.374871 tubeulator-0.0.9/src/tubeulator/topology/map.py
--rw-r--r--   0        0        0        0 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/utils/__init__.py
--rw-r--r--   0        0        0     4521 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/utils/lcp_trie.py
--rw-r--r--   0        0        0      670 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/utils/logs.py
--rw-r--r--   0        0        0     1508 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/utils/paths.py
--rw-r--r--   0        0        0     1874 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/utils/schemas.py
--rw-r--r--   0        0        0     2297 2024-04-28 17:46:43.803245 tubeulator-0.0.9/src/tubeulator/utils/string_conv.py
--rw-r--r--   0        0        0       65 2024-04-28 17:46:43.803245 tubeulator-0.0.9/tests/core_test.py
--rw-r--r--   0        0        0      281 2024-04-28 17:46:43.803245 tubeulator-0.0.9/tests/dto_test.py
--rw-r--r--   0        0        0      212 2024-04-28 17:46:43.803245 tubeulator-0.0.9/tests/fetch_test.py
--rw-r--r--   0        0        0      732 2024-04-28 17:46:43.803245 tubeulator-0.0.9/tests/topo_combine_test.py
--rw-r--r--   0        0        0      563 2024-04-28 17:46:43.803245 tubeulator-0.0.9/tests/topo_load_test.py
--rw-r--r--   0        0        0    13170 1970-01-01 00:00:00.000000 tubeulator-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-19 21:42:27.992632 tubeulator-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    12108 2024-05-19 21:42:27.992632 tubeulator-0.1.0/README.md
+-rw-r--r--   0        0        0     1980 2024-05-19 21:44:22.366636 tubeulator-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      625 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/__init__.py
+-rw-r--r--   0        0        0       76 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/__init__.py
+-rw-r--r--   0        0        0      541 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/names.py
+-rw-r--r--   0        0        0     1225 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/accident.py
+-rw-r--r--   0        0        0      138 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/air.py
+-rw-r--r--   0        0        0      877 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/bike.py
+-rw-r--r--   0        0        0      357 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/crowding.py
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/disruption_lifts.py
+-rw-r--r--   0        0        0      395 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/journey.py
+-rw-r--r--   0        0        0     3015 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/line.py
+-rw-r--r--   0        0        0      313 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/mode.py
+-rw-r--r--   0        0        0      588 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/occupancy.py
+-rw-r--r--   0        0        0     1331 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/place.py
+-rw-r--r--   0        0        0      987 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/road.py
+-rw-r--r--   0        0        0      674 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/search.py
+-rw-r--r--   0        0        0     2941 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/stop.py
+-rw-r--r--   0        0        0      415 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/types.py
+-rw-r--r--   0        0        0      390 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/vehicle.py
+-rw-r--r--   0        0        0      784 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/interface.py
+-rw-r--r--   0        0        0    18440 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/api/request.py
+-rw-r--r--   0        0        0     1920 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/cli.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/gen/__init__.py
+-rw-r--r--   0        0        0    13797 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/gen/dto.py
+-rw-r--r--   0        0        0     2880 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/gen/emit.py
+-rw-r--r--   0        0        0      566 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/gen/helpers.py
+-rw-r--r--   0        0        0      735 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/gen/jsonschema.py
+-rw-r--r--   0        0        0     2204 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/gen/resolution.py
+-rw-r--r--   0        0        0      538 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/load_test.py
+-rw-r--r--   0        0        0      658 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/codegen/populate.py
+-rw-r--r--   0        0        0    10306 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json
+-rw-r--r--   0        0        0      812 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json
+-rw-r--r--   0        0        0      683 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/all.json
+-rw-r--r--   0        0        0      344 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/casualty.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:27.992632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
+-rw-r--r--   0        0        0      135 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/vehicle.json
+-rw-r--r--   0        0        0     2473 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AirQuality/AirQuality.json
+-rw-r--r--   0        0        0       67 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AirQuality/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/AirQuality/schemas/object.json
+-rw-r--r--   0        0        0    12586 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/BikePoint.json
+-rw-r--r--   0        0        0      359 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/additionalproperties.json
+-rw-r--r--   0        0        0      788 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/all.json
+-rw-r--r--   0        0        0     1491 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/place.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-1.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-2.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-3.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-4.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-5.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-6.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray-7.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/tfl-api-presentation-entities-placearray.json
+-rw-r--r--   0        0        0     3569 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json
+-rw-r--r--   0        0        0      132 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/all.json
+-rw-r--r--   0        0        0      120 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      828 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json
+-rw-r--r--   0        0        0    64106 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/Journey.json
+-rw-r--r--   0        0        0     1988 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/metamodesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/metamodesget200textxmlresponse.json
+-rw-r--r--   0        0        0      873 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json
+-rw-r--r--   0        0        0      620 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json
+-rw-r--r--   0        0        0      350 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-12.json
+-rw-r--r--   0        0        0      424 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-13.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-14.json
+-rw-r--r--   0        0        0      243 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-15.json
+-rw-r--r--   0        0        0      359 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-16.json
+-rw-r--r--   0        0        0     1418 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json
+-rw-r--r--   0        0        0     2645 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json
+-rw-r--r--   0        0        0      218 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-19.json
+-rw-r--r--   0        0        0      180 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1362 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json
+-rw-r--r--   0        0        0     1892 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json
+-rw-r--r--   0        0        0      355 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-22.json
+-rw-r--r--   0        0        0     1294 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json
+-rw-r--r--   0        0        0      464 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-24.json
+-rw-r--r--   0        0        0      194 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-25.json
+-rw-r--r--   0        0        0      711 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json
+-rw-r--r--   0        0        0      179 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-27.json
+-rw-r--r--   0        0        0      368 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-28.json
+-rw-r--r--   0        0        0      561 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json
+-rw-r--r--   0        0        0     1324 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json
+-rw-r--r--   0        0        0      550 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json
+-rw-r--r--   0        0        0      714 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json
+-rw-r--r--   0        0        0     1335 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json
+-rw-r--r--   0        0        0      178 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-33.json
+-rw-r--r--   0        0        0      858 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json
+-rw-r--r--   0        0        0      552 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json
+-rw-r--r--   0        0        0      268 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-36.json
+-rw-r--r--   0        0        0      297 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-37.json
+-rw-r--r--   0        0        0      345 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-38.json
+-rw-r--r--   0        0        0      263 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-39.json
+-rw-r--r--   0        0        0      285 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-4.json
+-rw-r--r--   0        0        0      743 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json
+-rw-r--r--   0        0        0      302 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-5.json
+-rw-r--r--   0        0        0      453 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-6.json
+-rw-r--r--   0        0        0      378 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-7.json
+-rw-r--r--   0        0        0     1062 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json
+-rw-r--r--   0        0        0      511 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-9.json
+-rw-r--r--   0        0        0      304 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl.json
+-rw-r--r--   0        0        0   232588 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/Line.json
+-rw-r--r--   0        0        0     7137 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:27.996632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/id-stoppointsget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivals-stoppointid-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-arrivalsget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-status-startdate-to-enddate-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-statusget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/ids-statusget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metadisruptioncategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metamodesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metamodesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metamodesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaservicetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaseverityget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/metaseverityget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/mode-modes-statusget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/status-severity-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/status-severity-get200textxmlresponse.json
+-rw-r--r--   0        0        0     1417 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-10.json
+-rw-r--r--   0        0        0     2641 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-11.json
+-rw-r--r--   0        0        0      218 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-12.json
+-rw-r--r--   0        0        0     1362 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-13.json
+-rw-r--r--   0        0        0     1892 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-14.json
+-rw-r--r--   0        0        0      550 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-15.json
+-rw-r--r--   0        0        0      714 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-16.json
+-rw-r--r--   0        0        0     1335 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-17.json
+-rw-r--r--   0        0        0      178 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-18.json
+-rw-r--r--   0        0        0      858 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-19.json
+-rw-r--r--   0        0        0      269 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1221 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-20.json
+-rw-r--r--   0        0        0     1232 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-21.json
+-rw-r--r--   0        0        0      285 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-22.json
+-rw-r--r--   0        0        0      762 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-23.json
+-rw-r--r--   0        0        0      477 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-24.json
+-rw-r--r--   0        0        0      159 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-25.json
+-rw-r--r--   0        0        0      829 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-26.json
+-rw-r--r--   0        0        0      244 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-27.json
+-rw-r--r--   0        0        0      216 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-28.json
+-rw-r--r--   0        0        0      237 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-29.json
+-rw-r--r--   0        0        0      378 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-3.json
+-rw-r--r--   0        0        0      257 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-30.json
+-rw-r--r--   0        0        0      181 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-31.json
+-rw-r--r--   0        0        0      254 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-32.json
+-rw-r--r--   0        0        0      408 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-33.json
+-rw-r--r--   0        0        0      458 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-34.json
+-rw-r--r--   0        0        0      306 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-35.json
+-rw-r--r--   0        0        0      247 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-36.json
+-rw-r--r--   0        0        0      185 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-37.json
+-rw-r--r--   0        0        0      207 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-38.json
+-rw-r--r--   0        0        0      654 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-39.json
+-rw-r--r--   0        0        0     1062 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-4.json
+-rw-r--r--   0        0        0      529 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-40.json
+-rw-r--r--   0        0        0     2708 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-41.json
+-rw-r--r--   0        0        0      511 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-5.json
+-rw-r--r--   0        0        0      873 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-6.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-7.json
+-rw-r--r--   0        0        0      243 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-8.json
+-rw-r--r--   0        0        0      359 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-9.json
+-rw-r--r--   0        0        0      304 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl.json
+-rw-r--r--   0        0        0    19274 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/Mode.json
+-rw-r--r--   0        0        0      186 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/activeservicetype.json
+-rw-r--r--   0        0        0      939 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/all.json
+-rw-r--r--   0        0        0     2748 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/prediction.json
+-rw-r--r--   0        0        0      529 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-activeservicetypearray.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-4.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-5.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.000632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-6.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/tfl-api-presentation-entities-predictionarray-7.json
+-rw-r--r--   0        0        0    42059 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/Place.json
+-rw-r--r--   0        0        0     2157 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/all.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse-1.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/id-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/id-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/id-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/id-get200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/metaplacetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/searchget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/searchget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/searchget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/searchget200textxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/system.json
+-rw-r--r--   0        0        0     2640 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-10.json
+-rw-r--r--   0        0        0      359 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1416 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-3.json
+-rw-r--r--   0        0        0      378 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-4.json
+-rw-r--r--   0        0        0     1062 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-5.json
+-rw-r--r--   0        0        0      511 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-6.json
+-rw-r--r--   0        0        0      873 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-7.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-8.json
+-rw-r--r--   0        0        0      243 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-9.json
+-rw-r--r--   0        0        0      242 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/type-types-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/type-types-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/type-types-get200textxmlresponse.json
+-rw-r--r--   0        0        0      822 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/README.md
+-rw-r--r--   0        0        0   112822 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/Road.json
+-rw-r--r--   0        0        0     2250 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/all.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/get200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationgeo-jsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-statusget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/ids-statusget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/metaseveritiesget200textxmlresponse.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/system-2.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/system-3.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/system.json
+-rw-r--r--   0        0        0      813 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-2.json
+-rw-r--r--   0        0        0     1501 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-3.json
+-rw-r--r--   0        0        0     1358 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-4.json
+-rw-r--r--   0        0        0      579 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-5.json
+-rw-r--r--   0        0        0      519 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-6.json
+-rw-r--r--   0        0        0      245 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-7.json
+-rw-r--r--   0        0        0     5927 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-8.json
+-rw-r--r--   0        0        0      269 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-9.json
+-rw-r--r--   0        0        0     1958 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl.json
+-rw-r--r--   0        0        0    20177 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/Search.json
+-rw-r--r--   0        0        0      985 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/all.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasearchprovidersget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasortsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasortsget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/metasortsget200textxmlresponse.json
+-rw-r--r--   0        0        0      642 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/tfl-2.json
+-rw-r--r--   0        0        0      358 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/tfl.json
+-rw-r--r--   0        0        0   137945 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/StopPoint.json
+-rw-r--r--   0        0        0     6467 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/all.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivaldeparturesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.004632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-arrivalsget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-canreachonline-lineid-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-crowding-line-get200textxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-directionto-tostoppointid-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-placetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/id-routeget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      109 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metamodesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/metastoptypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/mode-modes-disruptionget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/servicetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-carparksget200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/stoppointid-taxiranksget200textxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/system.json
+-rw-r--r--   0        0        0     1417 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json
+-rw-r--r--   0        0        0     2641 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json
+-rw-r--r--   0        0        0      178 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-12.json
+-rw-r--r--   0        0        0      209 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-13.json
+-rw-r--r--   0        0        0      258 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-14.json
+-rw-r--r--   0        0        0      529 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json
+-rw-r--r--   0        0        0     2708 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json
+-rw-r--r--   0        0        0     1869 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json
+-rw-r--r--   0        0        0      755 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json
+-rw-r--r--   0        0        0      646 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json
+-rw-r--r--   0        0        0      304 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-2.json
+-rw-r--r--   0        0        0      967 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json
+-rw-r--r--   0        0        0      358 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-21.json
+-rw-r--r--   0        0        0      645 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json
+-rw-r--r--   0        0        0      378 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-3.json
+-rw-r--r--   0        0        0     1062 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json
+-rw-r--r--   0        0        0      511 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-5.json
+-rw-r--r--   0        0        0      873 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-7.json
+-rw-r--r--   0        0        0      243 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-8.json
+-rw-r--r--   0        0        0      359 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-9.json
+-rw-r--r--   0        0        0      242 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-get200textxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textjsonresponse.json
+-rw-r--r--   0        0        0      112 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/type-types-page-page-get200textxmlresponse.json
+-rw-r--r--   0        0        0    15378 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/Vehicle.json
+-rw-r--r--   0        0        0      425 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/all.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/ids-arrivalsget200textxmlresponse.json
+-rw-r--r--   0        0        0     2705 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json
+-rw-r--r--   0        0        0      495 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/tfl-3.json
+-rw-r--r--   0        0        0      529 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json
+-rw-r--r--   0        0        0     3579 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/crowding/crowding.json
+-rw-r--r--   0        0        0     5361 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/error_inventory.md
+-rw-r--r--   0        0        0    11496 2024-05-19 21:42:28.008632 tubeulator-0.1.0/src/tubeulator/data/openapi/namespace.json
+-rw-r--r--   0        0        0     7685 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/naming.md
+-rw-r--r--   0        0        0    24650 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/occupancy.json
+-rw-r--r--   0        0        0     1365 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/all.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/bikepoints-ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/carparkget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/carparkget200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnector-ids-get200textxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textjsonresponse.json
+-rw-r--r--   0        0        0      111 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/chargeconnectorget200textxmlresponse.json
+-rw-r--r--   0        0        0      330 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/tfl-2.json
+-rw-r--r--   0        0        0      360 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/tfl-3.json
+-rw-r--r--   0        0        0      697 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json
+-rw-r--r--   0        0        0      356 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/tfl.json
+-rw-r--r--   0        0        0     1503 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi/stationdata/stationdata.json
+-rw-r--r--   0        0        0   676093 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json
+-rw-r--r--   0        0        0      812 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json
+-rw-r--r--   0        0        0      283 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentstatsorderedsummary.json
+-rw-r--r--   0        0        0      186 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/activeservicetype.json
+-rw-r--r--   0        0        0      359 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/additionalproperties.json
+-rw-r--r--   0        0        0    29934 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json
+-rw-r--r--   0        0        0      361 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/apiversioninfo.json
+-rw-r--r--   0        0        0     1909 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json
+-rw-r--r--   0        0        0      356 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bay.json
+-rw-r--r--   0        0        0      697 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json
+-rw-r--r--   0        0        0      360 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/carparkoccupancy.json
+-rw-r--r--   0        0        0      344 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/casualty.json
+-rw-r--r--   0        0        0      360 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/chargeconnectoroccupancy.json
+-rw-r--r--   0        0        0      531 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json
+-rw-r--r--   0        0        0      586 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json
+-rw-r--r--   0        0        0     1378 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json
+-rw-r--r--   0        0        0      245 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterange.json
+-rw-r--r--   0        0        0      245 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/daterangenullable.json
+-rw-r--r--   0        0        0      184 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeography.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/dbgeographywellknownvalue.json
+-rw-r--r--   0        0        0      262 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguation.json
+-rw-r--r--   0        0        0      185 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disambiguationoption.json
+-rw-r--r--   0        0        0      646 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json
+-rw-r--r--   0        0        0     1961 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json
+-rw-r--r--   0        0        0      757 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json
+-rw-r--r--   0        0        0      860 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json
+-rw-r--r--   0        0        0      179 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farecaveat.json
+-rw-r--r--   0        0        0     1483 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json
+-rw-r--r--   0        0        0      254 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresmode.json
+-rw-r--r--   0        0        0      443 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faresperiod.json
+-rw-r--r--   0        0        0      571 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json
+-rw-r--r--   0        0        0      364 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farestation.json
+-rw-r--r--   0        0        0      247 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretap.json
+-rw-r--r--   0        0        0      464 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faretapdetails.json
+-rw-r--r--   0        0        0      695 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json
+-rw-r--r--   0        0        0      271 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geopoint.json
+-rw-r--r--   0        0        0      877 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json
+-rw-r--r--   0        0        0      325 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instruction.json
+-rw-r--r--   0        0        0     1362 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json
+-rw-r--r--   0        0        0      216 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/interval.json
+-rw-r--r--   0        0        0     1002 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json
+-rw-r--r--   0        0        0      653 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json
+-rw-r--r--   0        0        0      460 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyfare.json
+-rw-r--r--   0        0        0      552 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json
+-rw-r--r--   0        0        0      263 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyvector.json
+-rw-r--r--   0        0        0      620 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json
+-rw-r--r--   0        0        0      257 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/knownjourney.json
+-rw-r--r--   0        0        0     1649 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json
+-rw-r--r--   0        0        0     1038 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json
+-rw-r--r--   0        0        0      307 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linegroup.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetadisruptioncategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.012632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemetaservicetypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      243 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linemodegroup.json
+-rw-r--r--   0        0        0      477 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineroutesection.json
+-rw-r--r--   0        0        0      305 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetype.json
+-rw-r--r--   0        0        0      178 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/lineservicetypeinfo.json
+-rw-r--r--   0        0        0      252 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linespecificservicetype.json
+-rw-r--r--   0        0        0      786 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json
+-rw-r--r--   0        0        0     1335 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json
+-rw-r--r--   0        0        0      159 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroutesections.json
+-rw-r--r--   0        0        0     1256 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json
+-rw-r--r--   0        0        0      357 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/message.json
+-rw-r--r--   0        0        0      304 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/mode.json
+-rw-r--r--   0        0        0      361 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/networkstatus.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/object.json
+-rw-r--r--   0        0        0      302 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/obstacle.json
+-rw-r--r--   0        0        0      285 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/orderedroute.json
+-rw-r--r--   0        0        0      378 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengerflow.json
+-rw-r--r--   0        0        0      315 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/passengertype.json
+-rw-r--r--   0        0        0      419 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/path.json
+-rw-r--r--   0        0        0      180 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/pathattribute.json
+-rw-r--r--   0        0        0      542 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json
+-rw-r--r--   0        0        0     1491 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json
+-rw-r--r--   0        0        0      242 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placecategory.json
+-rw-r--r--   0        0        0      513 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json
+-rw-r--r--   0        0        0      262 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placepolygon.json
+-rw-r--r--   0        0        0      355 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/plannedwork.json
+-rw-r--r--   0        0        0      453 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/point.json
+-rw-r--r--   0        0        0      403 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/postcodeinput.json
+-rw-r--r--   0        0        0     2748 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json
+-rw-r--r--   0        0        0      529 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json
+-rw-r--r--   0        0        0     1340 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json
+-rw-r--r--   0        0        0      245 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendationresponse.json
+-rw-r--r--   0        0        0      233 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/redirect.json
+-rw-r--r--   0        0        0     1958 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json
+-rw-r--r--   0        0        0     6179 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json
+-rw-r--r--   0        0        0      542 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json
+-rw-r--r--   0        0        0      602 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json
+-rw-r--r--   0        0        0      245 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionschedule.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadmetacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0     1358 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json
+-rw-r--r--   0        0        0      458 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routeoption.json
+-rw-r--r--   0        0        0      948 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json
+-rw-r--r--   0        0        0      284 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchresponse.json
+-rw-r--r--   0        0        0     1417 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json
+-rw-r--r--   0        0        0      251 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesectionnaptanentrysequence.json
+-rw-r--r--   0        0        0      874 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json
+-rw-r--r--   0        0        0      596 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json
+-rw-r--r--   0        0        0      399 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchcriteria.json
+-rw-r--r--   0        0        0      358 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmatch.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetacategoriesget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasearchprovidersget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchmetasortsget200textxmlresponse.json
+-rw-r--r--   0        0        0      680 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json
+-rw-r--r--   0        0        0      254 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/servicefrequency.json
+-rw-r--r--   0        0        0      269 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stationinterval.json
+-rw-r--r--   0        0        0      269 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/statusseverity.json
+-rw-r--r--   0        0        0     2822 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json
+-rw-r--r--   0        0        0      242 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointcategory.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200applicationxmlresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textjsonresponse.json
+-rw-r--r--   0        0        0       69 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointiddirectiontotostoppointidget200textxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200applicationxmlresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textjsonresponse.json
+-rw-r--r--   0        0        0      107 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointmetastoptypesget200textxmlresponse.json
+-rw-r--r--   0        0        0      755 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json
+-rw-r--r--   0        0        0     1267 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json
+-rw-r--r--   0        0        0     1000 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json
+-rw-r--r--   0        0        0     1539 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json
+-rw-r--r--   0        0        0      813 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-1.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-2.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray-3.json
+-rw-r--r--   0        0        0      164 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-accidentstats-accidentdetailarray.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-1.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-2.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray-3.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-activeservicetypearray.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-1.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-2.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray-3.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-arrivaldeparturearray.json
+-rw-r--r--   0        0        0      154 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-1.json
+-rw-r--r--   0        0        0      154 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-2.json
+-rw-r--r--   0        0        0      154 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray-3.json
+-rw-r--r--   0        0        0      154 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-bikepointoccupancyarray.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-1.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-2.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray-3.json
+-rw-r--r--   0        0        0      152 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-carparkoccupancyarray.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-1.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-2.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-3.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-4.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-5.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-6.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray-7.json
+-rw-r--r--   0        0        0      160 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-chargeconnectoroccupancyarray.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-1.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-2.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-3.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-4.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-5.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-6.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray-7.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptedpointarray.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-1.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-2.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.016632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-3.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-4.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-5.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-6.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray-7.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-disruptionarray.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-1.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-10.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-11.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-12.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-13.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-14.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-15.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-16.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-17.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-18.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-19.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-2.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-20.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-21.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-22.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-23.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-24.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-25.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-26.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-27.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-28.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-29.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-3.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-30.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-31.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-32.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-33.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-34.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-35.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-4.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-5.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-6.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-7.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-8.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray-9.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-linearray.json
+-rw-r--r--   0        0        0      151 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-1.json
+-rw-r--r--   0        0        0      151 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-2.json
+-rw-r--r--   0        0        0      151 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray-3.json
+-rw-r--r--   0        0        0      151 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-lineservicetypearray.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-1.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-10.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-11.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-2.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-3.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-4.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-5.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-6.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-7.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-8.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray-9.json
+-rw-r--r--   0        0        0      140 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-modearray.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-1.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-10.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-11.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-12.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-13.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-14.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-15.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-16.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-17.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-18.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-19.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-2.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-20.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-21.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-22.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-23.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-24.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-25.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-26.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-27.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-28.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-29.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-3.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-30.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-31.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-4.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-5.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-6.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-7.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-8.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray-9.json
+-rw-r--r--   0        0        0      141 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placearray.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-1.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-2.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-3.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-4.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-5.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-6.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray-7.json
+-rw-r--r--   0        0        0      149 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-placecategoryarray.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-1.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-10.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-11.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-12.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-13.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-14.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-15.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-2.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-3.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-4.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-5.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-6.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-7.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-8.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray-9.json
+-rw-r--r--   0        0        0      146 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-predictionarray.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-1.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.020632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-10.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-11.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-2.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-3.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-4.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-5.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-6.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-7.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-8.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray-9.json
+-rw-r--r--   0        0        0      148 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roadcorridorarray.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-1.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-2.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-3.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray-4.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-roaddisruptionarray.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-1.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-2.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-3.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-4.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-5.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-6.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray-7.json
+-rw-r--r--   0        0        0      150 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-statusseverityarray.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-1.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-10.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-11.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-12.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-13.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-14.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-15.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-16.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-17.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-18.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-19.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-2.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-20.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-21.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-22.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-23.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-24.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-25.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-26.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-27.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-3.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-4.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-5.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-6.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-7.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-8.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray-9.json
+-rw-r--r--   0        0        0      145 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointarray.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-1.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-2.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray-3.json
+-rw-r--r--   0        0        0      153 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointcategoryarray.json
+-rw-r--r--   0        0        0      157 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-1.json
+-rw-r--r--   0        0        0      157 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-2.json
+-rw-r--r--   0        0        0      157 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray-3.json
+-rw-r--r--   0        0        0      157 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tfl-api-presentation-entities-stoppointroutesectionarray.json
+-rw-r--r--   0        0        0      685 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json
+-rw-r--r--   0        0        0      186 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettime.json
+-rw-r--r--   0        0        0      186 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/tickettype.json
+-rw-r--r--   0        0        0      268 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustment.json
+-rw-r--r--   0        0        0      509 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timeadjustments.json
+-rw-r--r--   0        0        0      285 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetable.json
+-rw-r--r--   0        0        0      806 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json
+-rw-r--r--   0        0        0      377 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableroute.json
+-rw-r--r--   0        0        0     1062 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json
+-rw-r--r--   0        0        0      181 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/twentyfourhourclocktime.json
+-rw-r--r--   0        0        0      550 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json
+-rw-r--r--   0        0        0      135 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehicle.json
+-rw-r--r--   0        0        0      495 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/vehiclematch.json
+-rw-r--r--   0        0        0      126 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/FeedInfo.csv
+-rw-r--r--   0        0        0    54508 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Lifts.csv
+-rw-r--r--   0        0        0      347 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/ModesAndLines.csv
+-rw-r--r--   0        0        0   168607 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/PlatformServices.csv
+-rw-r--r--   0        0        0   145838 2024-05-19 21:42:28.024632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Platforms.csv
+-rw-r--r--   0        0        0    20909 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/RampRoutes.csv
+-rw-r--r--   0        0        0   389058 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv
+-rw-r--r--   0        0        0   273465 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/StationPoints.csv
+-rw-r--r--   0        0        0    37832 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Stations.csv
+-rw-r--r--   0        0        0     8344 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv
+-rw-r--r--   0        0        0    28533 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Toilets.csv
+-rw-r--r--   0        0        0      119 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/gtfs/feed_info.txt
+-rw-r--r--   0        0        0      135 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/gtfs/levels.txt
+-rw-r--r--   0        0        0   548638 2024-05-19 21:42:28.028632 tubeulator-0.1.0/src/tubeulator/data/stationdata/gtfs/pathways.txt
+-rw-r--r--   0        0        0   430539 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/data/stationdata/gtfs/stops.txt
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/db/__init__.py
+-rw-r--r--   0        0        0     2290 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/db/mongod.py
+-rw-r--r--   0        0        0     1992 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/db/store_creds.py
+-rw-r--r--   0        0        0      722 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/exc.py
+-rw-r--r--   0        0        0     2947 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/AccidentStats.py
+-rw-r--r--   0        0        0      699 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/AirQuality.py
+-rw-r--r--   0        0        0     2232 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/BikePoint.py
+-rw-r--r--   0        0        0     1469 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/DisruptionsLiftsv2.py
+-rw-r--r--   0        0        0    25936 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Journey.py
+-rw-r--r--   0        0        0    36702 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Line.py
+-rw-r--r--   0        0        0     3711 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Mode.py
+-rw-r--r--   0        0        0    10716 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Place.py
+-rw-r--r--   0        0        0    11713 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Road.py
+-rw-r--r--   0        0        0     2965 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Search.py
+-rw-r--r--   0        0        0    16645 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/StopPoint.py
+-rw-r--r--   0        0        0     3067 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/Vehicle.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/crowding.py
+-rw-r--r--   0        0        0     2808 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/occupancy.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/generated/stationdata.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/_types.py
+-rw-r--r--   0        0        0     3063 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/dataclass_generator.py
+-rw-r--r--   0        0        0     1643 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/fetch.py
+-rw-r--r--   0        0        0     2028 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/reference.py
+-rw-r--r--   0        0        0     1971 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/scan.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/schema/__init__.py
+-rw-r--r--   0        0        0    13251 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/schema/aliased.py
+-rw-r--r--   0        0        0     1201 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/schema/base.py
+-rw-r--r--   0        0        0      489 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/openapi/schema/unified.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/py.typed
+-rw-r--r--   0        0        0      655 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/__init__.py
+-rw-r--r--   0        0        0     2013 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/combine.py
+-rw-r--r--   0        0        0     1934 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/data_model.py
+-rw-r--r--   0        0        0      592 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/gtfs_data_model.py
+-rw-r--r--   0        0        0     1117 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/load.py
+-rw-r--r--   0        0        0     1206 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/load_gtfs.py
+-rw-r--r--   0        0        0     2110 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/topology/map.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/utils/__init__.py
+-rw-r--r--   0        0        0     4521 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/utils/lcp_trie.py
+-rw-r--r--   0        0        0      670 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/utils/logs.py
+-rw-r--r--   0        0        0     1508 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/utils/paths.py
+-rw-r--r--   0        0        0     1874 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/utils/schemas.py
+-rw-r--r--   0        0        0     2297 2024-05-19 21:42:28.032632 tubeulator-0.1.0/src/tubeulator/utils/string_conv.py
+-rw-r--r--   0        0        0       65 2024-05-19 21:42:28.032632 tubeulator-0.1.0/tests/core_test.py
+-rw-r--r--   0        0        0      281 2024-05-19 21:42:28.032632 tubeulator-0.1.0/tests/dto_test.py
+-rw-r--r--   0        0        0    11820 2024-05-19 21:42:28.032632 tubeulator-0.1.0/tests/fetch_test.py
+-rw-r--r--   0        0        0      732 2024-05-19 21:42:28.032632 tubeulator-0.1.0/tests/topo_combine_test.py
+-rw-r--r--   0        0        0      563 2024-05-19 21:42:28.032632 tubeulator-0.1.0/tests/topo_load_test.py
+-rw-r--r--   0        0        0    13171 1970-01-01 00:00:00.000000 tubeulator-0.1.0/PKG-INFO
```

### Comparing `tubeulator-0.0.9/LICENSE.txt` & `tubeulator-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/README.md` & `tubeulator-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tubeulator
 
 > It's time for the tubeulator
 
-TfL open data interface library
+TfL open data interface library.
 
 ## Key features
 
 - Route planning (underground, overground, bus, walking)
 - Time estimation taking into account mixed modes of travel in one journey
 
 ## Requires
```

### Comparing `tubeulator-0.0.9/pyproject.toml` & `tubeulator-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "pymongo",
     "urllib3<2",
 ]
 description = "TfL open data interface library."
 name = "tubeulator"
 readme = "README.md"
 requires-python = ">=3.10,<3.13"
-version = "0.0.9"
+version = "0.1.0"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 folium = [
     "folium>=0.16.0",
@@ -59,14 +59,17 @@
 docs = [
     "mkdocs-material[recommended,imaging]>=9.5.2",
     "mkdocs-section-index>=0.3.8",
     "mkdocs>=1.5.3",
     "mkdocstrings[python]>=0.24.0",
 ]
 test = [
+    "inline-snapshot>=0.9.0",
+    "pytest-custom-exit-code>=0.3.0",
+    "pytest-xdist>=3.6.1",
     "pytest>=7.4.0",
 ]
 vercel = [
     "urllib3<2",
 ]
 
 [tool.pdm.resolution]
```

### Comparing `tubeulator-0.0.9/src/tubeulator/__init__.py` & `tubeulator-0.1.0/src/tubeulator/__init__.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/names.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/names.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/__init__.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/bike.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/bike.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/line.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/line.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/occupancy.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/occupancy.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/place.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/place.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/road.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/road.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/search.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/search.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/endpoint/routes/stop.py` & `tubeulator-0.1.0/src/tubeulator/api/endpoint/routes/stop.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/interface.py` & `tubeulator-0.1.0/src/tubeulator/api/interface.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/api/request.py` & `tubeulator-0.1.0/src/tubeulator/api/request.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/cli.py` & `tubeulator-0.1.0/src/tubeulator/cli.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/gen/dto.py` & `tubeulator-0.1.0/src/tubeulator/codegen/gen/dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             prop_type = f"{prop_type}Model"
         if prop_name in required:
             default = ""
         else:
             if is_array_prop:
                 contains_list = True
                 if is_pydantic:
-                    default = ""
+                    default = " = []"
                 else:
                     default = " = field(default_factory=list)"
             else:
                 default = " = None"
         dc_source += f"    {to_pascal_case(prop_name)}: {prop_type}{default}\n"
     source_schema_default = hidden_field(schema_name, style=style)
     component_default = hidden_field(component_name, style=style)
```

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/gen/emit.py` & `tubeulator-0.1.0/src/tubeulator/codegen/gen/emit.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/gen/helpers.py` & `tubeulator-0.1.0/src/tubeulator/codegen/gen/helpers.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/gen/jsonschema.py` & `tubeulator-0.1.0/src/tubeulator/codegen/gen/jsonschema.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/gen/resolution.py` & `tubeulator-0.1.0/src/tubeulator/codegen/gen/resolution.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/load_test.py` & `tubeulator-0.1.0/src/tubeulator/codegen/load_test.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/codegen/populate.py` & `tubeulator-0.1.0/src/tubeulator/codegen/populate.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/AccidentStats.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/accidentdetail.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/AccidentStats/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/AccidentStats/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/AirQuality/AirQuality.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/AirQuality/AirQuality.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/BikePoint.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/BikePoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/BikePoint/schemas/place.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/BikePoint/schemas/place.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Disruptions-Lifts-v2/Disruptions-Lifts-v2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Disruptions-Lifts-v2/schemas/liftdisruption.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/Journey.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/Journey.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-11.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-17.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-18.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-20.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-21.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-23.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-26.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-29.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-3.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-30.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-31.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-32.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-34.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-35.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-40.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Journey/schemas/tfl-8.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/Line.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/Line.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-10.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-11.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-11.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-13.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-13.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-14.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-14.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-15.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-15.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-16.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-16.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-17.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-17.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-19.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-19.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-20.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-20.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-21.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-21.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-23.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-23.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-26.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-26.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-39.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-39.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-4.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-40.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-40.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-41.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-41.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Line/schemas/tfl-6.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Line/schemas/tfl-6.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/Mode.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/Mode.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/prediction.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/prediction.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Mode/schemas/predictiontiming.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Place/Place.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Place/Place.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-10.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-3.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-3.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-5.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-5.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Place/schemas/tfl-7.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Place/schemas/tfl-7.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/README.md` & `tubeulator-0.1.0/src/tubeulator/data/openapi/README.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/Road.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/Road.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-2.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-3.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-3.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-4.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-5.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-5.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-6.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-6.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl-8.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl-8.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Road/schemas/tfl.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Road/schemas/tfl.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Search/Search.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Search/Search.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Search/schemas/tfl-2.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Search/schemas/tfl-2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/StopPoint.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/StopPoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-10.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-11.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-15.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-16.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-17.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-18.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-19.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-20.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-22.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/StopPoint/schemas/tfl-6.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/Vehicle.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/Vehicle.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/tfl-2.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/Vehicle/schemas/tfl.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/crowding/crowding.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/crowding/crowding.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/error_inventory.md` & `tubeulator-0.1.0/src/tubeulator/data/openapi/error_inventory.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/namespace.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/namespace.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/naming.md` & `tubeulator-0.1.0/src/tubeulator/data/openapi/naming.md`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/occupancy.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/occupancy.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/occupancy/schemas/tfl-4.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi/stationdata/stationdata.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi/stationdata/stationdata.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/ReleasedUnifiedAPIProd.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/accidentdetail.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/all.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/arrivaldeparture.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/bikepointoccupancy.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/coordinate.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/crowding.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/cyclesuperhighway.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruptedpoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/disruption.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/fare.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/farebounds.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faredetails.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/faressection.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/geocodesearchmatch.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/identifier.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/instructionstep.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/itineraryresult.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journey.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/journeyplannercyclehiredockingstationdata.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/jpelevation.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/leg.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/line.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/linestatus.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedroute.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/matchedstop.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/period.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/place.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/placegeo.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/prediction.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/predictiontiming.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/recommendation.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadcorridor.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruption.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionimpactarea.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roaddisruptionline.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/roadproject.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesearchmatch.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesection.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/routesequence.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/schedule.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/searchresponse.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppoint.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointroutesection.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsequence.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/stoppointsresponse.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/street.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/streetsegment.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/ticket.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/timetableresponse.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/trainloading.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json` & `tubeulator-0.1.0/src/tubeulator/data/openapi_unified/ReleasedUnifiedAPIProd/schemas/validityperiod.json`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Lifts.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Lifts.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/PlatformServices.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/PlatformServices.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Platforms.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Platforms.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/RampRoutes.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/RampRoutes.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/SameLevelPaths.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/StationPoints.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/StationPoints.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Stations.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Stations.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/StepFreeIntechangeInfo.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/detailed/Toilets.csv` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/detailed/Toilets.csv`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/gtfs/pathways.txt` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/gtfs/pathways.txt`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/data/stationdata/gtfs/stops.txt` & `tubeulator-0.1.0/src/tubeulator/data/stationdata/gtfs/stops.txt`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/db/mongod.py` & `tubeulator-0.1.0/src/tubeulator/db/mongod.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/exc.py` & `tubeulator-0.1.0/src/tubeulator/exc.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/AccidentStats.py` & `tubeulator-0.1.0/src/tubeulator/generated/AccidentStats.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     Id: int = None
     Lat: float = None
     Lon: float = None
     Location: str = None
     Date: datetime = None
     Severity: str = None
     Borough: str = None
-    Casualties: list["CasualtyModel"]
-    Vehicles: list["VehicleModel"]
+    Casualties: list["CasualtyModel"] = []
+    Vehicles: list["VehicleModel"] = []
     _source_schema_name: str = PrivateAttr(default='AccidentStats')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.AccidentStats.AccidentDetail')
 
 
 AccidentDetailModel = AccidentDetail
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/AirQuality.py` & `tubeulator-0.1.0/src/tubeulator/generated/AirQuality.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/BikePoint.py` & `tubeulator-0.1.0/src/tubeulator/generated/BikePoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     )
 
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='BikePoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.Place')
 
 
 PlaceModel = Place
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/DisruptionsLiftsv2.py` & `tubeulator-0.1.0/src/tubeulator/generated/DisruptionsLiftsv2.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Journey.py` & `tubeulator-0.1.0/src/tubeulator/generated/Journey.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Summary: str = None
     Detailed: str = None
-    Steps: list["InstructionStepModel"]
+    Steps: list["InstructionStepModel"] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-4')
 
 
 InstructionModel = Instruction
 
 
@@ -176,16 +176,16 @@
     Autogenerated from Journey::Tfl.Api.Presentation.Entities.Crowding
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    PassengerFlows: list["PassengerFlowModel"]
-    TrainLoadings: list["TrainLoadingModel"]
+    PassengerFlows: list["PassengerFlowModel"] = []
+    TrainLoadings: list["TrainLoadingModel"] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-9')
 
 
 CrowdingModel = Crowding
 
 
@@ -242,16 +242,16 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     LineString: str = None
-    StopPoints: list["IdentifierModel"]
-    Elevation: list["JpElevationModel"]
+    StopPoints: list["IdentifierModel"] = []
+    Elevation: list["JpElevationModel"] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-12')
 
 
 PathModel = Path
 
 
@@ -262,15 +262,15 @@
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Id: str = None
     Name: str = None
-    Directions: list[str]
+    Directions: list[str] = []
     LineIdentifier: IdentifierModel = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-13')
 
 
 RouteOptionModel = RouteOption
 
@@ -282,15 +282,15 @@
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanIdReference: str = None
     StationAtcoCode: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-14')
 
 
 LineGroupModel = LineGroup
 
 
@@ -300,15 +300,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     ModeName: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-15')
 
 
 LineModeGroupModel = LineModeGroup
 
 
@@ -343,17 +343,17 @@
     )
 
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-17')
 
 
 PlaceModel = Place
@@ -368,35 +368,35 @@
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanId: str = None
     PlatformName: str = None
     Indicator: str = None
     StopLetter: str = None
-    Modes: list[str]
+    Modes: list[str] = []
     IcsCode: str = None
     SmsCode: str = None
     StopType: str = None
     StationNaptan: str = None
     AccessibilitySummary: str = None
     HubNaptanCode: str = None
-    Lines: list["IdentifierModel"]
-    LineGroup: list["LineGroupModel"]
-    LineModeGroups: list["LineModeGroupModel"]
+    Lines: list["IdentifierModel"] = []
+    LineGroup: list["LineGroupModel"] = []
+    LineModeGroups: list["LineModeGroupModel"] = []
     FullName: str = None
     NaptanMode: str = None
     Status: bool = None
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-18')
 
 
 StopPointModel = StopPoint
@@ -435,15 +435,15 @@
     Name: str = None
     LineString: str = None
     Direction: str = None
     OriginationName: str = None
     DestinationName: str = None
     ValidTo: datetime = None
     ValidFrom: datetime = None
-    RouteSectionNaptanEntrySequence: list["RouteSectionNaptanEntrySequenceModel"]
+    RouteSectionNaptanEntrySequence: list["RouteSectionNaptanEntrySequenceModel"] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-20')
 
 
 RouteSectionModel = RouteSection
 
 
@@ -460,16 +460,16 @@
     Type: str = None
     CategoryDescription: str = None
     Description: str = None
     Summary: str = None
     AdditionalInfo: str = None
     Created: datetime = None
     LastUpdate: datetime = None
-    AffectedRoutes: list["RouteSectionModel"]
-    AffectedStops: list["StopPointModel"]
+    AffectedRoutes: list["RouteSectionModel"] = []
+    AffectedStops: list["StopPointModel"] = []
     ClosureText: str = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-21')
 
 
 DisruptionModel = Disruption
 
@@ -502,24 +502,24 @@
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Duration: int = None
     Speed: str = None
     Instruction: InstructionModel = None
-    Obstacles: list["ObstacleModel"]
+    Obstacles: list["ObstacleModel"] = []
     DepartureTime: datetime = None
     ArrivalTime: datetime = None
     DeparturePoint: PointModel = None
     ArrivalPoint: PointModel = None
     Path: PathModel = None
-    RouteOptions: list["RouteOptionModel"]
+    RouteOptions: list["RouteOptionModel"] = []
     Mode: IdentifierModel = None
-    Disruptions: list["DisruptionModel"]
-    PlannedWorks: list["PlannedWorkModel"]
+    Disruptions: list["DisruptionModel"] = []
+    PlannedWorks: list["PlannedWorkModel"] = []
     Distance: float = None
     IsDisrupted: bool = None
     HasFixedLocations: bool = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-23')
 
 
@@ -579,15 +579,15 @@
     HighZone: int = None
     Cost: int = None
     ChargeProfileName: str = None
     IsHopperFare: bool = None
     ChargeLevel: str = None
     Peak: int = None
     OffPeak: int = None
-    Taps: list["FareTapModel"]
+    Taps: list["FareTapModel"] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-26')
 
 
 FareModel = Fare
 
 
@@ -615,16 +615,16 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     TotalCost: int = None
-    Fares: list["FareModel"]
-    Caveats: list["FareCaveatModel"]
+    Fares: list["FareModel"] = []
+    Caveats: list["FareCaveatModel"] = []
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-28')
 
 
 JourneyFareModel = JourneyFare
 
 
@@ -636,15 +636,15 @@
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     StartDateTime: datetime = None
     Duration: int = None
     ArrivalDateTime: datetime = None
-    Legs: list["LegModel"]
+    Legs: list["LegModel"] = []
     Fare: JourneyFareModel = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-29')
 
 
 JourneyModel = Journey
 
@@ -680,15 +680,15 @@
     Id: int = None
     LineId: str = None
     StatusSeverity: int = None
     StatusSeverityDescription: str = None
     Reason: str = None
     Created: datetime = None
     Modified: datetime = None
-    ValidityPeriods: list["ValidityPeriodModel"]
+    ValidityPeriods: list["ValidityPeriodModel"] = []
     Disruption: DisruptionModel = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-31')
 
 
 LineStatusModel = LineStatus
 
@@ -745,20 +745,20 @@
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Id: str = None
     Name: str = None
     ModeName: str = None
-    Disruptions: list["DisruptionModel"]
+    Disruptions: list["DisruptionModel"] = []
     Created: datetime = None
     Modified: datetime = None
-    LineStatuses: list["LineStatusModel"]
-    RouteSections: list["MatchedRouteModel"]
-    ServiceTypes: list["LineServiceTypeInfoModel"]
+    LineStatuses: list["LineStatusModel"] = []
+    RouteSections: list["MatchedRouteModel"] = []
+    ServiceTypes: list["LineServiceTypeInfoModel"] = []
     Crowding: CrowdingModel = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-34')
 
 
 LineModel = Line
 
@@ -869,18 +869,18 @@
     Autogenerated from Journey::Tfl.Api.Presentation.Entities.JourneyPlanner.ItineraryResult
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    Journeys: list["JourneyModel"]
-    Lines: list["LineModel"]
+    Journeys: list["JourneyModel"] = []
+    Lines: list["LineModel"] = []
     CycleHireDockingStationData: JourneyPlannerCycleHireDockingStationDataModel = None
-    StopMessages: list[str]
+    StopMessages: list[str] = []
     RecommendedMaxAgeMinutes: int = None
     SearchCriteria: SearchCriteriaModel = None
     JourneyVector: JourneyVectorModel = None
     _source_schema_name: str = PrivateAttr(default='Journey')
     _component_schema_name: str = PrivateAttr(default='Tfl-40')
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Line.py` & `tubeulator-0.1.0/src/tubeulator/generated/Line.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,16 +91,16 @@
     Autogenerated from Line::Tfl.Api.Presentation.Entities.Crowding
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    PassengerFlows: list["PassengerFlowModel"]
-    TrainLoadings: list["TrainLoadingModel"]
+    PassengerFlows: list["PassengerFlowModel"] = []
+    TrainLoadings: list["TrainLoadingModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-5')
 
 
 CrowdingModel = Crowding
 
 
@@ -135,15 +135,15 @@
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanIdReference: str = None
     StationAtcoCode: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-7')
 
 
 LineGroupModel = LineGroup
 
 
@@ -153,15 +153,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     ModeName: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-8')
 
 
 LineModeGroupModel = LineModeGroup
 
 
@@ -196,17 +196,17 @@
     )
 
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-10')
 
 
 PlaceModel = Place
@@ -221,35 +221,35 @@
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanId: str = None
     PlatformName: str = None
     Indicator: str = None
     StopLetter: str = None
-    Modes: list[str]
+    Modes: list[str] = []
     IcsCode: str = None
     SmsCode: str = None
     StopType: str = None
     StationNaptan: str = None
     AccessibilitySummary: str = None
     HubNaptanCode: str = None
-    Lines: list["IdentifierModel"]
-    LineGroup: list["LineGroupModel"]
-    LineModeGroups: list["LineModeGroupModel"]
+    Lines: list["IdentifierModel"] = []
+    LineGroup: list["LineGroupModel"] = []
+    LineModeGroups: list["LineModeGroupModel"] = []
     FullName: str = None
     NaptanMode: str = None
     Status: bool = None
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-11')
 
 
 StopPointModel = StopPoint
@@ -288,15 +288,15 @@
     Name: str = None
     LineString: str = None
     Direction: str = None
     OriginationName: str = None
     DestinationName: str = None
     ValidTo: datetime = None
     ValidFrom: datetime = None
-    RouteSectionNaptanEntrySequence: list["RouteSectionNaptanEntrySequenceModel"]
+    RouteSectionNaptanEntrySequence: list["RouteSectionNaptanEntrySequenceModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-13')
 
 
 RouteSectionModel = RouteSection
 
 
@@ -313,16 +313,16 @@
     Type: str = None
     CategoryDescription: str = None
     Description: str = None
     Summary: str = None
     AdditionalInfo: str = None
     Created: datetime = None
     LastUpdate: datetime = None
-    AffectedRoutes: list["RouteSectionModel"]
-    AffectedStops: list["StopPointModel"]
+    AffectedRoutes: list["RouteSectionModel"] = []
+    AffectedStops: list["StopPointModel"] = []
     ClosureText: str = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-14')
 
 
 DisruptionModel = Disruption
 
@@ -358,15 +358,15 @@
     Id: int = None
     LineId: str = None
     StatusSeverity: int = None
     StatusSeverityDescription: str = None
     Reason: str = None
     Created: datetime = None
     Modified: datetime = None
-    ValidityPeriods: list["ValidityPeriodModel"]
+    ValidityPeriods: list["ValidityPeriodModel"] = []
     Disruption: DisruptionModel = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-16')
 
 
 LineStatusModel = LineStatus
 
@@ -423,20 +423,20 @@
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Id: str = None
     Name: str = None
     ModeName: str = None
-    Disruptions: list["DisruptionModel"]
+    Disruptions: list["DisruptionModel"] = []
     Created: datetime = None
     Modified: datetime = None
-    LineStatuses: list["LineStatusModel"]
-    RouteSections: list["MatchedRouteModel"]
-    ServiceTypes: list["LineServiceTypeInfoModel"]
+    LineStatuses: list["LineStatusModel"] = []
+    RouteSections: list["MatchedRouteModel"] = []
+    ServiceTypes: list["LineServiceTypeInfoModel"] = []
     Crowding: CrowdingModel = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-19')
 
 
 LineModel = Line
 
@@ -453,21 +453,21 @@
     RouteId: int = None
     ParentId: str = None
     StationId: str = None
     IcsId: str = None
     TopMostParentId: str = None
     Direction: str = None
     Towards: str = None
-    Modes: list[str]
+    Modes: list[str] = []
     StopType: str = None
     StopLetter: str = None
     Zone: str = None
     AccessibilitySummary: str = None
     HasDisruption: bool = None
-    Lines: list["IdentifierModel"]
+    Lines: list["IdentifierModel"] = []
     Status: bool = None
     Id: str = None
     Url: str = None
     Name: str = None
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Line')
@@ -486,17 +486,17 @@
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     LineId: str = None
     LineName: str = None
     Direction: str = None
     BranchId: int = None
-    NextBranchIds: list[int]
-    PrevBranchIds: list[int]
-    StopPoint: list["MatchedStopModel"]
+    NextBranchIds: list[int] = []
+    PrevBranchIds: list[int] = []
+    StopPoint: list["MatchedStopModel"] = []
     ServiceType: str = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-21')
 
 
 StopPointSequenceModel = StopPointSequence
 
@@ -507,15 +507,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Name: str = None
-    NaptanIds: list[str]
+    NaptanIds: list[str] = []
     ServiceType: str = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-22')
 
 
 OrderedRouteModel = OrderedRoute
 
@@ -530,18 +530,18 @@
     )
 
     LineId: str = None
     LineName: str = None
     Direction: str = None
     IsOutboundOnly: bool = None
     Mode: str = None
-    LineStrings: list[str]
-    Stations: list["MatchedStopModel"]
-    StopPointSequences: list["StopPointSequenceModel"]
-    OrderedLineRoutes: list["OrderedRouteModel"]
+    LineStrings: list[str] = []
+    Stations: list["MatchedStopModel"] = []
+    StopPointSequences: list["StopPointSequenceModel"] = []
+    OrderedLineRoutes: list["OrderedRouteModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-23')
 
 
 RouteSequenceModel = RouteSequence
 
 
@@ -593,17 +593,17 @@
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     LineId: str = None
     Mode: str = None
     LineName: str = None
-    LineRouteSection: list["LineRouteSectionModel"]
-    MatchedRouteSections: list["MatchedRouteSectionsModel"]
-    MatchedStops: list["MatchedStopModel"]
+    LineRouteSection: list["LineRouteSectionModel"] = []
+    MatchedRouteSections: list["MatchedRouteSectionsModel"] = []
+    MatchedStops: list["MatchedStopModel"] = []
     Id: str = None
     Url: str = None
     Name: str = None
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-26')
@@ -618,15 +618,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Input: str = None
-    SearchMatches: list["RouteSearchMatchModel"]
+    SearchMatches: list["RouteSearchMatchModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-27')
 
 
 RouteSearchResponseModel = RouteSearchResponse
 
 
@@ -654,15 +654,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Id: str = None
-    Intervals: list["IntervalModel"]
+    Intervals: list["IntervalModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-29')
 
 
 StationIntervalModel = StationInterval
 
 
@@ -747,18 +747,18 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Name: str = None
-    KnownJourneys: list["KnownJourneyModel"]
+    KnownJourneys: list["KnownJourneyModel"] = []
     FirstJourney: KnownJourneyModel = None
     LastJourney: KnownJourneyModel = None
-    Periods: list["PeriodModel"]
+    Periods: list["PeriodModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-34')
 
 
 ScheduleModel = Schedule
 
 
@@ -767,16 +767,16 @@
     Autogenerated from Line::Tfl.Api.Presentation.Entities.TimetableRoute
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    StationIntervals: list["StationIntervalModel"]
-    Schedules: list["ScheduleModel"]
+    StationIntervals: list["StationIntervalModel"] = []
+    Schedules: list["ScheduleModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-35')
 
 
 TimetableRouteModel = TimetableRoute
 
 
@@ -786,15 +786,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     DepartureStopId: str = None
-    Routes: list["TimetableRouteModel"]
+    Routes: list["TimetableRouteModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-36')
 
 
 TimetableModel = Timetable
 
 
@@ -821,15 +821,15 @@
     Autogenerated from Line::Tfl.Api.Presentation.Entities.Timetables.Disambiguation
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    DisambiguationOptions: list["DisambiguationOptionModel"]
+    DisambiguationOptions: list["DisambiguationOptionModel"] = []
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-38')
 
 
 DisambiguationModel = Disambiguation
 
 
@@ -842,16 +842,16 @@
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     LineId: str = None
     LineName: str = None
     Direction: str = None
     PdfUrl: str = None
-    Stations: list["MatchedStopModel"]
-    Stops: list["MatchedStopModel"]
+    Stations: list["MatchedStopModel"] = []
+    Stops: list["MatchedStopModel"] = []
     Timetable: TimetableModel = None
     Disambiguation: DisambiguationModel = None
     StatusErrorMessage: str = None
     _source_schema_name: str = PrivateAttr(default='Line')
     _component_schema_name: str = PrivateAttr(default='Tfl-39')
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Mode.py` & `tubeulator-0.1.0/src/tubeulator/generated/Mode.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Place.py` & `tubeulator-0.1.0/src/tubeulator/generated/Place.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Category: str = None
-    AvailableKeys: list[str]
+    AvailableKeys: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Place')
     _component_schema_name: str = PrivateAttr(default='Tfl')
 
 
 PlaceCategoryModel = PlaceCategory
 
 
@@ -55,17 +55,17 @@
     )
 
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Place')
     _component_schema_name: str = PrivateAttr(default='Tfl-3')
 
 
 PlaceModel = Place
@@ -117,16 +117,16 @@
     Autogenerated from Place::Tfl.Api.Presentation.Entities.Crowding
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    PassengerFlows: list["PassengerFlowModel"]
-    TrainLoadings: list["TrainLoadingModel"]
+    PassengerFlows: list["PassengerFlowModel"] = []
+    TrainLoadings: list["TrainLoadingModel"] = []
     _source_schema_name: str = PrivateAttr(default='Place')
     _component_schema_name: str = PrivateAttr(default='Tfl-6')
 
 
 CrowdingModel = Crowding
 
 
@@ -161,15 +161,15 @@
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanIdReference: str = None
     StationAtcoCode: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Place')
     _component_schema_name: str = PrivateAttr(default='Tfl-8')
 
 
 LineGroupModel = LineGroup
 
 
@@ -179,15 +179,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     ModeName: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='Place')
     _component_schema_name: str = PrivateAttr(default='Tfl-9')
 
 
 LineModeGroupModel = LineModeGroup
 
 
@@ -200,35 +200,35 @@
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanId: str = None
     PlatformName: str = None
     Indicator: str = None
     StopLetter: str = None
-    Modes: list[str]
+    Modes: list[str] = []
     IcsCode: str = None
     SmsCode: str = None
     StopType: str = None
     StationNaptan: str = None
     AccessibilitySummary: str = None
     HubNaptanCode: str = None
-    Lines: list["IdentifierModel"]
-    LineGroup: list["LineGroupModel"]
-    LineModeGroups: list["LineModeGroupModel"]
+    Lines: list["IdentifierModel"] = []
+    LineGroup: list["LineGroupModel"] = []
+    LineModeGroups: list["LineModeGroupModel"] = []
     FullName: str = None
     NaptanMode: str = None
     Status: bool = None
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='Place')
     _component_schema_name: str = PrivateAttr(default='Tfl-10')
 
 
 StopPointModel = StopPoint
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Road.py` & `tubeulator-0.1.0/src/tubeulator/generated/Road.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Name: str = None
     Closure: str = None
     Directions: str = None
-    Segments: list["StreetSegmentModel"]
+    Segments: list["StreetSegmentModel"] = []
     SourceSystemId: int = None
     SourceSystemKey: str = None
     _source_schema_name: str = PrivateAttr(default='Road')
     _component_schema_name: str = PrivateAttr(default='Tfl-3')
 
 
 StreetModel = Street
@@ -125,15 +125,15 @@
     ProjectDescription: str = None
     ProjectPageUrl: str = None
     ConsultationPageUrl: str = None
     ConsultationStartDate: datetime = None
     ConsultationEndDate: datetime = None
     ConstructionStartDate: datetime = None
     ConstructionEndDate: datetime = None
-    BoroughsBenefited: list[str]
+    BoroughsBenefited: list[str] = []
     CycleSuperhighwayId: str = None
     Phase: str = None
     ContactName: str = None
     ContactEmail: str = None
     ExternalPageUrl: str = None
     ProjectSummaryPageUrl: str = None
     _source_schema_name: str = PrivateAttr(default='Road')
@@ -223,35 +223,35 @@
     Severity: str = None
     Ordinal: int = None
     Category: str = None
     SubCategory: str = None
     Comments: str = None
     CurrentUpdate: str = None
     CurrentUpdateDateTime: datetime = None
-    CorridorIds: list[str]
+    CorridorIds: list[str] = []
     StartDateTime: datetime = None
     EndDateTime: datetime = None
     LastModifiedTime: datetime = None
     LevelOfInterest: str = None
     Location: str = None
     Status: str = None
     Geography: DbGeographyModel = None
     Geometry: DbGeographyModel = None
-    Streets: list["StreetModel"]
+    Streets: list["StreetModel"] = []
     IsProvisional: bool = None
     HasClosures: bool = None
     LinkText: str = None
     LinkUrl: str = None
     RoadProject: RoadProjectModel = None
     PublishStartDate: datetime = None
     PublishEndDate: datetime = None
     TimeFrame: str = None
-    RoadDisruptionLines: list["RoadDisruptionLineModel"]
-    RoadDisruptionImpactAreas: list["RoadDisruptionImpactAreaModel"]
-    RecurringSchedules: list["RoadDisruptionScheduleModel"]
+    RoadDisruptionLines: list["RoadDisruptionLineModel"] = []
+    RoadDisruptionImpactAreas: list["RoadDisruptionImpactAreaModel"] = []
+    RecurringSchedules: list["RoadDisruptionScheduleModel"] = []
     _source_schema_name: str = PrivateAttr(default='Road')
     _component_schema_name: str = PrivateAttr(default='Tfl-8')
 
 
 RoadDisruptionModel = RoadDisruption
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Search.py` & `tubeulator-0.1.0/src/tubeulator/generated/Search.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     Query: str = None
     From: int = None
     Page: int = None
     PageSize: int = None
     Provider: str = None
     Total: int = None
-    Matches: list["SearchMatchModel"]
+    Matches: list["SearchMatchModel"] = []
     MaxScore: float = None
     _source_schema_name: str = PrivateAttr(default='Search')
     _component_schema_name: str = PrivateAttr(default='Tfl-2')
 
 
 SearchResponseModel = SearchResponse
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/StopPoint.py` & `tubeulator-0.1.0/src/tubeulator/generated/StopPoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Category: str = None
-    AvailableKeys: list[str]
+    AvailableKeys: list[str] = []
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.StopPointCategory')
 
 
 StopPointCategoryModel = StopPointCategory
 
 
@@ -90,16 +90,16 @@
     Autogenerated from StopPoint::Tfl.Api.Presentation.Entities.Crowding
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    PassengerFlows: list["PassengerFlowModel"]
-    TrainLoadings: list["TrainLoadingModel"]
+    PassengerFlows: list["PassengerFlowModel"] = []
+    TrainLoadings: list["TrainLoadingModel"] = []
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.Crowding')
 
 
 CrowdingModel = Crowding
 
 
@@ -134,15 +134,15 @@
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanIdReference: str = None
     StationAtcoCode: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.LineGroup')
 
 
 LineGroupModel = LineGroup
 
 
@@ -152,15 +152,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     ModeName: str = None
-    LineIdentifier: list[str]
+    LineIdentifier: list[str] = []
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.LineModeGroup')
 
 
 LineModeGroupModel = LineModeGroup
 
 
@@ -195,17 +195,17 @@
     )
 
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.Place')
 
 
 PlaceModel = Place
@@ -220,35 +220,35 @@
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     NaptanId: str = None
     PlatformName: str = None
     Indicator: str = None
     StopLetter: str = None
-    Modes: list[str]
+    Modes: list[str] = []
     IcsCode: str = None
     SmsCode: str = None
     StopType: str = None
     StationNaptan: str = None
     AccessibilitySummary: str = None
     HubNaptanCode: str = None
-    Lines: list["IdentifierModel"]
-    LineGroup: list["LineGroupModel"]
-    LineModeGroups: list["LineModeGroupModel"]
+    Lines: list["IdentifierModel"] = []
+    LineGroup: list["LineGroupModel"] = []
+    LineModeGroups: list["LineModeGroupModel"] = []
     FullName: str = None
     NaptanMode: str = None
     Status: bool = None
     Id: str = None
     Url: str = None
     CommonName: str = None
     Distance: float = None
     PlaceType: str = None
-    AdditionalProperties: list["AdditionalPropertiesModel"]
-    Children: list["PlaceModel"]
-    ChildrenUrls: list[str]
+    AdditionalProperties: list["AdditionalPropertiesModel"] = []
+    Children: list["PlaceModel"] = []
+    ChildrenUrls: list[str] = []
     Lat: float = None
     Lon: float = None
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.StopPoint')
 
 
 StopPointModel = StopPoint
@@ -296,15 +296,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     LineName: str = None
-    LineSpecificServiceTypes: list["LineSpecificServiceTypeModel"]
+    LineSpecificServiceTypes: list["LineSpecificServiceTypeModel"] = []
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.LineServiceType')
 
 
 LineServiceTypeModel = LineServiceType
 
 
@@ -455,16 +455,16 @@
     Autogenerated from StopPoint::Tfl.Api.Presentation.Entities.StopPointsResponse
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
-    CentrePoint: list[float]
-    StopPoints: list["StopPointModel"]
+    CentrePoint: list[float] = []
+    StopPoints: list["StopPointModel"] = []
     PageSize: int = None
     Total: int = None
     Page: int = None
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.StopPointsResponse')
 
 
@@ -503,15 +503,15 @@
 
     Query: str = None
     From: int = None
     Page: int = None
     PageSize: int = None
     Provider: str = None
     Total: int = None
-    Matches: list["SearchMatchModel"]
+    Matches: list["SearchMatchModel"] = []
     MaxScore: float = None
     _source_schema_name: str = PrivateAttr(default='StopPoint')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.SearchResponse')
 
 
 SearchResponseModel = SearchResponse
```

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/Vehicle.py` & `tubeulator-0.1.0/src/tubeulator/generated/Vehicle.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/generated/occupancy.py` & `tubeulator-0.1.0/src/tubeulator/generated/occupancy.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
 
     model_config = ConfigDict(
         alias_generator=AliasGenerator(validation_alias=to_camel_case),
     )
 
     Id: str = None
-    Bays: list["BayModel"]
+    Bays: list["BayModel"] = []
     Name: str = None
     CarParkDetailsUrl: str = None
     _source_schema_name: str = PrivateAttr(default='occupancy')
     _component_schema_name: str = PrivateAttr(default='Tfl.Api.Presentation.Entities.CarParkOccupancy')
 
 
 CarParkOccupancyModel = CarParkOccupancy
```

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/_types.py` & `tubeulator-0.1.0/src/tubeulator/openapi/_types.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/dataclass_generator.py` & `tubeulator-0.1.0/src/tubeulator/openapi/dataclass_generator.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/fetch.py` & `tubeulator-0.1.0/src/tubeulator/openapi/fetch.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/reference.py` & `tubeulator-0.1.0/src/tubeulator/openapi/reference.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/scan.py` & `tubeulator-0.1.0/src/tubeulator/openapi/scan.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/schema/aliased.py` & `tubeulator-0.1.0/src/tubeulator/openapi/schema/aliased.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/openapi/schema/base.py` & `tubeulator-0.1.0/src/tubeulator/openapi/schema/base.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/__init__.py` & `tubeulator-0.1.0/src/tubeulator/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/combine.py` & `tubeulator-0.1.0/src/tubeulator/topology/combine.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/data_model.py` & `tubeulator-0.1.0/src/tubeulator/topology/data_model.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/gtfs_data_model.py` & `tubeulator-0.1.0/src/tubeulator/topology/gtfs_data_model.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/load.py` & `tubeulator-0.1.0/src/tubeulator/topology/load.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/load_gtfs.py` & `tubeulator-0.1.0/src/tubeulator/topology/load_gtfs.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/topology/map.py` & `tubeulator-0.1.0/src/tubeulator/topology/map.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/utils/lcp_trie.py` & `tubeulator-0.1.0/src/tubeulator/utils/lcp_trie.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/utils/logs.py` & `tubeulator-0.1.0/src/tubeulator/utils/logs.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/utils/paths.py` & `tubeulator-0.1.0/src/tubeulator/utils/paths.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/utils/schemas.py` & `tubeulator-0.1.0/src/tubeulator/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/src/tubeulator/utils/string_conv.py` & `tubeulator-0.1.0/src/tubeulator/utils/string_conv.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/tests/topo_combine_test.py` & `tubeulator-0.1.0/tests/topo_combine_test.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/tests/topo_load_test.py` & `tubeulator-0.1.0/tests/topo_load_test.py`

 * *Files identical despite different names*

### Comparing `tubeulator-0.0.9/PKG-INFO` & `tubeulator-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubeulator
-Version: 0.0.9
+Version: 0.1.0
 Summary: TfL open data interface library.
 Author-Email: Louis Maddox <louismmx@gmail.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -28,15 +28,15 @@
 Provides-Extra: polars-lts-cpu
 Description-Content-Type: text/markdown
 
 # tubeulator
 
 > It's time for the tubeulator
 
-TfL open data interface library
+TfL open data interface library.
 
 ## Key features
 
 - Route planning (underground, overground, bus, walking)
 - Time estimation taking into account mixed modes of travel in one journey
 
 ## Requires
```

