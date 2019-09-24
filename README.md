# Polkascan PRE
Polkascan PRE Main Application

## Run application

* Make sure to also clone submodules within the cloned directory: 
```bash
git submodule update --init --recursive
```

* or: Update submodules
```
git submodule update --remote --recursive
```

* During the first run let MySQL initialize (wait for about a minute)

```bash
docker-compose up -d mysql
```

* database create and migrate

```bash
docker-compose up harvester-api
Ctrl+C
```

* Then build the other docker containers
```bash
docker-compose up --build
```

* Alexander test network
```bash
docker-compose -p alexander -f docker-compose.alexander.yml up --build
```

## Links
* Polkascan Explorer GUI: http://127.0.0.1:8080
* Harvester task monitor: http://127.0.0.1:5555
* Harvester progress: http://127.0.0.1:8080/harvester/admin
