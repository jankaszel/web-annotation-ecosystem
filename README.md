# The Web Annotation Ecosystem: A Curation of Apps & Tools

Annotating sources is a common practice in science and beyond. The Web Annotation specification consists of both a [data model](https://www.w3.org/TR/annotation-model/) and an [HTTP-based protocol](https://www.w3.org/TR/annotation-protocol/) that describe how annotations can be modeled and exchanged on the web.

Others have curated annotation tools before—[such as this curation](https://github.com/taivop/awesome-data-annotation)—but services commonly don't share data among each other. The Web Annotation specification, however, was designed with interoperability between services in mind and can realize storage decoupling, similar to what the [Solid project](https://solidproject.org) does with _pods_ and Linked Data.

Little effort has been made to actually document interoperability between such services: Can I store annotations made with an annotation editor onto my own annotation server? Will annotations made with a particular editor be visible in a separate annotation viewer? The Web Annotation specification is flexible and extensible, but leaves us with uncertainty about which software will support which features of the data model.

This repository aims to shed light into this question of compatibility by documenting services that adhere to the Web Annotation specification. By stating which parts of the specification are supported, interested parties can ideally estimate which tools will be compatible with each other.

This is a living document with no claim of completeness. If you want to add services, please [feel free to contribute](#contributing). This document is licensed under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).

### Contributing

Contributions to this curation are welcome. In order to contribute, please raise a PR with your changes to this document.

## Annotation Viewers

## Annotation Editors

* [dokieli](https://github.com/linkeddata/dokieli): dokieli is a clientside editor for decentralised article publishing, annotations and social interactions.
* [Recogito](https://recogito.pelagios.org): A semantic annotation tool for texts and images, developed by [the Pelagios project](http://commons.pelagios.org). Recogito allows to annotate resources such as IIIF collections and TEI documents with text, persons, or places and can export JSON-LD data among other formats.

## Annotation Servers

* [Simple Annotation Server](https://github.com/falafeljan/simple-annotation-server): A simple annotation server written in JavaScript for the Node.js runtime. This server aims to closely adhere to the Web Annotation specification, serving as a possible reference implementation for both development and personal use.

## Annotation Libraries

* [Annotorious](https://recogito.github.io/annotorious/): Annotorious builds upon the internals of [RecogitoJS](https://github.com/recogito/recogito-js) and enables image annotation on the web. With the respective plugin, Annotious can be used with [OpenSeadragon](https://openseadragon.github.io) for annotating high-resolution, zoomable images.
* [Apache Annotator](https://github.com/apache/incubator-annotator): A library that provides annotation enabling code for browsers, servers, and humans. Written in TypeScript. Most notably, Apache Annotator provides functionality for creating and resolving Web Annotation selectors in DOM environments.
* [RecogitoJS](https://github.com/recogito/recogito-js): A modular UI component for annotating text on the web, RecogitoJS comes as an all-in-one solution for adding annotation capabilities and is extensible via themes and plugins.

## Annotation Tools

* [`validate-web-annotation`](https://github.com/falafeljan/validate-web-annotation): Validate JSON object against the Web Annotation Data Model using JSON schemata.
* [W3C Web Annotation Tests](https://github.com/w3c/web-annotation-tests): A suite of tests for validating the Web Annotation family of specifications. This suite is going to be included in the [W3C's Web Platform Tests infrastructure](https://github.com/web-platform-tests/wpt) and covers both the Annotation Model and Annotation Protocol.

