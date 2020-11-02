# cognitivoai data engineering test

- I used a docker-compose.yaml to run pyspark local, but this pipeline could easilly run at EMR using its notebook, or you can run as a pipeline using EMR cluster steps (bute code type should be script).

- To run the project you must have docker-compose installed on your machine, then just run `docker-compose up` on the project origin.

- The file format chosen was parquet. Parquet was designed to have more efficient column storage than the CSV itself, the final data scanned is really reduced even comparing with a compressed CSV (GZIP).

- I chosen to change columns before deduplicate the dataset. Because the field update_date should me timestamp before deduplicate.

- I noticed that email and name are switched.

Any doubts? Open a github issue or email me - I will be happy to answer you shortly!
