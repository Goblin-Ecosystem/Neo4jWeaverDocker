# Goblin dataset and weaver docker

This directory allows you to set up the [Maven Central Neo4j database](https://zenodo.org/records/11104819) and the [Weaver API](https://github.com/Goblin-Ecosystem/goblinWeaver) easily using Docker.

⚠️ If you wish to use the Maven database already containing the pre-calculated metrics, set the branch to “metrics_dataset”.

## Fisrt launch
To run it for the first time, use the command:
```
docker-compose up --build
```

On first launch, Docker will download the database dump, which may take some time.

## Second launch
To run it after the first time, use the command:
```
docker-compose up
```

The data is thus persistent.

## Accessibility

**Neo4j user**: neo4j

**Neo4j password**: Password1

- **Neo4j** will be accessible via http://localhost:7474 (web interface).
- **Weaver REST API** will be accessible via http://localhost:8080.
- **Weaver documentation** will be accessible via http://localhost:8080/swagger-ui/index.html