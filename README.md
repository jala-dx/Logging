h1. ATOM Structured Logging

Goals/Problem statement

* There are a few problems with the current state of logging.  You have different Applications/Containers/VMs feeding into each other. Debugging an issue requires logging into each individual box to look at the logs. With small number of apps/boxes it's not an issue, but it quickly becomes tedious as the number of apps/boxes increase!

Proposed Solution:
* It would be awesome to have all of your logs aggregated into one place so you can see the process flow and perform queries against the logs from all applications from one place.

** Enter EFK stack ..

What does EFK stands for:
* Elasticsearch: Elasticsearch is a search server based on Lucene. It provides a distributed, multitenant-capable full-text search engine with a RESTful web interface and schema-free JSON documents.

* Filebeat is a log data shipper for local files. Installed as an agent on your servers, Filebeat monitors the log directories or specific log files, tails the files, and forwards them either to Elasticsearch or Logstash for indexing.

* Kibana: A nifty tool to visualize logs and timestamped data.


h2. Proposed Logging Architecture via EFK

<p align="center">
  <img src="Untitled%20Diagram.png" />
</p>

** Log Producer
** Collector 
** Normalizer
** Indexer
** Query
** Optional presentation layer


h2. Atom Log lifecycle
  Generation
  Collection
  Indexing
  Retention
  
h2. 3rdparty product logs lifecycle
Generation
Collection
Normalization
Indexing
Retention

h2. Instance of our architecture with Filebeat/ELK

h2. Security

h2. Reliability with failure cases and mitigation.
