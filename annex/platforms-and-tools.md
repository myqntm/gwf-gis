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

# Platforms & Tools

> Digital mapping tools such as GIS technologies and Google Earth are founded within western epistemologies and perpetuate the colonial ‘gaze’ and power inequity. These maps are far from neutral: ‘The problem with positioning GIS as software that simply gathers empirical data and presents it as fact is that such ‘scientific objectivity’ is typically situated and privileges those in power’ ([Farman](https://www.semanticscholar.org/paper/Localizing-landscapes:-a-call-for-respectful-design-Syme/45d7844e449a644556cbc8e709a3a8756b32376b)).&#x20;

So it's important to remember that these platforms are simply tools. Tools that need to be used in responsible ways. Below you'll find a list of some of the more common GIS platforms as well as the features relevant for responsible GIS practices.

### [Mapeo](https://www.digital-democracy.org/mapeo)

<mark style="background-color:blue;">Great for those looking for a secure, community friendly.</mark>

Mapeo was built by [Digital Democracy](https://www.digital-democracy.org/) with and for earth defenders to easily document environmental & human rights information and to collect data about their land. It was designed to work in entirely offline environments, is highly customizable, and built on a decentralized peer-to-peer database that allows communities to own their own data.

**More Info:**

* **Import options:** Possible to import GPS tracks and shapefiles to Mapeo Desktop.
* **Export options:** _Mapeo Desktop_: PDF or print report, GeoJSON, CSV or Shapefile export. _Mapeo Mobile_: single point export to email, Whatsapp and other mobile sharing apps.

### QGIS

<mark style="background-color:blue;">Great for those aiming for a low-cost tool, and with the resources for capacity building</mark>

QGIS is an open-source Geographic Information System (GIS) software that offers powerful tools for data editing, viewing, analysis, and composition, making it a popular choice among geographers, planners, and researchers worldwide. Highly customizable and versatile, QGIS supports various vector, raster, and database formats and functionalities. It allows users to create rich maps and complex spatial analyses without the cost of proprietary software. The platform's strong community support and continual updates ensure that it remains at the cutting edge of GIS technology, providing a reliable and accessible option for anyone looking to utilize GIS in their projects, whether they are in academia, government, or the private sector.

#### More Info:

* Multiple plugins available to implement responsible GIS including plugins for [data protection](https://plugins.qgis.org/plugins/GeoPriv/), [differential privacy](https://plugins.qgis.org/plugins/differential\_privacy/#plugin-about), and [normalization](https://plugins.qgis.org/plugins/area\_weighted\_average/).
* QGIS has support for approximately [7,000 known CRSs](https://docs.qgis.org/3.34/en/docs/user\_manual/working\_with\_projections/working\_with\_projections.html).
* Forms a part of [OsGeoLive](https://live.osgeo.org/en/index.html), a self contained open source GIS solution that "allows you to try a wide variety of open source geospatial software without installing anything."

### ArcGIS

<mark style="background-color:blue;">Great for those looking for an all-in-one enterprise level tool</mark>

ArcGIS is a suite of GIS software developed by Esri, designed to facilitate the creation, management, analysis, and sharing of geographic information across various industries. This platform includes applications such as ArcGIS Pro for spatial data management and analysis, ArcGIS Online for cloud-based mapping, and ArcGIS Enterprise for secure, scalable geospatial applications. Additional specialized tools like ArcGIS Field Maps and ArcGIS StoryMaps enhance field operations and storytelling with maps, respectively.&#x20;

#### More Info:

* Esri UK has [committed to halve greenhouse gas emissions and reach net-zero emissions before 2030](https://www.esriuk.com/content/dam/distributor-restricted/esriuk-com/legal/carbon-reduction-plan/esri-holdings-carbon-reduction-plan-2021.pdf).&#x20;
* Coordinate systems: Supports over [2,000 systems](https://desktop.arcgis.com/en/arcmap/latest/map/projections/pdf/geographic\_coordinate\_systems.pdf).
* Esri has recently developed the experimental "[Geospatial Virtual Data Enclave](https://www.esri.com/about/newsroom/arcnews/dealing-with-geoprivacy-and-confidential-geospatial-data/)" aimed at facilitating the work of those who need to share yet protect their data.

### [**CARTO**](https://cartodb.com)&#x20;

<mark style="background-color:blue;">Great for those looking for a custom solution.</mark>

CARTO, is a cloud-based platform that provides GIS and web mapping tools for display in a web browser. It allows users to store, manage, and analyze spatial and non-spatial data. CARTO is designed to make complex spatial data more accessible and actionable for businesses, researchers, and governments. The platform supports various forms of data visualization, such as maps, charts, and tables, enabling users to discover and extract insights from large datasets.&#x20;

**More info:**

* [Coordinate systems](https://github.com/Vizzuality/CartoDB-Tutorials/blob/master/drafts/projections.md): Converts and stores all geometries in WGS84. For Google Maps or Leaflet, they use a different projection called Web Mercator.&#x20;

### [**Mapbox**](https://mapbox.com)&#x20;

<mark style="background-color:blue;">Great for those looking for a custom solution.</mark>

Mapbox provides mapping, location, and spatial analysis tools to developers, businesses, and organizations. It offers a variety of services that enable users to create custom maps and applications with live location data. Mapbox's tools are built on open source software and use data from multiple sources, including their own data collection and contributions from users. The platform is designed to be flexible and scalable, supporting everything from small projects to enterprise-level solutions. Mapbox emphasizes user privacy.

**More info:**

* [Coordinate systems](https://docs.mapbox.com/help/glossary/projection/): Mapbox Tiling Service and Mapbox SDKs for mobile and web accept GeoJSON that follows the GeoJSON standard for a geographic coordinate reference system equivalent to OGC:CRS84, using the WGS84 datum, decimal degrees, and longitude and latitude units (in that order). The Mapbox Uploads API accepts data inputs in a variety of formats and projections.

### [Felt](https://felt.com/)

<mark style="background-color:blue;">Great for those looking for a tool that's easy to use for non-experts.</mark>

Felt GIS is an innovative mapping platform designed to simplify the process of creating, sharing, and collaborating on maps. With a user-friendly interface and a focus on real-time collaboration, Felt enables users from various disciplines to effortlessly integrate geographic data into their projects. Whether for urban planning, environmental monitoring, or community engagement, Felt offers tools that make it easy to visualize complex data and draw meaningful insights. Its intuitive design and powerful functionality are geared towards democratizing GIS, making it accessible to both GIS professionals and novices alike, fostering a more collaborative approach to understanding and solving spatial challenges.

#### More info:

* Felt [will assume coordinates to be in latitude & longitude](https://feltmaps.notion.site/Uploading-Raster-Data-Imagery-c48cab7ff4474ff79a3456fdf022c5df#e8d03d8b85074e7cb6314383b8990c04) (when inside bounds) or Webmercator meters if it cannot find the coordinate system in the metadata. However, [UTM are not supported](https://feltmaps.notion.site/Troubleshooting-Data-Problems-61200a1a54c4489985662412e6b26efa#7d93dad58f3d4eeb8673b84e7ae65247).
* Support [many file formats up to 5GB](https://feltmaps.notion.site/Upload-Anything-b26d739e80184127872faa923b55d232#5dbefc7982d84fc6ac715a16739d4c24) in size.
* Can be [connected to QGIS](https://feltmaps.notion.site/Add-to-Felt-QGIS-Plugin-929f5952745a483e84f5ae814e9e20f4) for online maps.



### Other

* [MaskMy.XYZ](https://maskmy.xyz/) helps users perform a well-known geographic mask from scientific literature, known as donut masking.
