# Awesome International Image Interoperability Framework (IIIF) [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="https://upload.wikimedia.org/wikipedia/commons/e/e8/International_Image_Interoperability_Framework_logo.png" align="right" width="100">](https://iiif.io/)

A list of lists of awesome [IIIF](https://iiif.io/) resources.

The International Image Interoperability Framework (IIIF - "triple-eye-eff") is a group of standard APIs around sharing and reuse of media. It is also a growing community of galleries, libraries, archives, museums, companies, and others who develop the standards and interoperable software implementations. Content includes helpful links around each of the standards, demonstrations of their use, and tutorials and presentations. The list is especially helpful for orienting new community members and developers.

[![Contributing Guidelines](http://img.shields.io/badge/CONTRIBUTING-Guidelines-blue.svg)](./contributing.md)

## More Resources

The lists below are a great place to start for inspiration and tooling, but they are certainly not complete!

If you have a link or a resource to add, you have a few options: 
- check out the [Contributing Guidelines](./contributing.md) linked just above and submit a pull request yourself if you're familiar with Github worflows
- [open a new issue ticket](https://github.com/IIIF/awesome-iiif/issues/new) mentioning the link or resource you want to add and some description, and the community may be able to help add it

Likewise, there are other ways to see how people are implementing IIIF.
- [Github Topics page](https://github.com/topics/iiif?o=desc&s=updated) - This page will show you the Github repositories that self-identify as IIIF-related, with the most recently updated projects listed first. 
- [IIIF Community on Zenodo](https://zenodo.org/communities/iiif/) - A Zenodo community for gathering articles and data related to IIIF.

**Disclaimer**: The lists below are presented in alphabetical order within each section, and do not suggest any recommendation. Likewise, these lists are created for informational purposes only and any links do not constitute an endorsement, recommendation, or favoring by the IIIF Consortium.

## Contents
- [Standards](#standards)
- [Official Resources](#official-resources)
- [Image Servers](#image-servers)
- [Image Server Shims](#image-server-shims)
- [Image Viewers](#image-viewers)
- [Image API Libraries](#image-api-libraries)
- [Image Tools](#image-tools)
- [Presentation API Libraries](#presentation-api-libraries)
- [Presentation API Shims](#presentation-api-shims)
- [Presentation Manifest Tools](#presentation-manifest-tools)
- [Validators](#validators)
- [Exhibition and Guided Viewing Tools](#exhibition-and-guided-viewing-tools)
- [Content Search API Servers](#content-search-api)
- [Authentication](#authentication)
- [Tutorials](#tutorials)
- [Videos and Slide Decks](#videos-and-slide-decks)
- [Discovery](#discovery)
- [Annotations](#annotations)
- [CMS Integration](#cms-integration)
- [Newspapers](#newspapers)
- [STEM](#stem)
- [Experiments and Fun](#experiments-and-fun)
- [Community](#community)
- [Digital Asset Management (DAMs)](#digital-asset-management-dams-that-support-iiif)

## Standards

The IIIF community has developed [several standards](https://iiif.io/api/) for interoperable web-based image delivery.

- [Image API](https://iiif.io/api/image/) - Specifies a web service that returns an image in response to a standard HTTP or HTTPS request.
- [Presentation API](https://iiif.io/api/presentation/) - Provides the information necessary to allow a rich, online viewing environment for primarily image-based objects to be presented to a human user, likely in conjunction with the IIIF Image API.
- [Authentication API](https://iiif.io/api/auth/) - Describes a set of workflows for guiding the user through an existing access control system.
- [Change Discovery API](https://iiif.io/api/discovery/) -  This specification describes changes to IIIF content resources and the location of those resources for providers to harvest, to ultimately allow users to easily find and engage with content available via existing IIIF APIs.
- [Content Search API](https://iiif.io/api/search/) - Specifies interoperability mechanism for searching within annotations.
- [External Services API Annex](https://iiif.io/api/annex/services/) - Describes the set of related services that have been identified as useful to reference from the IIIF APIs.
- [API Annex Documents](https://iiif.io/api/annex/) - List of all API annex documents and API implementation notes.

There are also draft specifications, works-in-progress that benefit from community feedback as they're being developed:
- [Content State API](https://iiif.io/api/content-state/) - This specification provides the format of the content state (a IIIF Presentation API resource, or a part of a resource), and mechanisms for passing it between applications regardless of their different user interfaces and capabilities.

## Additional Lists

- [Implementations](https://github.com/IIIF/awesome-iiif/blob/master/implementations.md)
- [Reading and Viewing](https://github.com/IIIF/awesome-iiif/blob/master/reading-viewing.md)

## Official Resources

The [IIIF Consortium (IIIF-C)](https://iiif.io/community/consortium/), with support from the community, maintains a number of resources to assist with understanding and implementation of IIIF.

- [IIIF Cookbook](https://iiif.io/api/cookbook/) - A collection of IIIF "recipes," different reusable code snippets to help create IIIF manifests for common use cases.
- [IIIF Online Workshop](https://training.iiif.io/iiif-online-workshop/) - IIIF workshop materials and videos given by the IIIF-C and updated at each occurrence.
- [IIIF Guides](https://guides.iiif.io/) - A "how-to" resource with screenshots for finding IIIF Manifest URLs from various members of the IIIF community.
- [Image API validator](https://iiif.io/api/image/validator/) - A service to validate a IIIF Image API resource against the specification.
- [Presentation API validator](https://iiif.io/api/presentation/validator/service/) - A service to validate a IIIF Presentation API resource against the specification.

## Image Servers

These servers support the IIIF Image API. Some may also have support for the Presentation API.

- [aws-batch-iiif-generator](https://github.com/vt-digital-libraries-platform/aws-batch-iiif-generator) - An automated pipeline to generate IIIF tiles and manifests and use AWS S3 as an IIIF image server.
- [Cantaloupe](https://cantaloupe-project.github.io/) - Image server written in Java fully conformant to all IIIF Image API versions through 3.0.
- [digilib](https://robcast.github.io/digilib/) - Image server written in Java.
- [FSI Server](https://www.neptunelabs.com/fsi-server/) - FSI Server is a popular commercial solution for serving high resolution images in multiple formats.  It accompanies the Flash-based FSI Viewer for zoom and pan. [IIIF adaptor for FSI server](https://github.com/jhu-digital-manuscripts/rosa/tree/master/rosa-iiif-endpoint)
- [go-iiif](https://github.com/thisisaaronland/go-iiif) - IIIF server written in go (fork of [greut/iiif](https://github.com/greut/iiif)).
- [Hymir IIIF Server](https://github.com/dbmdz/iiif-server-hymir) - IIIF server written in Java supporting IIIF Image and Presentation API.
- [iiif_s3](https://github.com/cmoa/iiif_s3) - Ruby library for generating a static IIIF level 0 Image and Presentation API server on Amazon S3.
- [IIPImage Server](http://iipimage.sourceforge.net/documentation/server/) - High performance image server.
- [Loris](https://github.com/loris-imageserver/loris) - Written in Python.
- [Micrio](https://micr.io/iiif) - Commercial platform for hosting IIIF collections with Presentation API support.
- [RAIS](https://github.com/uoregon-libraries/rais-image-server) - 100% open source tile server for JP2 images written in Go.
- [riiif](https://github.com/curationexperts/riiif) - Written in Ruby as a Rails engine.
- [serverless-iiif](https://github.com/nulib/serverless-iiif) - IIIF Image API 2.1 server as an AWS Serverless Application.
- [SIPI](https://github.com/dasch-swiss/sipi) - IIIFv3 image server written in C++.
- [TremendousIIIF](https://github.com/britishlibrary/TremendousIIIF) - A .NET C# IIIF Image API 2.1 server


## Shim Image Servers 

As defined by Wikipedia a shim is a small library that transparently intercepts an API, changing the parameters passed, handling the operation itself, or redirecting the operation elsewhere. These shims allow you to use an image server that does not currently support IIIF. If you have not implemented an image server yet, this is probably not where you want to start. 

- [ContentDM Image translator](https://github.com/azaroth42/pi3f/tree/master/shims/ContentDM) - Makes ContentDM images available through IIIF. Python.
- [Djatoka Ruby gem](https://github.com/jronallo/djatoka) - Convert IIIF URLs into the URLs that Djatoka requires.
- [Flask-IIIF](https://github.com/inveniosoftware/flask-iiif) - Flask extension to support IIIF in Python/Flask applications. See [Flask-IIIF previewer demo](http://flask-iiif.herokuapp.com/previewer) and [Flask-IIIF RESTful demo](http://flask-iiif.herokuapp.com/restful).
- [Shimmy](https://github.com/mejackreed/shimmy) - Ruby gem designed to help you build shims for the IIIF Presentation API.

## Image Viewers
- [CanvasPanel](http://canvas-panel.netlify.com/) - React library to build IIIF Presentation 3 level viewing experiences including support for annotations.
- [Diva.js](https://ddmal.github.io/diva.js/) - IIIF image viewer optimized for speed and flexibility.
- [IIIF Curation Viewer](http://codh.rois.ac.jp/software/iiif-curation-viewer/) - A general IIIF viewer with added focus on curation and ordering of cropped IIIF images. [Demo](http://codh.rois.ac.jp/software/iiif-curation-viewer/demo/?curation=https://gist.githubusercontent.com/2SC1815J/18e1228c52a6650c64902142ed7496f8/raw/7a247b64b6e22357e83f573b7283e31f3111af68/curation_kibutsu.json&pos=4)
- [IIIFViewer](https://github.com/klokantech/iiifviewer) - IIIF WebGL / Canvas / DOM mobile-ready fast viewer powered by OpenLayers V3.
  - [Imaging Helper Plugin](https://github.com/msalsbery/OpenSeadragonImagingHelper) - OpenSeadragon plugin with utility functions.
- [Internet Archive BookReader](https://github.com/internetarchive/bookreader) - A viewer developed by the Internet Archive, specially suited for viewing books.
- [IIPMooViewer](https://iipimage.sourceforge.io/documentation/iipmooviewer/) - IIPMooViewer is an open source, Javascript and HTML5 image streaming and zooming client. IIPMooViewer is IIIF-compatible and works with IIPServer or other IIIF compatible servers. [Demo](https://iipimage.sourceforge.io/demo/)
- [Leaflet-IIIF](https://github.com/mejackreed/Leaflet-IIIF) - Lightweight, extensible IIIF image viewer.
- [Micrio](https://micr.io/iiif) - High-performance client with WebAssembly/WebGL engine and additional storytelling elements. Also offering full server IIIF support.
- [Mirador](https://github.com/IIIF/mirador) - Multi-up workspace. See also [Awesome Mirador list](https://github.com/ProjectMirador/mirador-awesome).
- [OpenLayers](https://openlayers.org) - High-performance, feature-packed Javascript library especially built for maps. It supports the IIIF Image API 2.1.
- [openseadragon-react-viewer](https://www.npmjs.com/package/openseadragon-react-viewer) - A React wrapper component around OpenSeadragon which offers selectable, extended UI functionality.
- [OpenSeadragon](https://openseadragon.github.io/examples/tilesource-iiif/) - IIIF tile support.
  - [Scalebar Plugin](https://github.com/NIST-ISG/OpenSeadragonScalebar) - OpenSeadragon plugin for physical scale overlay.
  - [Curtain Viewer](https://github.com/vanda/curtain-viewer) - Viewer based on OpenSeadragon using the curtain-sync plugin for comparing naturally aligned image variants
- [Tify](https://github.com/subugoe/tify) - Slim and fast IIIF document viewer built with Vue.js.
- [Universal Viewer](https://github.com/UniversalViewer/universalviewer) - Rich embeddable interface.

## Image API Libraries
- [iiif_url](https://github.com/NCSU-Libraries/iiif_url) - Ruby library for creating and parsing IIIF Image API URLs.
- [iiif-apis](https://github.com/dbmdz/iiif-apis) - Java IIIF API libraries.
- [iiif](https://github.com/zimeon/iiif) - Python library providing a reference implementation of the Image API. Also includes a test server and static tile generator.
- [image-iiif](https://github.com/conlect/image-iiif) - A bring your own framework solution for implementing IIIF Image API 2.1 with PHP.
- [iOSTiledViewer](https://github.com/moravianlibrary/iOSTiledViewer) - IIIF image API and Zoomify viewer for iOS, written in Swift.
- [libvips](https://libvips.github.io/libvips/) - A fast image processing library with low memory needs. Includes an operation that can build image pyramids compatible with IIIF Image API.
- [piffle](https://github.com/emory-lits-labs/piffle) - Python library for generating and parsing IIIF Image API URLs.

## Image Tools

Various tools for working with images such as cropping tools.

- [Compariscope](https://vanda.github.io/iiif-features/) - A demo app by the Victoria & Albert useful for the alignment of overlayed images, served by the IIIF Image API, and providing an interactive viewer for overlayed images, presented fluidly, using responsive image tags.
- [dezoomify-rs](https://github.com/lovasoa/dezoomify-rs) - A command-line tiled image downloader. Support IIIF, Deepzoom and others zoomable image formats.
- [IIIF cropping tool](https://ncsu-libraries.github.io/iiif-crop-tool/) - Website using [Leaflet-IIIF Cropping](https://bl.ocks.org/mejackreed/6936585f435b60aa9451ae2bc1c199f2) and Jekyll that allow users to enter the URL of a IIIF image and get the URL for the cropped section of the image.
- [iiif-dl](https://github.com/ryanfb/iiif-dl) - Command-line tile downloader/assembler for IIIF endpoints/manifests. Download full-resolution image sequences from any IIIF server.
- [IIIF-imageManipulation](https://github.com/jbhoward-dublin/iiif-imageManipulation) - UCD's tool to crop images and manipulate via IIIF attributes; integrate with Mirador via plugin.
- [Leaflet-IIIF Cropping](https://bl.ocks.org/mejackreed/6936585f435b60aa9451ae2bc1c199f2) - Example of using Leaflet to provide IIIF cropping.
- [OpenSeadragon Cropping Tool](http://sul-dlss-deprecated.github.io/iiif-cropper/demo/) - Script to allow for cropping an image from within OpenSeadragon.
- [Stanford Cropper](https://github.com/lizfischer/iiif-tools#cropper) - Simple image cropper.
- [Wikimedia Commons Image Cropper](http://zone47.com/crotos/lab/cropper/) - Create IIIF image regions from image files at Wikimedia Commons.

## Presentation API Libraries
- [IIIF Manifest Generator](https://github.com/yale-web-technologies/IIIF-Manifest-Generator) - PHP library for generating IIIF manifests.
- [iiif-apis](https://github.com/dbmdz/iiif-apis) - Java IIIF API libraries.
- [iiif-prezi](https://github.com/IIIF/iiif-prezi) - Python library providing a reference implementation.
- [iiif-tree-component](https://github.com/edsilv/iiif-tree-component) - IIIF tree menu sortable by date with multi-select capability.
- [jiiify-presentation](https://github.com/ksclarke/jiiify-presentation) - A Java IIIF Presentation library.
- [Manifesto](https://github.com/UniversalViewer/manifesto) - IIIF Presentation API client and server utility library.
- [Manifold](https://github.com/UniversalViewer/manifold) - Wraps Manifesto to provide viewer state and related utilities.
- [O'Sullivan](https://github.com/IIIF/osullivan) - Ruby API for creating IIIF manifests.
- [pyIIIFpres](https://github.com/giacomomarchioro/pyIIIFpres) - A Python module built for easing the construction of JSON manifests compliant with IIIF API 3.0 in a production environment, similarly to iiif-prezi for earlier versions of the protocol.
- [Swiiift](https://github.com/mejackreed/Swiiift) - IIIF presentation API library for Swift.
- [tabula-rasa](https://www.npmjs.com/package/tabula-rasa) - npm module for creating and manipulating IIIF manifests.
- [ViewDir](https://iiif-commons.github.io/) - Documentation on IIIF-related libraries and components, from an open community of designers and developers interested in creating composable and interoperable interfaces for consuming and creating online content.

## Presentation API Shims

These shims allow you to use systems with presentation metadata (e.g. structure or sequences) that do not currently support IIIF. If you have not implemented the Presentation API yet, this is probably not where you want to start.

- [Chronicling America](https://github.com/azaroth42/presentation-api-shims/tree/master/shims/chronam) - For newspapers digitized in the National Digital Newspaper Program.
- [Shimmy](https://github.com/mejackreed/shimmy) - Ruby gem designed to help you build shims for the IIIF Presentation API, and has samples for NYPL, Flickr, and the US National Archives.

## Presentation Manifest Tools

- [biiif](https://github.com/edsilv/biiif/) - Organise your files according to a simple naming convention to generate IIIF v3 manifests.
- [demetsiiify](https://github.com/jbaiter/demetsiiify) - Web service for creating IIIF manifests from METS/MODS documents.
- [File Analyzer IIIF Manifest Generator from Existing Metadata](http://georgetown-university-libraries.github.io/File-Analyzer-Test-Data/iiif/) - Georgetown's desktop application that will generate IIIF manifest files from existing metadata files.
- [IIIF Download](https://www.lizmfischer.com/iiif-tools/download) - Input a IIIF Manifest URL to and the desired image size to download a zip of all that Manifest's images
- [IIIF Manifest Explorer](https://www.lizmfischer.com/iiif-tools/manifest) - Input a IIIF manifest link to see basic object and image metadata in a human-friendly format.
- [iiif-producer](https://github.com/ubleipzig/iiif-producer) - A CLI tool that generates IIIF Presentation 2.1 Manifests from METS/MODS (produced by Kitodo).
- [Manifest Editor](https://github.com/bodleian/iiif-manifest-editor) - Web application for importing, viewing, updating, and exporting manifests. See a [demo](https://digital.bodleian.ox.ac.uk/manifest-editor/).
- [Brif](https://github.com/pierrz/brif) - A boilerplate tool based on Docker and FastAPI, designed to streamline the development and deployment of IIIF compliant platforms. Powering up muzz.app. See live [demo](https://brif-demo.muzz.app/dashboard).

## Validators 
- [Hyperion](https://www.npmjs.com/package/@hyperion-framework/validator) - IIIF Presentation API 3 Validator in JavaScript
- [Tripoli](https://ddmal.github.io/tripoli/) - IIIF Presentation API 2.0+ validation library.

## Exhibition and Guided Viewing Tools

Tools and resources that provide functionality for presenting IIIF materials in an exhibition-like setting (and potentially other functionality).

- [Annona Range Storyboard](https://ncsu-libraries.github.io/annona/range/) - [Annona](https://ncsu-libraries.github.io/annona/) toolkit which allows for the guided viewing of segments of a manifest, in addition to the [Annona Multi Storyboard Viewer](https://ncsu-libraries.github.io/annona/multistoryboard/) for guided comparison of multiple manifests.
- [Curation Tools](http://codh.rois.ac.jp/software/) - Set of tools, including a Viewer, Curation Manager, Curation Board, and more from the Center for Open Data in the Humanities (all tool descriptions in Japanese, some also available in English).
- [Exhibit](https://exhibit.so/) - A free IIIF storytelling tool that allows for guided navigation of one or more IIIF Manifests using annotations.  
- [Micrio](https://micr.io/iiif) - High-performance client with WebAssembly/WebGL engine and additional storytelling elements. Also offering full server IIIF support.
- [Omeka-S plugins](#cms-integration) - additional plugins and description in the [CMS Integration](#cms-integration) section
- [Panel Truck](https://geoservices.leventhalmap.org/cartinal/documentation/panel-truck.html) - Vue-based presentation tool, embeddable into any page as a Web Component, which supports slide-like narration over one or multiple IIIF sources, as well as static images and tiled map sources. ([Example](https://geoservices.leventhalmap.org/panel-truck/example.html))
- [Simple Site IIIF Extensions](https://jpadfield.github.io/simple-site/extensions.html) This [Simple Site](https://jpadfield.github.io/simple-site/) has several extensions that make use of IIIF to produce customised presentations of a bespoke selection of IIIF manifests (e.g. in Mirador 3, Curtain Viewer and Panel Truck).
- [Spotlight](http://spotlight.projectblacklight.org/) - a self-service approach for creating exhibit websites to highlight digital collections; based on [Blacklight](http://projectblacklight.org/).
- [Storiiies Editor](https://storiiies-editor.cogapp.com/) – a free online storytelling platform for creating guided tours of a single IIIF manifest using annotations.
- [Wax](https://minicomp.github.io/wax/) - a minimal computing project for producing digital exhibitions focused on longevity, low costs, and flexibility.
- [Yith](https://yith.dev) - a component library that interweaves IIIF manifests and their content into flexible layouts in a usable, responsive, and accessible way.


## Content Search API

Libraries and applications that support the Content Search API.

- [Blacklight IIIF Search](https://github.com/boston-library/blacklight_iiif_search) - Plugin that provides IIIF Content Search functionality for [Blacklight](https://github.com/projectblacklight/blacklight)-based Rails applications.
- [Ocracoke](https://github.com/NCSU-Libraries/ocracoke) - Rails application to create, index, and search text from page images and provide results in IIIF Content Search API format.
- [Whiiif](https://github.com/mbennett-uoe/whiiif) - Python/Flask/Solr application to index IIIF manifests alongside ALTO representations and provide a IIIF Content Search API endpoint.

## Authentication

Some resources about the IIIF Authentication API.

- [IIIF Auth Demonstrator](https://iiifauth.digtest.co.uk/) - Manifests with accompanying images that demonstrate various IIIF authentication modes.
- [iiif-auth-client](https://github.com/digirati-co-uk/iiif-auth-client) - Client implementation of the IIIF Authentication specification.
- [iiif-auth-server](https://github.com/digirati-co-uk/iiif-auth-server) - A demo server implementation of all apsects of the IIIF Authentication specification.
- [iiif-image-auth](https://github.com/robcast/iiif-image-auth) - A simple server implementation based on Docker and Flask.
- [IIIF.io : the hardest part will be saying "no".](http://mcormond.blogspot.com/2017/06/iiif-hardest-part-saying-no.html) - Blog post by Russell McOrmond considering the challenges of restricting access to Canadiana's resources.

## Tutorials

Tutorials for how to accomplish functionality in your applications.

- [Archiviiify](https://literarymachin.es/archiviiify/) - A short guide to download digitized books from Internet Archive and rehost on your own infrastructure using IIIF with full-text search [from raffaele messuti / [@atomotic](https://github.com/atomotic)].
- [Drag and Drop](https://medium.com/@aeschylus/create-and-share-iiif-items-quickly-and-easily-with-drag-and-drop-over-email-879f13c9caba) - Getting a IIIF image into Mirador with drag-and-drop and email.
- [Experiments with IIIF and Gallica](https://github.com/altomator/IIIF/) - A guided tour of end user applications of IIIF to Gallica materials, by Jean-Philippe Moreux (BnF).
- [Fellow Travelers: The Canterbury Tales and IIIF](http://web.stanford.edu/group/dmstech/cgi-bin/wordpress/author/blalbrit/) - Benjamin Albritton; includes an explanation of the use case for medieval scholars using Chaucer as an example and short section on how to make a page comparison demo in Mirador.
- [Getting started with IIIF](https://iiif.github.io/training/intro-to-iiif/) - Introduction originally presented during a workshop at the 2017 Code4Lib Conference at Los Angeles, CA.
- [Introduction to APIs using IIIF](http://www.meanboyfriend.com/overdue_ideas/2016/06/introduction-to-apis-using-iiif/) - Uses IIIF as an example to explain APIs.
- [IIIF Implementation Guide](http://iiif.io/assets/acc_implementation_guide_011017.pdf) - A step-by-step walkthrough of how to implement IIIF.
- [IIIF Intro (fr)](https://doc.biblissima.fr/introduction-iiif) - Introduction to IIIF (in French).
- [IIIF Quick Start Guide](http://iiif.io/technical-details/) - Quick overview of how you might get started with implementing various IIIF standards.
- [IIIF Workshop](http://ronallo.com/iiif-workshop/) - An online workshop that covers the basics of IIIF including the Image and Presentation APIs.
- [IIIF Workshop for DHNord2020](https://github.com/regisrob/Atelier_IIIF_Conference_DHNord_2020) - French langauge workshop with three exercises from a workshop entitled "Adopt and use IIIF standards for your digital image corpora," created by Régis Robineau (technical coordinator of Biblissima) and Johann Holland (TGIR Huma-Num).
- [Image API Playground](https://www.learniiif.org/image-api/playground) - Learn about the structure of a IIIF URL through manipulating the parameters and seeing the results in a live demo.
- [Image Choice video](https://www.youtube.com/watch?v=4AJPVktQ1Zw) - Demonstration of how a canvas can have a choice of images and a viewer can toggle between them.
- [Introduction to APIs using IIIF](http://www.meanboyfriend.com/overdue_ideas/2016/06/introduction-to-apis-using-iiif/) - Uses IIIF as an example to explain APIs.
- [Introduction to IIIF](https://resources.digirati.com/iiif/an-introduction-to-iiif/) - A thorough introduction to the IIIF specifications and tools for using them, by Tom Crane at Digirati.
- [Introduction to IIIF in Portuguese](https://medium.com/ecologiadigital/conhecendo-o-iiif-padr%C3%B5es-e-ferramentas-para-publica%C3%A7%C3%A3o-de-imagens-na-web-a62af62a1b36) - Covers Image API, Presentation API, and annotations.
- [Suggested measures for deploying IIIF in Swiss cultural heritage institutions (White paper)](https://doi.org/10.5281/zenodo.2640415) - Julien A. Raemy & René Schneider (2019).

## Videos and Slide Decks

Slide decks and presentation videos with a focus on IIIF.

- [An Introduction to the International Image Interoperability Framework](https://drive.google.com/file/d/0BwIq5pa1_rvfMnhCZmtzNTc5dnc/view) - Presentation introducing IIIF for new audiences as "the API for humans" - also contains videos from other IIIF presentations.
- [Collection of slide decks](http://www.slideshare.net/IIIF_io/clipboards) - From various IIIF events.
- [DHtech Workshop: Image Servers and IIIF](https://doi.org/10.20375/0000-000b-cb01-f) - Slides and recording from a DARIAH-DE workshop in 2018 by Robert Casties.
- [Image API Introduction](https://docs.google.com/presentation/d/1urCPiL3LffkIWglKGW4SSEiojBt2_RKmt5YuDtBoRfY/edit?usp=sharing) - High level overview of the Image API parameters.
- [IIIF For Small Projects](http://www.slideshare.net/workergnome/iiif-for-small-projects) - How IIIF can be used on small projects with limited infrastructure, presented at [KeystoneDH 2016](http://keystonedh.network/2016/).
- [IIIF Tutorials (German)](https://www.youtube.com/playlist?list=PLxDekeBVQtVJeRqoTgsif7fJki2X96O-1) - YouTube playlist from the Zurich Central Library (Zentralbibliothek Zürich).
- [Introduction to IIIF](https://drive.google.com/open?id=0B8APFBow4sHvNUNDQmp1Yko4VjQ) - Extensive presentation introducing IIIF with numerous examples and video demos, Beijing, October 2017.
- [Introduction to IIIF (German)](https://drive.google.com/open?id=1PQAuaTbkPzmJOMDxtihyS0-gbUtTTcDC) - German translation of the above presentation.
- [Introduction to the Presentation API](http://www.slideshare.net/azaroth42/iiif-presentation-api) - Rob Sanderson.
- [OA - Shared Canvas - TEI - Biblissima project](http://www.slideshare.net/biblissima/oa-shared-canvas-tei-biblissima-project) - Part of a workshop on TEI and neighboring standards including IIIF.
- [Video from IIIF event at the National Gallery of Art](https://www.youtube.com/playlist?list=PLYPP1-8uH9c6iQpKTXnhnlQpmoMLT1fB7) - May 2015.
- [Video from the outreach event at the Museum of Modern Art ](https://www.youtube.com/playlist?list=PLYPP1-8uH9c5smSD2wyVgsqKxD218khZq) - May 2016.
- [YouTube playlist from IIIF Göttingen Lightning Talks](https://www.youtube.com/playlist?list=PLYPP1-8uH9c6rqC0KbHUPyfmHkfvCQYCk) - Short talks (usually ~10 minutes) covering a variety of topics and new IIIF implementations; recorded June June 26, 2019 (see [full program](https://iiif.io/event/2019/goettingen/wednesday/) for links to abstracts).
- [YouTube playlist from IIIF Göttingen Showcase](https://www.youtube.com/playlist?list=PLYPP1-8uH9c534aTUrsPX1xX86KGVWmAu) - Day of presentations geared toward relative newcomers to IIIF, covering a variety of general topics; Recorded June 24, 2019 (see [full program](https://iiif.io/event/2019/goettingen/showcase/) for links to abstracts).
- [YouTube playlist from IIIF Week 2020](https://www.youtube.com/watch?v=k1VsUZZTDNE&list=PLYPP1-8uH9c4QFWKf-dbv3Il4ukkuFAje) - Presentations and demos from the IIIF Week Online event which was held between 1 and 5 June 2020.

## Discovery

Links to help you discover IIIF resources that have been shared, demonstrations of IIIF discovery and useful discovery tools.

- [Biblissima IIIF-Collections](https://iiif.biblissima.fr/collections/) - Prototype application that allows you to search across IIIF-compliant manuscripts and rare books dated before 1800.
- [Europeana's IIIF filtered search](https://www.europeana.eu/portal/en/search?q=provider_aggregation_edm_isShownBy%3A*iiif*&view=grid) - Europeana provides a filter to identify all IIIF-enabled resources in its collections.
- [IIIF Discovery in Japan](http://iiif2.dl.itc.u-tokyo.ac.jp/s/iiif/page/home) - Prototype discovery system for IIIF resources in Japan.
- [IIIF Explorer](https://researchworks.oclc.org/iiif-explorer/) - OCLC's IIIF Explorer is a prototype application that searches across images (all IIIF-enabled) in the CONTENTdm digital content management systems hosted by OCLC.
- [iiif-universe](https://github.com/ryanfb/iiif-universe) - Repository that includes links to known IIIF presentation manifest collections.
- [iNQUIRE demo](http://inquire.armtest.uk/) - Open-source IIIF-compliant research and discovery platform. This is the IIIF-compliant version of the platform driving [Digital Bodleian] (http://digital.bodleian.ox.ac.uk/).
- [iNQUIRE source](https://github.com/armadillo-systems/inquire) - Github repository for iNQUIRE.
- [Musiclibs](https://musiclibs.net) - Provides cross-library search of thousands of musical scores and manuscripts.

### Import to Viewers

- [iiif.link](https://github.com/atomotic/iiif.link) - A url shortener for sharing a IIIF resource; upon opening the URL the viewer will open at the saved zoom and region of interest.
- [Open in IIIF Viewer](https://github.com/2SC1815J/open-in-iiif-viewer) - A web browser extension to open IIIF manifest link in your favorite IIIF viewer. 

## Annotations

While annotations are not specified by IIIF they are an important enabling technology.

- [Annona Annotation Library: iiif-annotation viewer JavaScript library](https://ncsu-libraries.github.io/annona/) - JavaScript library that uses custom tags and url of the annotation to load annotated image, corresponding annotations, tags, and text into HTML object or OpenSeadragon viewer with overlays.
- [In the Spotlight](http://playbills.libcrowds.com/) - Crowdsourced contributions are serialised according to the [Web Annotations Data Model](https://www.w3.org/TR/annotation-model/).
- [Recogito](https://recogito.pelagios.org/) - A popular and award-winning Digital Humanities platform for collaborative document annotation, maintained by [Pelagios](https://pelagios.org/). 
- [Storiiies](http://storiiies.cogapp.com/) - Demos of using annotations for storytelling.

### Annotation Servers

- [annotot](https://github.com/PenguinParadigm/annotot) - Simple IIIF annotations mounted in a Ruby on Rails applications.
- [Elucidate](https://github.com/dlcs/elucidate-server) - Java and Postgres annotation server.
- [ipfs-iiif-db](https://github.com/pgte/ipfs-iiif-db) - IIIF annotations JS client over IPFS.
- [Local IIIF Annotation Server](https://github.com/dnoneill/annotate) - Jekyll front end, Flask backend, equipped with Vagrant Box that provides a Mirador viewer for creating and save annotations into Jekyll site. Annotations are sharable by using GitHub pages with Jekyll front end.
- [MangoServer](https://github.com/azaroth42/MangoServer) - Mongo-backed annotation server written in Python.
- [SimpleAnnotationServer](https://github.com/glenrobson/SimpleAnnotationServer) - Java annotation server backed by an Apache Jena triple store, Sesame, or Solr.

### Annotation Clients

- [Annonatate](https://annonatate.herokuapp.com) - Website that allows users to create annotations via their GitHub account. The website saves all the annotations to the user's GitHub. Also makes use of Annona and allows users to create custom Annona views.
- [IIIF Annotation Studio](https://github.com/atomotic/iiif-annotation-studio) - Mirador Viewer packaged as a desktop app (macos, linux) with an embedded annotation endpoint that saves annotations to a local sqlite database.

## CMS Integration

Content Management Systems (CMS) modules that implement or leverage the IIIF APIs.

- [IIIF Image Field](https://www.drupal.org/sandbox/sdellis/2421047) - Drupal 7 module that provides an easy way to add IIIF Images to content types, and configure their display. Supports Image API versions 1.0 or 2.0.
- [IIIF Server Omeka S Module](https://omeka.org/s/modules/IiifServer/) - Omeka S module that implements the IIIF Image and Presentation APIs.
- [IIIF Toolkit](https://github.com/utlib/IiifItems) - IIIF Toolkit by University of Toronto Libraries is a plugin for Omeka Classic (2.3+) that integrates Mirador with a built-in annotator, a manifest generator, Simple Pages shortcodes and Exhibit Builder blocks for a rich presentation experience.
- [Mirador Viewer Omeka S Module](https://github.com/Daniel-KM/Omeka-S-module-Mirador) - Omeka S module that integrates the Mirador image viewer.
- [UniversalViewer Omeka S Module](https://omeka.org/s/modules/UniversalViewer/) - Omeka S module that integrates UniversalViewer.

## Newspapers

These are resources that are specifically useful for working with newspapers. Many of them are outputs of the [IIIF Newspaper Community Group](http://iiif.io/community/groups/newspapers/).

- [docker-open-oni](https://github.com/open-oni/docker-open-oni) - Docker friendly setup for open-oni, which will set up and configure the Web application as well as the MySQL, Solr and RAIS Image Server.
- [IIIF Newspapers Google Drive Folder](https://goo.gl/jNFfVw) - Working documents of the Interest Group for meeting minutes, and working drafts of best practices, etc.
- [ndnp_iiif](https://github.com/umd-mith/ndnp_iiif) - Python program for turning [National Digital Newspaper Program data](https://www.loc.gov/ndnp/) into static IIIF JSON that is ready for mounting on the Web.
- [open-oni](https://github.com/open-oni/open-oni) - Friendly fork of [chronam](https://github.com/libraryofcongress/chronam) which is a webapp for viewing National Digital Newspaper Program data from the Library of Congress.
- [Populating the Annotation Store with IIIF Annotation List](https://github.com/glenrobson/SimpleAnnotationServer/blob/master/doc/PopulatingAnnotations.md) - Provides instructions on how to edit OCR text using annotations in Mirador.
- [Welsh Newspapers Online](http://newspapers.library.wales/) - Provides access to over 1 million newspaper pages using the IIIF Image API.
- National Library of Wales' guide to [IIIF Newspapers](http://dev.llgc.org.uk/wiki/index.php?title=IIIF_Newspapers) provides an explanation and examples of how IIIF applies to newspapers.

## STEM

Science, Technology, Engineering, Math/Medicine

- [CellXplorer](https://courses.edx.org/courses/course-v1:HarvardX+MCB64.1x+2T2016/d16e07a5cec442eeb7cd9dfcb695dce0/) - Cell biology annotations in a deep zoom viewer.

## Experiments and Fun

- [3D trade cards explorer](http://labs.cogapp.com/tc/) - A 3D environment that displays nineteenth-century trade cards from the [Boston Public Library](https://www.digitalcommonwealth.org/collections/commonwealth:gq67jz045). Designed to be viewed on a mobile phone, ideally with Google Cardboard. Created using three.js by Jon White, Cogapp.
- [Animal Crossing Art Generator](https://experiments.getty.edu/ac-art-generator) - Getty's tool leverages IIIF to create custom patterns featuring artwork from famous art collections around the world.
- [ANTLITZ.NINJA](https://antlitz.ninja) - Award-winning digital art app that cuts and re-combines historical portraits. Based on IIIF.
- [cover.boutique](https://cover.boutique) - Award-winning web application to create designs for smartphone cases from IIIF resources.
- [Automapic collections bot](https://twitter.com/auto_mapic) - Twitter bot that randomly pulls a IIIF excerpt, zoomed in at maximum resolution, from the Leventhal Map & Education Center's digital collections
- [David Rumsey MapTab](https://chrome.google.com/webstore/detail/david-rumsey-map-collecti/fnheacjohhlddiffbmafmpoblbkfgmde?hl=en) - A IIIF powered, Chrome extension that displays a random map from the David Rumsey Map Collection everytime you open a new tab in your browser. Built using Leaflet-IIIF and React.js. Created by Jack Reed, Stanford University Libraries.
- [Exquisite Corpse](https://github.com/harvardartmuseums/exquisite-iiif-demo) - A prototype that deliberately mixes up portrait paintings. Created using Node.js by Jeff Steward, Harvard Art Museums.
- [Fractals](http://www.appliediiif.org.uk/live/fractalshome.htm) - Deep zoom into a huge (1bn x 1bn pixel) fractal image, created by Sean Martin, Applied IIIF.
- [IIIF Gallery](http://digirati-co-uk.github.io/iiif-gallery/src/) - A virtual art gallery using OpenSeadragon and custom image generation, created by Stephen Fraser, Digirati. Also see [full source code](https://github.com/digirati-co-uk/iiif-gallery/).
- [IIIF Stereographs](https://stereograph.davidnewbury.com/) - Exploring Stereo Photos with IIIF
- [Image Comparison with a Magnifying Glass](http://resources.digirati.com/iiif/an-introduction-to-iiif/dee-mag.html) - Image comparison using leaflet magnifying glass by Digirati.
- [Image Comparison with a Slider](http://resources.digirati.com/iiif/an-introduction-to-iiif/dee-sbs.html) - Image comparison using leaflet slider by Digirati.
- [Old Map Room](https://itunes.apple.com/us/app/old-map-room/id1347431506) - An AppleTV application that uses IIIF to turn any room into a map room.
- [Puzzles! Powered by IIIF](http://puzzle.mikeapps.me/) - Drag-and-drop image tile puzzles created by Michael Appleby, Yale Center for British Art.
- [Sleep Stories](http://bitly.com/wcquilt) - Experiment with the W3C Web Annotation Data Model. The  annotations present a sequence of stories associated with a large image. Optimised for mobile. Created by Andrew Dyton and Stephen Fraser, Digirati, for Wellcome Collection.
- [Slider puzzles](http://blalbrit.github.io/puzzles) - More drag-and-drop puzzles and a Medieval Word Maker, created by Ben Albritton, Stanford University Libraries.
- [Storiiies](http://storiiies.cogapp.com/) - Cogapp's showcase of recent experiments in digital storytelling using IIIF.
- [The Transcriptinator](http://labs.cogapp.com/transcriptinator/) - A prototype "game" created for use on the British Library's crowd-sourcing arcade machine. Players have to flag up errors in the OCR transcriptions of content taken from the [Qatar Digital Library](http://www.qdl.qa). Created by Jon White and Tristan Roddis, Cogapp.
- [Wax](https://minicomp.github.io/wax/) - Minimal computing for producing digital exhibitions with Jekyll.
- [X-raying Balenciaga](https://www.vam.ac.uk/articles/x-raying-balenciaga) - Beautiful use of IIIF images to show X-rays of Balenciaga fashion by the Victoria & Albert Museum.

## Community

IIIF is a community-based initiative that relies on active participation, discussion, and input. To get involved and learn more, see the [IIIF Community page](http://iiif.io/community/).

- Join the [IIIF-Discuss email list](https://groups.google.com/forum/#!forum/iiif-discuss).
- Join [IIIF Slack](https://docs.google.com/forms/d/e/1FAIpQLSdGV9QSFo8i2z1R5iIMP7B2JVhS9akHqcykWF5_y4mtWqVrBA/viewform) for the most up to date and broad discussions.
- Read quarterly [IIIF Community Newsletters](http://iiif.io/news/) to stay up to date with the latest community activities.
- [Submit a IIIF-related news item](https://goo.gl/forms/2LMe9zUHVBEbI62C3) to the IIIF Community Newsletter.
- Contribute to one of the [IIIF community and/or technical groups](http://iiif.io/community/groups/).
- Participate in the bi-weekly IIIF community calls. See the [IIIF community calendar](http://iiif.io/community/groups/) for details.
- Learn more about the [IIIF Consortium](http://iiif.io/community/consortium/).
- Attend a [IIIF event](http://iiif.io/event/).
- [iiif_io on Twitter](https://twitter.com/iiif_io).

## Digital Asset Management (DAMs) that support IIIF

 - [Archipelago](https://archipelago.nyc/)
 - [Axiell Collections](https://www.axiell.com/solutions/product/axiell-collections/)
 - [CollectiveAccess](https://collectiveaccess.org)
 - [ContentDM](https://www.oclc.org/en/contentdm/iiif.html)
 - [Goobi](https://goobi.io)
 - [Islandora](https://islandora.github.io/documentation/user-documentation/iiif/)
 - [Invenio](https://invenio-software.org/products/framework/)(Image API implementation via [invenio-iiif](https://github.com/inveniosoftware/invenio-iiif))
 - [Libnova/Libsafe](https://www.libnova.com/)(Image API)
 - [Luna](http://www.lunaimaging.com/iiif)
 - [Muzz.app platform](https://muzz.app) (based on [Brif](https://github.com/pierrz/brif))
 - [ResCarta](https://rescarta.org/)
 - [ResourceSpace](https://www.resourcespace.com/knowledge-base/api/iiif)
 - [Rosetta](https://knowledge.exlibrisgroup.com/Rosetta/Training/What's_New_Videos/Rosetta_5-3)

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, all contributors waive all copyright and related neighboring rights to this work.
