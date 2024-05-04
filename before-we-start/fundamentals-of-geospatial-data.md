---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Fundamentals of Geospatial Data

> "GPS tells you where a spot is on a map… GIS tells you everything about that spot." \~ [Wagadugo](https://www.reddit.com/r/gis/comments/1c3inhc/comment/kzheiil/?utm\_source=share\&utm\_medium=web3x\&utm\_name=web3xcss\&utm\_term=1\&utm\_content=share\_button)

Geographical or location data refers to information that identifies the specific physical location of a place or object. It can be obtained from diverse sources, including satellite imagery, global positioning systems (GPS), and online mapping platforms.&#x20;

Geospatial data consists of three essential components: spatial[^1], attribute, and often temporal data.&#x20;

### Spatial Data

Spatial data represents the shapes and positions of features, such as cities, rivers, and forests, on maps. Spatial data can be further categorized into two types:

**Vector Data**: This type of data represents geographic features as points, lines, and polygons. Each of these features is defined by its coordinate(s) on the Earth's surface.&#x20;

{% tabs %}
{% tab title="Point" %}
Represents a single, specific location on the map, identified by its latitude and longitude coordinates. Examples include the location of a city or a landmark.

<figure><img src="../.gitbook/assets/image.png" alt="" width="188"><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Line" %}
Represents a series of connected points, forming a line or a path. This can represent rivers, roads, or routes, among others.

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="188"><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Polygon" %}
Represents a closed shape made up of connected lines, enclosing an area on the map. Polygons are used to represent regions, such as country borders, land-use zones, or administrative boundaries.

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="188"><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}

### Attribute Data

Attribute data refers to information linked to the spatial features. These are typically stored in a tabular (table) format. For instance, a vector map of roads might include attribute data on road names, classifications, pavement types, and conditions. This data is crucial for providing context and additional details about the spatial features, enabling deeper analysis and decision-making.

### Temporal Data

Temporal data is increasingly important in geospatial analyses, as it allows users to track changes over time at a specific location. This can be crucial for applications such as environmental monitoring, urban development planning, and historical studies.

{% hint style="info" %}
### **Common Geospatial File Types**

Geospatial data comes in various file formats, each suited to specific types of data and use cases:

* **GeoJSON (.geojson)**: A format for encoding a variety of geographic data structures using JSON. It supports points, lines, and polygons and is particularly useful for web applications.
* **KML (.kml)/KMZ (.kmz)**: Used primarily by Google Earth and Google Maps, KML/KMZ files store geographic data with rich visualization features including shapes, images, and text overlays.
* **Geodatabase (.gdb)**: A more robust and scalable database model that can store multiple types of data and large datasets more efficiently than shapefiles. It is proprietary to Esri.
* **TIFF (.tiff) with GeoTIFF extension**: A format for raster data that includes embedded geographic metadata such as the coordinate system, map projection, and other specifics. GeoTIFFs are widely used for satellite imagery and aerial photography. "The information on the scale of the image (the area it covers) and the location is often stored in an accompanying .tfw file, [which should always be kept in the same folder.](https://kit.exposingtheinvisible.org/en/)"
* **NetCDF (.nc)**: Stands for Network Common Data Form, used mainly for storing multidimensional scientific data such as temperature, humidity, wind speed, direction over time, and space.
* **CSV**: This is a simple database format that can be opened in most spreadsheet and database applications and imported into many map-making applications. I[n order to place this data on a map, it must contain location information](https://kit.exposingtheinvisible.org/en/how/maps.html), such as latitude and longitude coordinates or addresses."
{% endhint %}



\
\


[^1]: 
