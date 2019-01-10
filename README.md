# Lusail: A System for Querying Linked Data at Scale


The RDF data model allows publishing interlinked RDF datasets, where each dataset is independently maintained and is queryable via a SPARQL endpoint. Many applications would  benefit from querying the resulting large, decentralized, geo-distributed graph through a federated SPARQL query processor. A crucial factor for good  performance in federated query processing is pushing as much computation as possible to the local endpoints. Surprisingly, existing federated SPARQL engines are not effective at this task since they rely only on schema information. Consequently, they cause unnecessary data retrieval and communication, leading to poor scalability and response time. This paper addresses these limitations and presents Lusail, a scalable and efficient federated SPARQL system for querying large RDF graphs that are geo-distributed on different endpoints. Lusail uses a novel query rewriting algorithm to push computation to the local endpoints by relying on information about the RDF instances and not only the schema. The query rewriting algorithm has the additional advantage of exposing parallelism in query processing, which Lusail exploits through advanced scheduling at query run time. Our experiments on billions of triples of real and synthetic data show that Lusail outperforms state-of-the-art systems by orders of magnitude in terms of scalability and response time.

* [**Why do I need Lusail?**](docs/why_lusail.md) We show the limitations of existing systems to query geo-distributed graphs.

* [**Design Rationale**](docs/design_rationale.md) A brief explanation of the system architecture and 
design rationale.

* [**Quick Start**](docs/quick_start.md) A guide to setup Lusail and start running some queries.

* [**FAQ**](docs/faq.md) Collection of frequent questions

* **Publications**
  -  I. Abdelaziz, E. Mansour, M. Ouzzani, A. Aboulnaga and P. Kalnis. [*"Lusail: a system for querying linked data at scale"*](http://www.vldb.org/pvldb/vol11/p485-abdelaziz.pdf), VLDB 2017
  - I. Abdelaziz, E. Mansour, M. Ouzzani, A. Aboulnaga and P. Kalnis, [*"Query Optimizations over Decentralized RDF Graphs"*](https://ieeexplore.ieee.org/document/7929955), ICDE, 2017 (Short paper)
  - E. Mansour, I. Abdelaziz, M. Ouzzani, A. Aboulnaga and P. Kalnis, [*"A demonstration of Lusail: Querying linked data at scale"*](https://dl.acm.org/citation.cfm?id=3058731), SIGMOD, 2017 (Demo)
