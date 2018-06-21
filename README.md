# ES-GUNPACK

Golang client that monitors one or multiple Elasticsearch indices and
1. Finds unparsed in ES-documents with binary data
2. Unpacks the data to JSON
3. Updates the documents with unpacked data



## Todos 
* Parse protobuf signal based on signal name
* Add JSON after parse
* Indicies as CLI arguments
* Password/user as optional input argument

## Done
* ~~Restructure project according to cli/pkg~~
* ~~Find a way of updating matched documents~~
* ~~Get data from Elasticsearch~~
* ~~Command line interface~~
* ~~Unmarshall Elasticsearch document to golang map~~
* ~~Update document with "parsed tag"~~


## Sprints
| Sprint # |                  Target                  |  Time (Actual)  |
|----------|------------------------------------------|-----------------|
|        4 | Restructure project according to cli/pkg | 45 (37)         |
|        3 | Update documents based on ID             | 45 (71)         |
|        2 | Unmarshall json, ~~add parsed tag~~      | 45 (82)         |
|        1 | Use Elasticsearch client, retrieve data  | 45 (50)         |
|          |                                          | **Total**: 2h23 |

##
* Elasticsearch in general
    - https://www.elastic.co/blog/found-optimizing-elasticsearch-searches - Query vs Filter
    - https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html - BoolQuery, Must, Must_not
* elasticsearch client
    - https://godoc.org/github.com/olivere/elastic
    - https://github.com/olivere/elastic/wiki
* cli refererence - https://github.com/urfave/cli#generated-help-text
* Go best practices
    - [Peter Bourgon - Best practices 2016](https://peter.bourgon.org/go-best-practices-2016/#dependency-management)
    - [Template for repository structure](https://github.com/thockin/go-build-template)