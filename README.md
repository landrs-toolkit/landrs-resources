# Development Learning Resources for LANDRS

This repository contains developer related background materials for the Linked And Networked DRoneS
(LANDRS) project. These include Linked Data Development tutorials, links to toolkits used in the LANDRS frameworks development, and links to existing vocabularies and ontologies that will be leveraged in the project development.



## Linked Data Development Background
A very general set of background documents on linked data and linked data technologies is available in the Zazuko Github organization repository [linked-data-training](https://github.com/zazuko/linked-data-training). These materials provide a reasonable starting point to understand the LANDRS development linked-data technology stack.

## Linked Data Frameworks
Toolkits for developing using RDF, Ontologies and linked-data have been developed for many programming languages. The LANDRS project will focus on Python and Javascript technologies and will leverage the following technologies and frameworks.
### Python
*  [RDFLib](https://github.com/RDFLib/rdflib)
*  [PySHACL](https://github.com/RDFLib/pySHACL)
*  [pyLDAPI](https://github.com/RDFLib/pyLDAPI) Linked Data API

### Javascript
*  [RDF-ext library javascript library](https://github.com/rdf-ext/rdf-ext) General RDF Library
*  [RDF-ext](https://github.com/rdf-ext) Toolkits using [RDF JAVASCRIPT LIBRARIES COMMUNITY GROUP
](https://www.w3.org/community/rdfjs/) data model [recommendation](http://rdf.js.org/data-model-spec/). The community group also has a [Github repository](https://github.com/rdfjs) where the model specifications are located.

### Hydra Core Vocabulary
API documentation for LANDRS convenience APIs should use the [Hydra W3C Community Group](https://www.hydra-cg.com/spec/latest/core/) recommendation for A Vocabulary for Hypermedia-Driven Web APIs as a first class citizen. Cross-walks can be provided to other API documentation representations such as [OpenAPI](https://swagger.io/specification/). In serializing of linked API we will preferably use [JSON-LD 1.1](https://www.w3.org/TR/json-ld11/) and [Turtle](https://www.w3.org/TR/turtle/).

### Hydra in the Wild
To facilitate rapid prototyping and development, LANDRS will leverage the following hydra based frameworks to publish the hydra apiDocumentation specification.
* [hydra-box](https://github.com/zazuko/hydra-box) for creating Hydra Core based api endpoints
* [Alcaeus](https://github.com/wikibus/Alcaeus) Promise-based library for consuming Hydra APIs
* [hypermedia-app](https://github.com/hypermedia-app) Javascript libraries for hydra based web development.

Examples of these technologies in action include.
* [Wikibus](https://github.com/wikibus/sources.wikibus.org) as a hydra-box demonstrator endpoint for public transportation using linked data technologies.
* [Backend for Zurich Municipal Linked Statistical Data](https://github.com/StatistikStadtZuerich/stat.stadt-zuerich.ch)

The Apache Jena Project maintains an open source triple store the has recently integrated SHACL and GeoSPARQL support. Note the geosparql-jena extensions have been integrated in the main Jena repository but still provide some useful documentation.
* [Apache Jena Set of Frameworks](https://jena.apache.org/)
* [Apache Jena Fuseki](https://jena.apache.org/documentation/fuseki2/index.html)
* [Jena Geosparql Github Repo](https://github.com/galbiston/geosparql-jena)
* [Geosparql-Fuseki](https://github.com/galbiston/geosparql-fuseki)

We use [Zazuko Trifid](https://github.com/zazuko/trifid) as a linked data server and proxy for the Fuseki triple store. Additionally Trifid has the [Yasgui](https://github.com/TriplyDB/YASGUI) SPARQL query editor integrated into it's web interface. Vocabularies and ontologies are developed using [Zazuko Ontology Manager](https://zazuko.com/products/ontology-manager/).

## Existing Vocabularies and Ontologies
* [W3C Semantic Sensor Network (SOSA)](https://www.w3.org/TR/vocab-ssn/)
* [W3C Semantic Sensor Network Extensions (SOSA-EXT)](https://w3c.github.io/sdw/proposals/ssn-extensions/)
* [Projects using SOSA](https://w3c.github.io/sdw/ssn-usage/)
* [OWL-Time](https://www.w3.org/TR/owl-time/)
* [OWL-Time Extensions](https://rawgit.com/w3c/sdw/time-entity-relations/proposals/time-entity-relations/index.html)
* [WoT Thing Description](https://www.w3.org/TR/wot-thing-description/)
* [Schema.org](https://schema.org)
* [DCAT version 2](https://www.w3.org/TR/vocab-dcat-2/)
* [DCAT Profiles](https://w3c.github.io/dxwg/profiles/)
* [GeoSPARQL](https://www.opengeospatial.org/standards/geosparql)
* [W3C Decentralized Identifiers Primer](https://w3c-ccg.github.io/did-primer/)
* [W3C Decentralized Identifiers Core Spec](https://www.w3.org/TR/2019/WD-did-core-20191107/)

### Non-Standards Body Ontology Work
* [Semantic Trajectory Episodes](https://talespaiva.github.io/step/)
* [VSSo: a Vehicle Signals and Attribute Ontology](https://github.com/klotzbenjamin/vss-ontology)
* [W3C Automotive Business Group VSSo Draft](http://automotive.eurecom.fr/vsso)
* [USGS Geographic Information Name Serviec (GNIS-LD)](https://gnis-ld.org/)

### Related Best Practices
* [Spatial Data on the Web Best Practices](https://www.w3.org/TR/sdw-bp/)
* [Data on the Web Best Practices](https://www.w3.org/TR/dwbp/)
* [OGC API - Features - Part 1: Core](http://docs.opengeospatial.org/DRAFTS/17-069r1.html)
* [Second Environmental Linked Features Experiment](https://github.com/opengeospatial/SELFIE)
* [OGC Sensorthings API Documentation](https://developers.sensorup.com/docs/#introduction)
* [Science On Schema.org](https://github.com/ESIPFed/science-on-schema.org)
* [Vehicle Information Service Specification](https://www.w3.org/TR/vehicle-information-service/)

## How we develop
* Test-driven development
* User stories
* Web Frameworks
* API specification
* OGC standards for spatial data
* W3C standards for linked-data and web development

## Relevant References
* [GNIS-LD: Serving and Visualizing the Geographic Names Information System Gazetteer As Linked Data](http://geog.ucsb.edu/~regalia/paper/eswc2018.pdf)
* [GeoSPARQL-Jena: Implementation and Benchmarking of a GeoSPARQL Graphstore](http://www.semantic-web-journal.net/system/files/swj2108.pdf)

## Blogs releated to developing linked data applications
* [Shaping Linked Data apps](https://ruben.verborgh.org/blog/2019/06/17/shaping-linked-data-apps/)
* [Piecing the puzzle: Self-publishing queryable research data on the Web](https://ruben.verborgh.org/articles/queryable-research-data)
* [Linked Data Shapes, Forms and Footprints -- TBL](https://www.w3.org/DesignIssues/Footprints.html)
* [The Semantic Web identity crisis: in search of the trivialities that never were](https://ruben.verborgh.org/articles/the-semantic-web-identity-crisis/)
* [Paradigm shifts for the decentralized Web As separate markets for data and apps emerge, Web development needs to adopt a new shape](https://ruben.verborgh.org/blog/2017/12/20/paradigm-shifts-for-the-decentralized-web)
* [Designing a Linked Data developer experience Making decentralized Web app development fun](https://ruben.verborgh.org/blog/2018/12/28/designing-a-linked-data-developer-experience/)