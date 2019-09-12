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

* Then build the other docker containers
```bash
docker-compose up
```

## Links
* Polkascan Explorer GUI: http://127.0.0.1:8080
* Harvester task monitor: http://127.0.0.1:5555
* Harvester progress: http://127.0.0.1:8080/harvester/admin
