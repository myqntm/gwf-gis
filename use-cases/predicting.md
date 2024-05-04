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

# Predicting

GIS can also support environmental justice advocates in forecasting environmental impacts and vulnerabilities. By analyzing historical data and current trends, GIS can model potential future scenarios, such as the spread of pollution or the impact of flooding on specific populations. This can enable communities to prepare for environmental effects before they occur.&#x20;

### GeoAI

GeoAI, or Geographic Artificial Intelligence, goes even deeper than traditional prediction algorithms and combines AI technologies such as machine learning and deep learning with geographic data and analysis. This allows for advanced processing and interpretation of spatial data, mapping support, and environmental monitoring. For example, we can use geoAI to [trace the outlines of an area](https://mapscaping.com/podcast/ai-autocomplete-for-qgis/) or [support us when creating maps](https://mediaspace.esri.com/media/t/1\_c1ftfyju).

However, Hugo Powell from immap notes that while GeoAI has strong potential for preparatory phases, its deployment in emergency situations can be challenging. A single neural network may not be universally applicable, as building structures vary greatly between different contexts. In such cases, relying on human judgment and intervention might be more effective." ([Mapscaping Podcast](https://mapscaping.podbean.com/e/what-is-humanitarian-gis/))



{% tabs %}
{% tab title="Humanitarian Aid" %}
Forecast-based Action (FbA) represents a transformative shift in delivering humanitarian aid by employing risk and threat analysis to predict and prepare for emergencies before they occur.

In regions like Sudan, the lack of current maps complicates the task of identifying high-risk populations affected by armed conflicts, natural disasters, and other threats such as malnutrition and disease. Access to updated geospatial data is important for implementing FbA effectively and for supporting broader climate adaptation initiatives and emergency responses.

**Solution: The Missing Maps Project** Established in 2014 by organizations including the American Red Cross, British Red Cross, Humanitarian OpenStreetMap Team, and Médecins Sans Frontières, the Missing Maps project aims to provide free mapping services to humanitarian organizations globally. This initiative enhances the availability of up-to-date maps, facilitating better planning and execution of aid.

**Methods:**

The project involves detailed mapping of risk factors on separate layers:

* **Conflict Layer**: This includes data on recurrent combat and identifies areas most affected by conflicts from 2000 to 2021.
* **Natural Hazard Layer**: Contains information on regions prone to floods and droughts.
* **Vulnerability Layer**: Covers critical data on food security, medical care availability, educational facilities, and locations of internally displaced persons and refugees.

Using open-source mapping tools and Esri’s OpenStreetMap feature layers, these data sets are analyzed through a weighted overlay process. Expert-assigned weights help in creating multi-hazard hotspot maps that pinpoint areas with compounded risks.

Via [Esri](https://www.esri.com/about/newsroom/arcuser/sudan-aid/)
{% endtab %}

{% tab title="Disease Spread" %}
The COVID-19 pandemic introduced new dynamics into the realm of big data, particularly highlighting the increased self-production of data and the profound divide between data managers and the individuals who contribute their personal data while bearing the consequences. Amidst the pandemic, remote working conditions enabled academics and volunteers to contribute significantly to data-centric projects, often as a means of giving back to the community while gaining recognition. Notable among these initiatives was the Corona Map project, which leveraged user-submitted data to track and map COVID-19 cases, recoveries, and deaths across 181 countries. This project utilized an automated form that combined personal data with a series of yes/no questions to estimate a user's infection risk. However, this process raised ethical concerns as it automatically published individual data on a global map without users’ explicit consent, spotlighting issues of privacy and autonomy in data use.

In a more controlled environment, the Indian government introduced the Aarogya Setu app, employing Bluetooth technology to monitor and trace interactions between individuals to assess potential COVID-19 infection risks. When the app detects a new positive case, it notifies the authorities about all the contacts made by the infected individual, effectively placing substantial control over personal data in the hands of the state. This approach has been met with criticism from various quarters, including the Internet Freedom Foundation, which voiced concerns about the potential infringement on individual privacy. Moreover, legal experts and rights groups highlighted broader systemic issues, such as the manipulation of data and unequal access to technology, particularly smartphones, which could limit the representation and participation of less privileged populations. These developments underscore a pressing need for a more just approach to information-based aid, one that ensures all individuals have the autonomy to decide whether to share their data or partake in aid, challenging the colonialist structures that historically dictate the distribution and control of aid. This paradigm shift is crucial for dismantling the oppressive structures that diminish individual agency and perpetuate inequality in the data-driven landscape of global health.

Via [GenderIT](https://genderit.org/articles/data-maps-and-colonialism-times-pandemic)
{% endtab %}
{% endtabs %}

