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

# Projections

<figure><img src="../.gitbook/assets/Wrapping.jpg" alt="Young black man trying to wrap a ball unsuccessfully " width="375"><figcaption><p>Round things and flat things don't mix.</p></figcaption></figure>

Geographic projection systems are methods used to represent the round surface of the Earth on flat maps. Because the Earth is a sphere, it's impossible to show its surface on a map without some distortion of area, shape, distance, or direction. Projection systems help to manage these distortions depending on the purpose of the map. When we turn our round Earth into a flat map, [we alter four key things: shape, size, distance, and direction](https://mgimond.github.io/Spatial/chp09\_0.html#spatial-properties). Each projection method currently available to make a map can only keep one or two of these accurate, but not all at the same time.&#x20;

### **The Web Mercator Projection**

Interactive online maps, like the ones we use on our phones and computers, add another layer of complexity in this area. These maps [use "tiling" to break down the whole world](https://en.wikipedia.org/wiki/Web\_Mercator\_projection) into small, manageable squares for our screens also known as the 'Web Mercator.' This Mercator is different from the one used in traditional, large-scale maps, as simplifications were made for simplicity and speed on the web ([How to Lie with Maps](https://press.uchicago.edu/ucp/books/book/chicago/H/bo27400568.html)). While this projection is useful for browsing maps online, [it's inaccurate when measuring distances or areas](https://gis.utah.gov/blog/2015-12-21-nad83-and-webmercator-projections/) and is [difficult to change](https://www.linkedin.com/in/aaron-maxwell-adams/). (Note: Web Mercator is currently used in Google Earth, Bing, CARTO, OpenStreetMap, and ArcGIS Online.)

### **Why It Matters for Environmental Justice**

Choosing the right map projection is crucial for environmental justice efforts. Accurate maps help ensure fair and equitable resource distribution, environmental planning, and policy-making. For instance, projections that distort land sizes can misrepresent the true scale of a problem, like deforestation or pollution, affecting local communities, particularly those in less affluent regions. Having accurate, fair maps ensures that these issues are seen and treated with the urgency they require.

Historical and contemporary biases are evident in the persistence of the [Mercator projection, which disproportionately enlarges regions in the Northern Hemisphere, mainly Europe and North America, at the expense of countries in the Global South](https://sites.lsa.umich.edu/qmss/2022/06/14/why-your-view-of-the-world-may-be-completely-wrong/). This distortion not only reflects but also perpetuates imperialist and Eurocentric narratives, underscoring the projection's ethical quandaries.

### **Guidance on Selecting the Right Projection**

Selecting the right projection depends on the map’s purpose. For local-scale projects, it's important to choose projections that accurately reflect land shapes and sizes to avoid misrepresenting the geographical context. For global maps, one might choose projections that balance between distortions across various dimensions. Always consider the audience and purpose: is the map for navigation, statistical representation, comparative studies, or educational purposes? Consulting with a GIS professional can also help in making informed decisions about which projection to use for your specific needs.

\


{% hint style="info" %}
**Acknowledgments**: [Aaron Adams](https://www.linkedin.com/in/aaron-maxwell-adams/)

**Art:** [Fanesha Fabre](https://www.faneshafabreart.com/)
{% endhint %}
