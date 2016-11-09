# Introduction to The Elastic Stack

## What is Elasticsearch
* A near-real-time application for quickly indexing and searching 'documents'
* Horizontally scales using Nodes in Clusters to adapt to huge data loads
* Document content stored in an 'inverted index' to allow for hugely fast 'aggregations', 'filters', and other analytics operations
![inverted index](InvertedIndex.png)
* In addition to the inverted index, it stores the _source data as a JSON object for fast recall - no 'hydration' required - you get the whole thing
* Lucene under the hood
* First built as a more approachable version of Lucene by Shay Bannon to search recipes
* Now a full-fledged company still focused on open source but also offering Enterprise Support

## Things I like
* REST for all the things (seriously)
* Use with any language because HTTP (Yay!)
* Dev kits for most languages (see Language Packs below)
* REALLY easy to get up and running (test use cases make it even easier)
* Use it most anywhere in the stack
* Really powerful and easy to extend / customize
* Open source from the start
* The Docs are pretty comprehensive

## Notable Features for Analysis
* Full text search
* Text analysis (grammar, root word, pluralization, etc)
* "More Like This" Term Frequency Analyzers
* Advanced Queries with operators (fuzzy search, etc)



## Why Use Elasticsearch
* You know, for search!
* Logging (big use case)
* "Big Data" (or, pretty big data)
* Rapid filtering / counts / aggregation of data
* Supplement existing big data / activity logging (Kafka) applications
* Percolation / Alerting
* Data Visualization w/ Kibana

## Language Packs:
Python (High Level, Official): https://github.com/elastic/elasticsearch-dsl-py
Python (Low Level, Official): https://github.com/elastic/elasticsearch-py
Go (Community): https://olivere.github.io/elastic/
Clojure your thing?: http://clojureelasticsearch.info/
Java: https://www.elastic.co/guide/en/elasticsearch/client/java-api/current/client.html
JavaScript: https://www.elastic.co/guide/en/elasticsearch/client/javascript-api/current/index.html

## The Hard Bits
* Starting is easy, maturing is hard
* A good deal of gotchas and lots of best practices - this is getting better with time but still will take some time to mature a solution
* Using the API is straightforward. Getting your data ready and thinking about structure is hard


## Let's get cracking

Installation Instructions:

* Download your Apps (Elasticsearch + Kibana recommended, Logstash great for ingest):
https://www.elastic.co/products

* Install the X-Pack if you'd like and/or want to see what is offered for Enterprise

* If you'd like to ingest your own data sets, use Logstash

* Because it's the season, we'll work with the FEC example that is handily provided by Elastic: https://github.com/elastic/examples/tree/master/ElasticStack_usfec

* I've done this for you already! Hooray! (INSERT GH URL)

