# ElasticSearch

## installation guide

https://www.elastic.co/search-labs/tutorials/search-tutorial/starter-project

https://www.elastic.co/search-labs/tutorials/install-elasticsearch/docker

### 1.Docker installtion (Local)

```bash
docker run -p 127.0.0.1:9200:9200 -d --name elasticsearch \
  -e "discovery.type=single-node" \
  -e "xpack.security.enabled=false" \
  -e "xpack.license.self_generated.type=trial" \
  -v "elasticsearch-data:/usr/share/elasticsearch/data" \
  docker.elastic.co/elasticsearch/elasticsearch:8.15.0
```

test on `http://localhost:9200`

check after installation

```bash
docker ps -a
```

### 2.Create Virtual environment

```bash
python3 -m venv elastic_search


source elastic_search/bin/activate

```

### 3. Create an index (in elasticsearch with the python client)

```bash
python -m jupyter notebook
```

index is a colletion of document
