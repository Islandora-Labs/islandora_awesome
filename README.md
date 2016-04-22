# Awesome Islandora [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

## Introduction

A curated list of great modules for Islandora that are not included in the core release. Inspired by the [awesome](https://github.com/sindresorhus/awesome) list.

These community modules are mostly functional or well on their way. Some may find their way into future releases as part of the standard Islandora suite. Others may always stand alone, but they all add useful functionality and new tools. We offer this list for discovery, but do not officially provide support for any of these modules.

## Table of Contents
   * [Solution Packs](#solution-packs)
   * [Utility Modules](#utility-modules)
   * [Viewers](#viewers)
   * [Demo Modules](#demo-modules)
   * [Other](#other)

## Contribute

If you would like to contribute to this list, please check out [CONTRIBUTING.md](CONTRIBUTING.md). 

Please ensure your pull request adheres to the following guidelines:

* Use the following format: 
   * `[Module Name](link)` (Status: **Stable** or **In Development**) - Brief Description of what the module does
* Make an individual pull request for each new item.
* Link additions should be inserted alphabetically to the relavant category
* New categories or improvements to the existing categorization are welcome.
* Check your spelling and grammar.
* The pull request and commit should have a useful title.

## Troubleshooting/Issues

Having problems or solved a problem? Check out the Islandora google groups for a solution.

* [Islandora Group](https://groups.google.com/forum/?hl=en&fromgroups#!forum/islandora)
* [Islandora Dev Group](https://groups.google.com/forum/?hl=en&fromgroups#!forum/islandora-dev)

## Maintainers/Sponsors

Current maintainers:

* [Melissa Anez](https://github.com/manez)

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the owner has waived all copyright and related or neighboring rights to this work.

## The List

### Solution Packs
* [Islandora Binary Solution Pack](https://github.com/Islandora-Labs/islandora_binary_object) (Stable) - Adds all required Fedora objects to allow users to ingest supplemental files through the Islandora interface. Used best in conjunction with the Islandora Compound Solution Pack.
* [Islandora Document Solution Pack](https://github.com/discoverygarden/islandora_solution_pack_document) (Stable) - Provides a collection and a content model for users’ documents. Documents are converted to the pdf format to display them. This solution pack needs OpenOffice running as a service and also the JODCoverter library installed.
* [Islandora EAD Solution Pack](https://github.com/DrexelUniversityLibraries/islandora_solution_pack_ead) (Stable) - Provides functionality for ingestion and management of EADs.
* [Islandora Manuscript Solution Pack](https://github.com/discoverygarden/islandora_solution_pack_manuscript) (Stable) - Allows users to create and view Manuscripts. Including the upload of TEI and XSLT and CSS documents. Users will be able to view transformed manuscript TEI (via the upload XSLT) side by side with the image(s) of the manuscript (via the Open Seadragon viewer). Users will also be able to browse Manuscripts via Box / Folder hierarchies as defined by their record in an associated finding aid.

### Utility Modules
* [Islandora Authority](https://github.com/discoverygarden/islandora_authority) (Stable) - This module adds two Drupal form API elements and a menu path used for autocompletion on one of them.
* [Islandora Block Options](https://github.com/echidnacorp/block_islandora_options) (Stable) - Adds additional placement options to all blocks for Islandora options that are similar to the content type options for nodes. Adds the ability to limit blocks visibility based on the cmodel being viewed.
* [Islandora Drag & Drop](https://github.com/unc-charlotte-libraries/islandora_ingest_dragndrop) (Stable) - This ingest module provides a methodology for creating a drag-and-drop batch ingest workflow powered by a local Linux-based NAS system integrated with an Islandora ingest server.
* [Islandora Entity Bridge](https://github.com/btmash/islandora_entity_bridge) (Stable) - Provides a simple connector between Islandora/Fedora Entities and Drupal. It is to allow for referencing Islandora Objects (like in Flag, Entity Queue, Entityreference, etc) without bringing in the full weight of an Entity like Node. 
* [Islandora Generate/Regenrate Collection Datastreams](https://github.com/qadan/islandora_batch_derivative_trigger) (Stable) - Allows mass regeneration of selected derivatives for selected content models, as well mass regeneration of the DC metadata for selected content models within a collection. 
* [Islandora GSearcher](https://github.com/discoverygarden/islandora_gsearcher) Stable - Sends created and edited objects to be indexed via the Fedora Generic Search Service on page exit, removing the need for ActiveMQ between Fedora and GSearch.
* [Islandora Job](https://github.com/discoverygarden/islandora_job) (Stable) - Utilizes Gearman to facilitate asynchronous and parallel processing of Islandora jobs and allows for Drupal modules to register worker functions and routes received messages from the job server to the appropriate worker functions.  
* [Islandora Object Lock](https://github.com/discoverygarden/islandora_object_lock) (Stable) - Allows users to lock objects to prevent modifications by other users. It also automatically locks objects when edits are being made to datastreams through the XML Form Builder.
* [Islandora Plupload](https://github.com/discoverygarden/islandora_plupload) (Stable) - Integrates the Plupload library with Islandora file fields to allow for the upload of files greater than limits imposed by PHP.
* [Islandora PROAI](https://github.com/fritsvanlatum/islandora_proai) Stable) - Provides an integration of Fedora's [OAI Provider Service 1.2.2](https://wiki.duraspace.org/display/FCSVCS/OAI+Provider+Service+1.2.2) within Islandora.
* [Islandora Relationship Editor](https://github.com/giancarlobi/islandora_relationship_editor) (Stable) - With this module, you can add RELS-EXT relationships to an object via the "Manage" tab. You can also add the reciprocal ('symmetric') relationship. Relationships are derived from the ontology file.
* [Islandora REST API](https://github.com/discoverygarden/islandora_rest) (Stable) - An extremely well documented module that provides a number of REST end points for fetching/manipulating objects, datastreams, and object relationships from islandora.
* [Islandora Saved Searches](https://github.com/echidnacorp/islandora_saved_searches) (stable) - Adds the ability to save searches on the Islandora SOLR index provided by the Islandora SOLR module.
* [Islandora Usage Stats Callbacks](https://github.com/flvc/islandora_usage_stats_callbacks) (stable) - A helper module that works with [Islandora Usage Stats](https://github.com/Islandora/islandora_usage_stats) to take the data it collects and expose it via URL callbacks.
* [Islandora Webform](https://github.com/commonmedia/islandora_webform) (Stable) - A module that allows the use of Drupal webforms to contribute metadata for an Islandora object, with a workflow at the webform or object level for site managers to review and ingest submissions. Useful for allowing public contributions into a moderated workflow.
* [Islandora XML Form Builder States](https://github.com/Michigan-State-University/islandora_xml_form_builder_states) (Unknown) - This module modifies the way forms work to add basic support for the "#states" function inherant in Drupal 7 core. While this module has limitations in support of multiple values on a condition, it does extend basic functionality. This module assumes you know how to use the Islandora XML Form Builder. If you need to learn how to use the Islandora XML Form Builder, please consult the help for that module.

### Viewers

### Demo Modules
* [Islandora Porcus](https://github.com/ajstanley/islandora_porcus) (N/A) - Developed for the first Islandora Camp Developer's Track workshop and refined at subsequent camps. On the surface, Porcus is a module that will take text and translate it to pig latin. Check under the hood and you will find a heavily commented training tool that presents the basics of module development for Islandora and provides a handy reference for how the various parts interact. Created For Islandora Camp NY 2013.
* [Islandora Meme Solution Pack]() (N/A) - Created for Islandora Camp Colorado 2014 in order to provide a framework to learn how to query solr in Islandora.
* [Piggy Back](https://github.com/ppound/islandora_piggyback) (N/A) - An extension for the Porcus module with additional demonstrations and tools. Created for Islandora Camp CA 2014.

### Other
