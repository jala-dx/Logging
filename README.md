# Goals
There are a few problems with the current state of logging.  The first is that there is no real unified or agreed upon standard for how to do logging, across software platforms, so it is typically left up to the software designer to choose how to design and output logs.  Because of this non standardized approach, there are many many different formats that logs can become.  Obviously this is an issue if you are attempting to gather useful and meaningful data from a variety of different sources.  Because of this large number of log types and formats, numerous logging tools have been created, all trying to solve a certain type of logging problem, and so selecting one tool that offers everything can quickly become a chore.  The other big problem is that logs can produce an overwhelming amount of information.  Many of the traditional tools do nothing to correlate and represent the data that they collect.  Therefore, narrowing down specific issues can also become very difficult.


# Proposed Logging Architecture
  Log Producers
  Collector 
  Normalizer
  Indexer
  Query
  Optional presentation layer

<p align="center">
  <img src="Untitled%20Diagram.png" />
</p>

# Atom Log lifecycle
  Generation
  Collection
  Indexing
  Retention
  
# 3rdparty product logs lifecycle
Generation
Collection
Normalization
Indexing
Retention

# Instance of our architecture with Filebeat/ELK

# Security

# Reliability with failure cases and mitigation.
