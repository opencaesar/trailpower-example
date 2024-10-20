# Trailpower Example

[![CI](https://github.com/opencaesar/trailpower-example/actions/workflows/ci.yml/badge.svg)](https://github.com/opencaesar/trailpower-example/actions/workflows/ci.yml)
[![Pages](https://img.shields.io/badge/Pages-HTML-blue)](http://opencaesar.github.io/trailpower-example/) 
[![Gitpod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/opencaesar/trailpower-example) 

This is a description of the Trail Power system in [OML](https://github.com/opencaesar/oml) using the Sierra method.

## Clone
```
  git clone https://github.com/opencaesar/trailpower-example.git
  cd trailpower-example
```

## Build
Check the consistency of the dataset
```
./gradlew build
```

## Start Fuseki Server
Start the Fuseki triple store
```
./gradlew startFuseki
```
Navigate to http://localhost:3030

Verify you see two datasets: `trailpower.inf` and `trailpower.tdb`

## Stop Fuseki Server
Stop the Fuseki triple store
```
./gradlew stopFuseki
```

## Load Dataset to Fuseki
Load the dataset to Fuseki server
```
./gradlew load
```
Navigate to http://localhost:3030/#/dataset/trailpower.inf/info

Click on `count triples in all graphs` and observe the triple counts

Navigate to http://localhost:3030/#/dataset/trailpower.tdb/info

Click on `count triples in all graphs` and observe the triple counts

## Run Queries
Run the queries at `src/sparql/opencaesar.io/trailpower`

```
./gradlew query
```
Inspect the results at `build/results/trailpower`

## Save Dataset from Fuseki
Assuming you have updated the `trailpower` dataset in Fuseki
```
./gradlew save
```
Find the updates in the `src/oml/opencaesar.io/trailpower` folder

## Publish to Maven Local
Publish the OML dataset as an archive in the local maven repo
```
./gradlew publishToMavenLocal
```
Inspect the OML archive
```
ls ~/.m2/repository/io/opencaesar/trailpower
```