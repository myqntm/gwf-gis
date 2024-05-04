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

# Privacy Considerations

Privacy-enhancing methods refer to the strategies and technologies designed to protect personal data and maintain the confidentiality of the locations and individuals involved in environmental datasets. These methods help mitigate the risks of unauthorized data access and ensure that sensitive information is not exploited or misused.

However, as [Solymosi, et al](https://app.gitbook.com/o/Nam0YGMZovCTZKyp9wxc/s/WqDPSxrYf8fkp1NrCRXh/)[ ](https://kth.diva-portal.org/smash/get/diva2:1781428/FULLTEXT01.pdf)shared, "violations of geodata privacy are not necessarily through disregard for ethical practice, but rather lack of knowledge or information. For instance, such violations can happen in cases where the data may be believed to be anonymised."

### **The Methods**

Several key methods are commonly employed to enhance privacy in GIS:

* [**Differential Privacy**](https://www.cerias.purdue.edu/news\_and\_events/events/security\_seminar/details/index/j9cvs3as2h1qds1jrdqfdc3hu8) Differential privacy is a technique used to protect the privacy of individual data within a dataset by adding "noise". Imagine you have a jar full of multicolored marbles, each color representing a person's private information. Differential privacy works by adding a few random marbles into the jar. This way, if someone tries to find information about a specific color (or person), the extra marbles make it difficult to be sure whether the information they see comes from the original marbles or the added ones. [Local differential privacy adds noise to individual data points, and global differential privacy adds it to the outputs. ](https://medium.com/secure-and-private-ai-writing-challenge/introducing-local-and-global-differential-privacy-7ae9edea57c9)
* **Location Obfuscation** Obfuscation reduces the precision of location data, reporting locations within a certain radius rather than exact coordinates similar to when we say we're in the town square instead of the bakery.
  * [**GeoMasking**](https://www.youtube.com/watch?v=TCYy-\_vvFQk) This technique involves altering the actual geographic coordinates of a location. The modification can include adding random noise or shifting the coordinates by a certain distance.
  * [**Spatial Cloaking**](https://link.springer.com/referenceworkentry/10.1007/978-0-387-35973-1\_136): This technique hides the exact location by providing a larger area where the individual might be, making it harder to pinpoint the exact location.&#x20;
* **K-Anonymity** K-anonymity ensures that each individual's data is indistinguishable from at least $$𝑘−1k−1$$ other individuals. In simpler terms, imagine you have a group of people, and you're looking at their data. If your dataset is 3-anonymous, this means that any details you can see about one person could apply to at least two other people in the group. There are [two common ways to achieve this](https://en.wikipedia.org/wiki/K-anonymity):&#x20;
  * **Suppression**: For example, substituting all names with an asterisk.
  * **Generalization**: For example, substituting all ages with an age range category.
* **Aggregation**: Using the data to build an aggregate measure which retains the important information. For example, "in their work aggregating individual-­level registered data in Sweden, Andersson and Malmberg (2015) created individualised neighbourhoods (also called ‘egohoods’ or bespoke neighbourhoods) by expand- ing a buffer around a specific location." ([Solymosi, Buil-Gil, Ceccato](https://kth.diva-portal.org/smash/get/diva2:1781428/FULLTEXT01.pdf))

### **Why It Matters for Environmental Justice**

Privacy in GIS is crucial for environmental justice because it protects the identities and locations of individuals and communities who might be at risk of retaliation or discrimination for their environmental advocacy. Ensuring privacy helps maintain trust between civil society organizations and the communities they serve, encouraging more open sharing of crucial data needed for advocacy and protection efforts.

### **Guidance for Your Own Use**

For organizations looking to implement privacy-enhancing methods in GIS, consider the following steps:

* **Assess Your Data**: Understand what data you have and identify any sensitive information that requires protection.
* **Choose Appropriate Methods**: Select privacy methods that best fit your data type and the sensitivity level of the information.
* **Train Your Team**: Educate your staff and volunteers on the importance of privacy and how to apply these methods in their daily work.
* **Regularly Review and Update**: As technology and privacy threats evolve, regularly review and update your privacy practices to ensure they remain effective.

{% tabs %}
{% tab title="To Locate or Not to Locate" %}
The Biden administration has been providing the Israeli government with the locations of humanitarian groups in Gaza, including GPS coordinates of medical facilities and movements of aid organizations. This effort was intended to prevent accidental strikes on these facilities amid ongoing conflicts. However, despite these precautions, Israel has continued to strike such sites, raising concerns about the safety and security of humanitarian operations.

Amid escalating aerial bombardments in Gaza, aid groups sought additional means to communicate their locations, reaching out not only through the United Nations' Humanitarian Notification System (HNS) but also directly to U.S. officials and members of Congress. This system, which was also utilized during the 2014 conflict, aims to protect civilian sites by informing all parties involved in the conflict, including non-state actors. Unfortunately, this year has seen an unprecedented number of U.N. aid workers killed in Gaza, underscoring the severe risks and challenges faced by humanitarian personnel in conflict zones.\
\
Via [Politico](https://www.politico.com/news/2023/11/21/u-s-has-sent-israel-data-on-aid-group-locations-to-try-to-prevent-strikes-00128336)
{% endtab %}

{% tab title="Protecting Nature" %}
iNaturalist, a well-regarded citizen science platform, has been pivotal in recording diverse wildlife observations globally, from birds to plants and beyond. However, with widespread data sharing, a critical challenge emerged: protecting endangered species from potential threats such as poaching.

As enthusiasts shared detailed locations and images of rare species on iNaturalist and other platforms like eBird, the risk of these species being targeted by poachers increased. This was especially true for species whose locations or unique traits made them vulnerable to illegal trade.

**Response:** In response to this threat, iNaturalist started to hide location data for endangered animals in 2011, a strategy later adopted by eBird in 2017. eBird's overhaul included features that allowed data of protected species to be visible only to the person who entered it and the eBird data review team, but not to the public. This ensured that sensitive information was shielded, even though the platforms were inherently designed for open data sharing.

**Outcome:** These adjustments aimed to strike a balance between the benefits of citizen science—educating the public and advancing scientific knowledge—and the necessity of protecting vulnerable species. The hiding  of specific data points helped reduce the risk of poaching, though it also meant that some of the value of sharing precise data was lost.

Via [Slate](https://slate.com/technology/2019/04/superbloom-california-nature-internet-collide-birds-poaching-science.html)
{% endtab %}
{% endtabs %}
