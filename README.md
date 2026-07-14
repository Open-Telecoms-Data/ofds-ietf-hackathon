# IETF 126 Hackathon - Open Fibre Data Standard (OFDS)
18-19 July 2026 - Vienna, Austria.

📆📆📆📆📆📆📆📆📆📆📆📆\
**COME TO OUR SIDE MEETING - Weds, July 22, 2:45-3:45 - Grand Klimt Hall 3**\
📆📆📆📆📆📆📆📆📆📆📆📆

The Open Fibre Data Standard (OFDS) - [ofds.info](https://ofds.info) - is a format to describe fibre and
broadband networks that can be used to generate maps for understanding Internet resilience. Network operators use many different formats for mapping their networks. OFDS is an attempt to provide a common language.

OFDS is NOT _(yet)_ an IETF standard. It was developed independently by a group of organizations including the World Bank, Mozilla, Internet Society, Internet Telecommunication Union (ITU), Liquid Intelligent Technologies, CSquared, and Digital Council Africa. The group is now seeking a permanent institutional home for OFDS in a standards development organization (SDO) and is here at IETF 126 to see if there is sufficient interest within the IETF to explore bringing it into the IETF process.

----

## Goals
At the IETF 126 Hackathon, beyond introducing people to OFDS, we'd like to:
* Expand the [Good Practice Map](https://opentelecomdata.org/good-practice-map/index.html) with more examples of maps of fibre / broadband maps.
* Digitize some of the identified maps so that they are available in OFDS and can be added to the [public data sets](https://github.com/Open-Telecoms-Data/OFDS-public-data).
* Install, use, review, fix the open source tools that work with OFDS.
* Improve the current documentation for OFDS.
* Provide input into the next version 0.5 of OFDS. (See [call for input](https://github.com/Open-Telecoms-Data/open-fibre-data-standard/discussions/355))

----

Note: There is a set of [OFDS public data sets](https://github.com/Open-Telecoms-Data/OFDS-public-data) that can be used to see what OFDS looks like, and for testing some of the different tools and systems.

----

## Getting Started 

Before getting started on projects, you want to review:

* [OFDS Documentation](https://standard.ofds.info/en/latest/) including the [Primer](https://standard.ofds.info/en/latest/primer/)
* [Blog post- What's New in OFDS 0.4: New Features, GeoPackage Support, and Practical Tools](https://ofds.info/en/blog/2026/04/whats-new-in-ofds-04/)
* [The main OFDS site](https://ofds.info/en/), including the interactive map, news stories, and other info

----

## Projects - Mapping

The end result will be a more completely filled-in map that can provide examples of good practice around the world.

### Finding Maps of broadband / fiber systems that can be digitized
Ready to do some web searching? The objective is to find network maps that are out there that are not yet known. In some countries regulators _may_ have these maps, but usually it is the Internet Service Providers (ISPs) / network operators who may have these maps. Often, they just simply are not posted online.

**Tasks:**
* Find broadband maps through searching. (You can use the [current map](https://opentelecomdata.org/good-practice-map/index.html) to see where maps are needed. Note that a country is shaded if only _one_ map is found. There may be many more networks within a shaded country.)
* Once you have found a network map, check the [current map](https://opentelecomdata.org/good-practice-map/index.html) to see if it has already been entered
* Add to [the list of identified maps](identified-maps.md), either [as an issue](https://github.com/Open-Telecoms-Data/ofds-ietf-hackathon/issues) or through a PR.

### Digitizing maps

Once maps have been identified, we need to turn the map into something that can be converted to OFDS. If the map is already in Google Earth, or has a KML file, we can potentially use the `KML2OFDS` tool (below) to generate OFDS. Otherwise, it is a process that involves tracing over the endpoints.

**Tasks:**
* Get a JPEG of the network map
* Import into (Google Earth?)
* Follow these steps (to be added)
* Export your data as... (to be added)

Note: You can watch this 10-minute video (add link) to see the steps involved.

----

## Projects - Tools

There are several open source tools that work with OFDS. The tasks in the Hackathon would be to test out the tools, raise issues if you experience any problems or have suggestions, review the documentation, and offer changes.

### KML to OFDS Converter
KML2OFDS is a Python script for converting KML maps of fibre optic network infrastructure into OFDS. A typical workflow might involve digitizing a map using Google Earth (see above) to then generate a KML file. The next step is to take that KML file and run it through `KML2OFDS` to get the resulting ODFS files.

The tool is found in the repo: https://github.com/Open-Telecoms-Data/kml2ofds

**Tasks:**
* Install `KML2OFDS` and get it running.
* Review the documentation and [raise any issues](https://github.com/Open-Telecoms-Data/kml2ofds/issues)
* Review [current issues](https://github.com/Open-Telecoms-Data/kml2ofds/issues) and see if you can assist with more info or a PR.
* Modify the code to add functionality (using an issue and PR).

### OFDS Studio

OFDS Studio is [a plugin for creating and editing OFDS data](https://plugins.qgis.org/plugins/ofds_studio/) using the free and open-source GIS tool [QGIS](https://qgis.org/), you can:

* Create OFDS data from scratch
* Import and edit an existing OFDS dataset
* Check that the data conforms to the OFDS data model
* Export OFDS data in GeoPackage and JSON formats.

You can also leverage QGIS’s powerful suite of GIS features to trace and digitise raster maps, transform non-OFDS datasets into OFDS format, and combine your OFDS data with a range of basemaps and geospatial datasets to perform spatial analysis and processing.

The code for OFDS Studio is in this repo: https://github.com/Open-Telecoms-Data/ofds-qgis-plugin

**Tasks:**
* Install OFDS Studio (and QGIS if necessary) and raise [any issues](https://github.com/Open-Telecoms-Data/ofds-qgis-plugin/issues) found during installation
* Browse the [current set of issues](https://github.com/Open-Telecoms-Data/ofds-qgis-plugin/issues) to see if you can help.
* Raise any issues and or send a PR for any improvements or suggestions.

### CoVE

CoVE (Convert, Validate, and Explore) is an online tool that performs validation on OFDS files to ensure they are correct. It can be found at https://cove.ofds.info - or it can be installed locally using Docker.

The code base is in the repo: https://github.com/Open-Telecoms-Data/cove-ofds
Issues are at: https://github.com/Open-Telecoms-Data/cove-ofds/issues

**Tasks:**
* Use COVE - https://cove.ofds.info - and raise issues if you have feedback.
* Explore [the list of current issues](https://github.com/Open-Telecoms-Data/cove-ofds/issues) to see if you can help.

----

## Project - Provide Input Into OFDS Version 0.5

With the release of OFDS version 0.4 in April 2026 ([announcement](https://ofds.info/en/blog/2026/04/whats-new-in-ofds-04/)), the group is now looking for how OFDS should evolve for the next 0.5 version. **You can help provide input!**

**Tasks:**
* Read the **[Call for Inputs into 0.5](https://github.com/Open-Telecoms-Data/open-fibre-data-standard/discussions/355)**
* Provide feedback on any of the listed open issues, particularly:
    * https://github.com/Open-Telecoms-Data/open-fibre-data-standard/issues/352
    * https://github.com/Open-Telecoms-Data/open-fibre-data-standard/issues/354
* Add any additional suggestions to [the list of open issues](https://github.com/Open-Telecoms-Data/open-fibre-data-standard/issues)

----

## Project - Documentation
The current OFDS documentation has been developed over time, but could certainly use new sets of eyes. The task here will be to read through the docs and offer suggestions to make them better / simpler / easier-to-understan.

**Tasks:**
* Review current documentation at https://standard.ofds.info/en/latest/
* Go to where documentation currently is in this repo: https://github.com/Open-Telecoms-Data/open-fibre-data-standard/tree/0.4-dev/docs
    * [Raise issues](https://github.com/Open-Telecoms-Data/open-fibre-data-standard/issues)
    * Open a pull request with suggestions
 
* This can also be done for the [OFDS Developer Handbook](https://ofds-standard-development-handbook.readthedocs.io/en/latest/)
    * Repo: https://github.com/Open-Telecoms-Data/standard-development-handbook/tree/main
    * Issues: https://github.com/Open-Telecoms-Data/standard-development-handbook/issues

----

## Project - Virtualization

The open source tools identified above could be virtualized so that they could be easily installed via Docker or similar technologies.

----

## Other Project Ideas

There are MANY other things that can be done with OFDS. A few suggestions are below.

### Export into OFDS
* Create a tool / plugin / module that will export into OFDS?
* Add OFDS export into an existing tool?

### Import from OFDS
* Import OFDS into Open Street Map?
* Import OFDS into Open Infrastructure Map? - https://openinframap.org
