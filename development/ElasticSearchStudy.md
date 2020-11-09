# ElasticSearch

Elasticsearch 是一个分布搜索, 分析引擎

## Search

```bash
curl -X GET "localhost:9200/_search?pretty" -H 'Content-Type: application/json' -d'
{
  "query": { 
    "bool": { 
      "must": [
        { "match": { "title":   "Search"        }},
        { "match": { "content": "Elasticsearch" }}
      ],
      "filter": [ 
        { "term":  { "status": "published" }},
        { "range": { "publish_date": { "gte": "2015-01-01" }}}
      ]
    }
  }
}
'

```

### Context
* Query: query, 返回结果包含socre(表示result跟query的匹配程度)
* Filter: filter, 返回结果不包含socre

### Boolean query

bool 包含如下字句, bool的字句间关系是and, 必须都满足才返回结果

* must: 必须包含, 在query上下文
* filter: 必须包含, 在filter上下文, 结果会被缓存
* should: or
* must_not: 必须不包含

## Reference
* [search-your-data](https://www.elastic.co/guide/en/elasticsearch/reference/7.x/search-your-data.html)
* [query-dsl](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl.html)
* [search-api](https://www.elastic.co/guide/en/elasticsearch/reference/7.x/search-search.html)
