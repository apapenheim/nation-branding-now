---
title: Administrative Divisions
---

This guide will help you find records for administrative units that are not quite states within *NBN*.

# Making Sense of Statoids

Counties, cantons, councils, communes, cities, castelli... subnational entities can be heterogeneous to a point seeming to elude all possibility of systemic order.<sup>[1]</sup> *NBN* treats the [Global Administrative Unit Layers (GAUL)](http://www.fao.org/geonetwork/srv/en/metadata.show?id=12691) data product from the Food and Agriculture Organization of the United Nations and [Core Geo-Database](http://ungiwg.org/coreDB) of the United Nations Geographic Information Working Group as sources of best information in determining both the **level** and **boundaries** of these administrative divisions.

## Administrative Levels

Just as countries are subservient to a [continent-based geoscheme](continent-coding.html), these administrative divisions are subservient to their [respective states](country-classification.html). Administrative divisions differ, however, in that one may frequently be wholly contained within another. For purposes of clarity, it is not sufficient to refer to these levels of administration with colloquial labels such as "county-level" or "departmental-level," as such a designation can convey a degree of delegated authority not necessarily comparable or applicable between countries. As a result, *NBN* adopts FAO convention and describes such divisions as sequential **administrative levels**. To illustrate this, here is a case from France <img src="/images/FlagKit/EU/FR/FR.png" class="flagkit">:

| Example | Localized Administrative Unit Name | NBN Subdivision Descriptor |
| :---: | :---: | :--- |
| Provence-Alpes-Côte d'Azur | *région* | **Primary** administrative level |
| Alpes-Maritimes | *département* | **Secondary** administrative level |
| Nice | *arrondissement* | **Tertiary** administrative level |
| Beausoleil | *canton* | **Quaternary** administrative level |
| Villefranche-sur-Mer | *commune* | **Quinary** administrative level |

Administrative levels offer a **clear**, **precise**, and **neutral** method to catalogue constituent units of states. Branding and identity projects of the nature described on *NBN* tend to fall under the exclusive competency of one such unit. For example, any material relating to *l'office de Tourisme de Villefranche-sur-Mer* is entered into the "Records" column on the Villefranche-sur-Mer's **quinary** page. While a *charte graphique* from the *Conseil général des Alpes-Maritimes* would also very much pertain to and see usage within Villefranche-sur-Mer, it should be placed on the **secondary** page for Alpes-Maritimes, as it is departmental in application.

The directory structure of *NBN* nests these administrative divisions of differing levels within one another – that is, the `FR` directory for France contains within it a directory for each of the thirteen regions of France, each regional directory contains within it a directory for every département within its territory, and so on.

## Intercommunality 
##### *I.e., records pertaining to multiple aministrative divisions*

#### Placing intercommunal records within the directory structure
Some identities are created for use across multiple administrative divisions at the same level. These are known as **bonding intercommunalities**. To continue using our example from the South of France, the commune of Villefranche-sur-Mer is within the *Métropole Nice Côte d'Azur*, an intercommunal structure containing the City of Nice and environs. It is *not* an administrative division of its own. It is a collaborative effort of 49 different quinary-level communes, but it is coterminus with neither the tertiary Nice arrondissement, nor the secondary Alpes-Maritimes département. [Nonetheless, it developed a brand identity.](http://www.nicecotedazur.org/) 

Cataloguing a record such as this one is not as straightforward as instantiating a listing which very clearly relates to a single administrative division and belongs in said divion's directory. There are two pieces of information needed in this case: the administrative division which is large enough to contain all covered territories, and the administrative divisions which are stakeholders in the brand identity (as well as their administrative level). The Métropole Nice Côte d'Azur is composed of 49 quinary (commune) level administrative divisions. The territory it covers is more expansive than any one quaternary (canton) or tertiary (arrondissement) level of administration. It does, however, fit neatly within the bounds of a secondary (département) level administrative division, Alpes-Maritimes. As the Métropole is larger than the Arrondissement of Nice, it cannot be entered there. Conversely, it is far too narrow in scope to merit inclusion on the state-level page for Metropolitan France <img src="/images/FlagKit/EU/FR/FR.png" class="flagkit">, as well as the regional page for Provence-Alpes-Côte d'Azur. Since the Alpes-Maritimes Department contains all of the territory yet still provides some level of geographic specificity, it should be linked to from the Alpes-Maritimes "Records" column.

> Such projects are catalogued under *the smallest administrative division capable of containing all impacted territories*.

Other identities are employed by authorities in multiple administrative divisions at heterogeneous levels of administration. Such authorities are known as **bridging intercommunalities**. When the sub-division at the highest level of precedence contains within its borders or encircles all relevant subservient territory, the record is placed at the highest order sub-division.

Certain programs resulting in the development of a regional brand identity are the result of a close, collaborative relationship between an administrative division and the central government of its state. These are called **linking intercommunalities**, and their records should be stored in the directory for the relevant subordinate administrative divison, and not that for the state itself.

#### Finding intercommunal records within the catalogue

While the smallest administrative division encompassing all of the effected territories is the proper place to store files pertaining to a bonding intercommunality, and the most senior administrative divison the place to store bridging intercommunalities, it is not always as straightforward to provision *links to* those files on the *NBN* index pages.

Cases like these are to always include a note of the limited regional scope for the aid of the reader. Should one feel it necessary to abrogate these guidelines, always defer to clarity, readability, and ease-of-access.

[← Back to User Guide](../guide.html)

---

<sup>[1]</sup> Duchies, departments, delegations, districts, and divisions are to be covered in a separate article.

---

Page instantiated: 10 July 2017.
Date of last revision: 19 February 2019.