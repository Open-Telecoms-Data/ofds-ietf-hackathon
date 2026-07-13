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
* Digitize some of the identified maps so that they are available in OFDS.
* Install, use, review, fix the open source tools that work with OFDS.
* Improve the current documentation for OFDS.
* Provide feedback on the current draft 0.4 of OFDS.

----

## Projects

### Mapping - Identifying and digitzing maps
The end result will be a more completely filled-in map that can provide examples of good practice around the world.

#### Finding Maps of broadband / fiber systems that can be digitized
Ready to do some web searching? The objective is to find network maps that are out there that are not yet known. In some countries regulators _may_ have these maps, but usually it is the Internet Service Providers (ISPs) / network operators who may have these maps. Often, they just simply are not posted online.

**Tasks:**
* Find broadband maps through searching.
* Check the [current](https://opentelecomdata.org/good-practice-map/index.html) to see if it has already been entered
* Add to [file]

#### Digitizing maps

----

### Tools

There are several open source tools that work with OFDS. The tasks in the Hackathon would be to test out the tools, raise issues if you experience any problems or have suggestions, review the documentation, and offer changes.

#### KML to OFDS Converter
KML2OFDS is a Python script for converting KML maps of fibre optic network infrastructure into OFDS. A typical workflow might involve digitizing a map using `OFDS Studio` (see below) to then generate a KML file. The next step is to take that KML file and run it through `KML2ODFS` to get the resulting ODFS files.

The tool is found in the repo: https://github.com/Open-Telecoms-Data/kml2ofds

**Tasks:**
* Install `KML2ODFS` and get it running.
* Review the documentation and [raise any issues](https://github.com/Open-Telecoms-Data/kml2ofds/issues)
* Review [current issues](https://github.com/Open-Telecoms-Data/kml2ofds/issues) and see if you can assist with more info or a PR.
* Modify the code to add functionality (using an issue and PR).

#### OFDS Studio

#### COVE

----



### Input Into OFDS Version 0.5

----

### Documentation
The current OFDS documentation has been developed over time, but could certainly use new sets of eyes. The task here will be to read through the docs and offer suggestions to make them better / simpler / easier-to-understan.

**Tasks:**
* Review current documentation at https://standard.ofds.info/en/latest/
* Go to where documentation currently is in this repo: https://github.com/Open-Telecoms-Data/open-fibre-data-standard/tree/0.4-dev/docs
    * [Raise issues](https://github.com/Open-Telecoms-Data/open-fibre-data-standard/issues)
    * Open a pull request with suggestions

----

### Virtualization

----

### Other Project Ideas

There are MANY other things that can be done with OFDS. A few suggestions are below.

#### Export into OFDS
* Create a tool / plugin / module that will export into OFDS?
* Add OFDS export into an existing tool?

#### Import from OFDS
* Import OFDS into Open Street Map?
* Import OFDS into Open Infrastructure Map? - https://openinframap.org
