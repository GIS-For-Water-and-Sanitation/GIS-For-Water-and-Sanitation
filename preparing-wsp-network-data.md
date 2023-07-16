---
description: This page includes QGIS and WSP Network Data Structure and Data Types,
---

# Preparing WSP Network Data

### QGIS and WSP Network Data Structure and Data Types

QGIS Software can be downloaded and installed on various platforms for open-source license. This section of the guide demonstrates how GIS network layers can be prepared for Majidata. Since the Majidata system was developed using GIS data from various WSP was used. The network data had similar GIS data structures which had to be harmonized with an improved GIS data model.&#x20;

The Majidata Data model ensures the correct representation of real-world scenarios in a GIS system. The data model includes the main layers of water/sewer systems and the layer relationships tables. This has been made possible in the Majidata system using foreign keys in the GIS database. The purpose of this relationship is to ensure clean data entry for a user who has to choose from predefined values and avoid human typing errors. Some of the fields are also automatically filled based on one qualified rule such as selecting the WSP name. We are going to see how the population of each field attribute is done for all WSP network layers.

<figure><img src="https://lh5.googleusercontent.com/AssLKdI3W4GLxM1lWSYN4uTdUff4i_zdAewgAD-rgH57D5OU3AulPJ5KBlJEi94sT6S44HrLI8Opwr_mQEZuok7PQtbDBAALXvmgrH9OYWkcWMLJBbvzIvaQEUxscii0ZB3YBfT8aKnt4qeUKkrLqg" alt=""><figcaption></figcaption></figure>

Figure 0-1 QGIS Software with WSP Network Layers

Each layer should be formatted as in the following tables in GIS software with the projection mentioned earlier or later reprojected. The column order follows the order of the New Attribute Name order in each layer. It is important to follow the Data type for storing data in GIS as described in the tables.

To understand how the Majidata system function on how to utilize GIS data from different WSP, there exist pre populated fields marked in each layer as TRUE or FALSE.

Using WSP Water Storage layer as an example auto populate layer attribute with default string for feature column can be set as follows.&#x20;

<figure><img src="https://lh4.googleusercontent.com/go56FvgcvkNVuYyOfsStZPQWo05eXz749sBCd7U7aNw8BeKGAfh2JLR_4KbL8T2JODvRn03x-PbqXsCgV0prxJ90A96krKYblQpyQQa71Nt5rYRKENbmGneXUccf-gfjtHBzUAKoV3S66ynn_2MHgQ" alt=""><figcaption></figcaption></figure>

Figure 0-2 Auto fill attribute with default value

1. In the QGIS layer pane select the layer choose a layer e.g WSP Water Storage and double click the layer to open properties.&#x20;
2. In the properties window go to the Attribute Form tab and select Feature attribute.
3. Go to section 3 highlighted and change to show form on add feature so that when a user inserts a new WSP Water Storage feature a form is displayed to fill attributes.
4. Choose widget type to text edit
5. On default value type the text to insert into the attribute e.g ‘WSP Water Storage’. For every layer type appropriately.
6. Check to apply the default value on update.

\


There are columns used to categorize or classify WSP Storage Facilities. These are added as a drop down field in QGIS through value map functionality. This is replicated in any field that requires predefined values to select from in various attributes. To make use of the value map follow the steps below.

<figure><img src="https://lh5.googleusercontent.com/sbIGw_bgQ3maPLP_JcUm2yv3YoaH4wruDNwSO2eIFGCE4Nl1lI8znnhHOQ13KSgoBLTyuI-7E4Vrhh45MaC_trAgzMq1kVeWmlnaOgHgf28YmWCwf752LbBNal85YN-akPZJLrgsT5CuNyrkdHp-sA" alt=""><figcaption></figcaption></figure>

Figure 0-3 Value Map functionality in QGIS 1

<div data-full-width="false">

<figure><img src="https://lh6.googleusercontent.com/bxNnLXn9meK6DMik9M2TpHcdXJWZasCaNq0iaCqdx7VOILZJmWedZZl8TyYOYMm6k5mkt_vxjqiC0L52KUvTkEYsc0GAbmHizhxROcb5d1nnBRptdTgdbm2lWcuxonvsK6jord7qzRNVQkQ4xsi8lA" alt=""><figcaption></figcaption></figure>

</div>

Figure 0-4 Value Map functionality in QGIS 2

1. Double click the layer to go to properties, in this case we are using WSP Water Storage.
2. In the properties window go to the Attribute Form tab and select op\_status attribute. This attribute alias is Operational Status which can be included in the alias section under general.
3. Under widget type select value map and you are going to load values from either from the layer already in QGIS or load data from the CSV file.&#x20;
4. WSP users are able to request the data model from WASREB. I have a table named wsp\_op\_status with the values of all operation status that a feature can have.
5. Click ok to finish adding the values.
