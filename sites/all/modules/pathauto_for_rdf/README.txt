
CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Installation
 * Configuration


INTRODUCTION
------------

Pathauto for RDF is a pathauto-based module that creates readable paths for 
RDF versions of nodes. It is most useful with pathauto, RDF, restws and 
global redirect modules. With this module the RDF document describing a 
node can accessed at the pathauto alias URL. The module also allows custom 
paths for RDF URLs and bulk creation/update of RDF aliases.

For example, the pathauto module can create an alias for the page:

	http://site/node/1

to a more meaningful URL:

	http://site/organisation/some-organisation-name

that displays the information from the original node.


However when using RDFx and restws the RDF is still available at:

	http://site/node/1.rdf

This module allows the RDF to be accessed at:

	http://site/organisation/some-organisation-name.rdf

INSTALLATION
------------

Module installation is pretty straight forward, the prerequisites 
are the pathauto and RDFx. restws and global redirect modules are
would be nice but are optional. The module won't break anything 
without them, just not do anything!

1. For general information check 

http://drupal.org/documentation/install/modules-themes/modules-7

2. Configure the module

CONFIGURATION
-------------

By default, the module will alias URLs to the pattern:

	[node:content-type]/[node:title].rdf

as per the example above. But this can be changed, to e.g.:

	[node:content-type]/[node:title]/rdf

Configure the pattern via the URL alias patterns page:

	http://site/admin/config/search/path/patterns

under the heading RDF PATHS.

FEEDBACK
--------

If you have any comments, suggestions or bug reports, get in touch!
