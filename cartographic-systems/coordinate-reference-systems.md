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

# Coordinate Reference Systems

<figure><img src="../.gitbook/assets/Dog.jpg" alt="" width="375"><figcaption><p>Objects can appear differently depending on where you're sitting.</p></figcaption></figure>

Geographic coordinate reference systems (datums) are frameworks used to precisely map the Earth's curved surface onto a flat map. A datum defines the position of the spheroid relative to the center of the Earth. It provides a reference point for measuring locations on the surface of the Earth in latitude and longitude. These systems can vary because the Earth is not a perfect sphere and has an uneven distribution of mass. Different datums are used based on the region or the needs of the mapping project to ensure that the coordinates are accurate and useful.&#x20;

### What are the Different Types Available?

["In general, CRS can be divided into **projected coordinate reference systems** (also called Cartesian or rectangular coordinate reference systems) and **geographic coordinate reference systems**."](https://docs.qgis.org/3.34/en/docs/gentle\_gis\_introduction/coordinate\_reference\_systems.html) The most commonly used datums include:

* [**WGS 84 (World Geodetic System 1984)**](https://gisgeography.com/wgs84-world-geodetic-system/): Used globally by GPS systems.
* [**NAD 83 (North American Datum 1983)**](https://geodesy.noaa.gov/datums/horizontal/north-american-datum-1983.shtml): Commonly used in North America for geospatial data.
* [**ED 50 (European Datum 1950)**](https://community.esri.com/t5/coordinate-reference-systems-blog/the-european-datum-a-history-part-3/ba-p/902176): Used in Europe before being largely replaced by newer systems.
* [**UTM** **(Universal Transverse Mercator)**](https://docs.qgis.org/3.34/en/docs/gentle\_gis\_introduction/coordinate\_reference\_systems.html#universal-transverse-mercator-utm-crs-in-detail)**:** A global map projection. This means, it is generally used all over the world.

Each datum adjusts for regional variations in the Earth's shape, providing higher accuracy for location data in that specific region. For example, the global model, based on satellite data, can be used for ‘one-size-fits-all’ purposes; it [mainly serves as the foundation for local models](https://desktop.arcgis.com/en/arcmap/latest/map/projections/datums.htm) that aim for greater accuracy. For example, in the UK, the local datum [differs from reality within its border by only 5 meters](https://desktop.arcgis.com/en/arcmap/10.3/guide-books/map-projections/geoid.htm).  This knowledge is essential as you may be faced with having to join two files based on different reference systems and may find that locations don't align. The best GIS platforms may provide  **on-the-fly** projection, which "...means that you can define a certain projection when you start the GIS, and all layers that you then load, no matter what coordinate reference system they have, will be automatically displayed in the projection you defined." ([QGIS](https://docs.qgis.org/3.34/en/docs/gentle\_gis\_introduction/coordinate\_reference\_systems.html#on-the-fly-projection))

### Why It Matters for Environmental Justice

For environmental justice initiatives, using the correct geographic coordinate system and datum is crucial for accurately identifying and reporting issues such as pollution, resource distribution, and environmental impacts on communities. Accurate data ensures that interventions are well-directed and that environmental risks and resources are mapped correctly, which is essential for advocating effectively and ensuring equitable treatment of all communities.

### Selecting a Datum

Selecting the right datum depends on your project's geographic focus and the nature of the data you are working with. Consider these guidelines:

* **Match the Datum to Your Data Sources**: Ensure that all your data sources use the same datum for consistency.
* **Use Local Datums for Regional Projects**: For projects focused on specific regions, use the datum that aligns best with regional geographic nuances.
* **Consult with GIS Professionals**: When in doubt, consult with GIS professionals who can provide guidance based on the latest practices and the specific needs of your project.



{% hint style="info" %}
**Art:** [Fanesha Fabre](https://www.faneshafabreart.com/)
{% endhint %}

## &#x20;
