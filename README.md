iibench-mongodb
===============

iiBench Benchmark for MongoDB and TokuMX


Requirements
=====================

* Java 1.6 or 1.7 or 1.8
* currently 3.1.1 driver is in the repo and is included by the run.simple.bash script

* This example assumes that you already have a MongoDB server running on the same machine as the iiBench client application.
* You can connect a different server or port by editing the run.simple.bash script. 


Running the benchmark
=====================

In the default configuration the benchmark will run a single insert thread for 1 hour, or 100 million inserts, whichever comes first.

```bash
git clone https://github.com/tmcallaghan/iibench-mongodb.git
cd iibench-mongodb

```

*[optionally edit run.simple.bash to modify the benchmark behavior]*

```bash
./run.simple.bash

```

Things to vary would be NUM_LOADER_THREADS, QUERIES_PER_INTERVAL to add querying to insert workload (default, 0 queries), etc.
