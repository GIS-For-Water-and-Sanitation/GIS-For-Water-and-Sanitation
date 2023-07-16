---
description: >-
  This page contains prerequisite in preparing GIS data which are QGIS Version
  >3.x, Data Model from WASREB, and Layer Styles/symbology.
---

# How to prepare GIS data

### Prerequisite

1. #### QGIS Version >3.x

QGIS is open-source GIS software available to use for free and has various plugins to enhance its capabilities. It is recommended to use the latest Long-Term Release, for this documentation we are going to be using QGIS Version 3.28 at the time of this documentation however previous versions are still able to work.&#x20;

QGIS can be downloaded through this [LINK](https://qgis.org/en/site/forusers/download.html)&#x20;

<figure><img src="https://lh4.googleusercontent.com/eSnq3r7Q6eOWCxxwAJSLW94zUeOSpXvBVX31ffG-gzGOf6ftYeWUmqjjzIvJl8cfzhW3xnMF197LxK2ZJUbsxHRqQIjNSh9WEa9OpDwDAsE151CWJclrQQkPXE92ZNUE8zjrNadS4bC2r_wHhAplbg" alt=""><figcaption></figcaption></figure>

2. #### Data Model from WASREB

Majidata WSP users are able to log in the Majidata website, view, and authorize edits or modify their own network information through the web browser. The data structure found in Majidata portal is provided by a data model which defines the network elements, attributes, and the relationships.&#x20;

The data model can be provided by WASREB for use at the WSP level to prepare GIS data, or most probably migrate the GIS data into the WASREB standards. GIS information prepared in this manner will ensure compatibility with the Majidata system and ensure an improved GIS standard at the WSP level. Although Majidata systems architecture includes a database, it is possible that some of the WSPs have no similar infrastructure therefore a file base GIS files such as shapefile. Moreso, a localhost database can be set up in the GIS department to use with other departments in the WSP.

This documentation is tailored into the details on what each layer means, the columns meaning, and the table relationships. Therefore, it is possible to replicate this with other GIS software.

3. #### Layer Styles/symbology

Network styles are GIS symbols of network features. They are GIS representations of elements that enhance visualization of features and assist in map interpretation. From Majidata portal different network features are visualized differently together with attribute definition that can be categorized and styled accordingly. A WSP user can request for network layer styling for use at a WSP level, however in this documentation styling is best illustrated in the QGIS environment which might be different from what is in the Majidata portal.

In QGIS the network layers styles/symbology assist users to better visualize and interpret the network layers on a map canvas. Network symbology assists Majidata users to understand GIS information and they enhance map interpretation for users. Majidata system has defined styles for each layer in the web portal, you can request the styles for use with your GIS. The image that follows does not necessarily reflect what is Majidata system but emphasizes on the importance of using communicating symbology for GIS. WSP Water Storage has been styled according to the op\_status/Operating Status where each status has a different color. Similarly the other layers are styled accordingly based on the categorization attribute.

<figure><img src="https://lh5.googleusercontent.com/xzoeN91WewxAZNGYrb0ZEgzbdMSOx0nsrGY6mPBWnM8l-oz2WrbPUQi_5Ns7ldzA8UIp62n4b1VcfuSojSFzr8rRgDOpbkuNaTUtAwEPVvLo7JBBJJG9HQWG0KCqJgUI2NLlyNUQC-A4c-26ZoRNHQ" alt=""><figcaption></figcaption></figure>

Figure 0-5 Symbology in WSP Network data

\
