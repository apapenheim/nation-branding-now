---
title: Continent Coding
---

# Continent Coding

This guide will help you locate and create geopolitical entity entries within *NBN*.

## Basic Geoscheme

When working with regions of the world, a clarification of terms is in order. The continental scheme .<sup>[1]</sup> While the continental scheme is a physical and cultural construct, that construct is nonetheless important. *NBN* is a political atlas, not a geological one.

The highest order of classification on *NBN* is by macro-geographical region, arranged – to the extent possible – by continent. High-level directories in this repository are named following two-letter **continent codes**:

| Code  | Continent     |
| :---: | :------------ |
| `AF`  | Africa        |
| `AN`  | Antarctica    |
| `AS`  | Asia          |
| `EU`  | Europe        |
| `NA`  | North America |
| `OC`  | Oceania       |
| `SA`  | South America |

The United Nations Statistics Division (*UNSD*) [M.49 coding classification](https://unstats.un.org/unsd/methodology/m49/) provides the seven-continent geoscheme utilized in this project. When in doubt, you can locate territories based on the UN standard. While countries are grouped into regions based on the M.49 classification, the alphabetical codes used to refer to each continent within *NBN* are inherited from the [International Astronomical Union Working Group for Planetary System Nomenclature](https://planetarynames.wr.usgs.gov/Abbreviations), rather than the numeric codes found in M.49. The reason for this departure from standard is to harmonize the region coding protocol used on *NBN* with that already widely in use at the [Datasets Project](https://github.com/datasets/continent-codes), the [GeoIP PHP Extension](http://php.net/manual/en/function.geoip-continent-code-by-name.php), the [GeoNames Project](http://download.geonames.org/export/dump/readme.txt), and in <a href="https://en.wikipedia.org/wiki/List_of_sovereign_states_and_dependent_territories_by_continent_(data_file)">Wikipedia's categorization scheme</a>. 

> Note for contributors: The implementation of and adherence to the M.49 standard is a deliberate choice. Avoid originating new folders bearing continent codes from the root directory, as well as the merging of existing folders. While there may be instances in which, for the sake of clarity, individual territories or organizations receive special accommodations (see below), the seven-continent scheme in place is a valuable and useful one for the purposes of this project.

## Special Cases

### International Organizations

Global governance is not strictly confined to arbitrary landmass divisions. Intergovernmental organizations with an international membership, scope, or presence require a bit more work to pin down. Some IOs, such as *MERCOSUR* or the *SAARC*, have membership exclusively within one of the seven coded divisions listed above. Entries for such organizations are placed within one of the above sub-directories and referenced in the Records listing of said continent's index file.

What about organizations with jurisdiction and membership reaching beyond (ex: the *UN*) or between (ex: the *OAS*) continents? Such entities are categorized separately, accessible from the home page via the [Worldwide](../WW.html) link, and relevant records are stored in a special directory:

| Code  | Classification  |
| :---: | :-------------- | 
| `WW`  | Worldwide (IOs) |

### Transcontinental Countries

Some territories have boundaries either transversing continental divides, or have classifications subject to dispute. To create a clear and user-friendly system of organization, some states may be listed in more than one region. While the *repository architecture* should always adhere as closely as possible to UN M.49 coding, it is sometimes appropriate to place state-level redirects within other continental indices.

#### Contiguous territory test

> The sun never sets on the British Empire, but the United Kingdom <img src="/images/FlagKit/EU/GB/GB.png" class="flagkit"> is in Europe.

Avoid creating redirects for countries as a consequence of their *non-contiguous* overseas territories, including exclaves operating with irregularly limited or expanded competencies. These entities should be referenced with an independent listing ([if appropriate](country-classification.html#dependent-and-specially-administrated-territories)) or as a sub-division of the listing for the state which the area depends upon. For example: The overseas collectivity of Wallis-et-Futuna <img src="/images/FlagKit/OC/WF/WF.png" class="flagkit"> can be represented in the `OC` index, but Metropolitan France <img src="/images/FlagKit/EU/FR/FR.png" class="flagkit"> should not.

As Egypt <img src="/images/FlagKit/AF/EG/EG.png" class="flagkit"> controls *mainland* territory on both sides of the Isthmus of Suez, links to the country appear on both the `AF` and `AS` index pages. Per its UN M.49 classification, however, Egypt's content is only to be stored in the African directory `/AF/EG/*`

The following countries pass the contiguous territory test and are, on that basis, approved for a cross-category linkage:

| Flag  | Name  |
| :---: | :---- |
| <img src="/images/FlagKit/AF/EG/EG.png" class="flagkit"> | Egypt |
| <img src="/images/FlagKit/EU/RU/RU.png" class="flagkit"> | Russian Federation |
| <img src="/images/FlagKit/AS/TR/TR.png" class="flagkit"> | Turkey |

#### The boundary between Europe and Asia

This project accepts a more permissive classification of what may be labelled a "European" country than does the UNSD. Any country excluded from Europe in M.49, but which has [completed accession to the Council of Europe](http://www.coe.int/en/web/portal/47-members-states) is eligible to have a redirect placed on `/EU/README.md`. 

For example, the nation of Cyprus <img src="/images/FlagKit/AS/CY/CY.png" class="flagkit"> is considered (under M.49) to be in West Asia. Records for the country are stored at `/AS/CY/`. However, the Council of Europe counts the island nation among its member states. As readers may then expect to find an entry for Cyprus at the `EU` index, it is permissible to include a redirect to `/AS/CY.html` within the aforementioned file.

The following countries coded to Asia have completed accession to the Council of Europe and are, on that basis, approved for a cross-category linkage:

| Flag  | Name  |
| :---: | :---- |
| <img src="/images/FlagKit/AS/AM/AM.png" class="flagkit"> | Armenia |
| <img src="/images/FlagKit/AS/AZ/AZ.png" class="flagkit"> | Azerbaijan |
| <img src="/images/FlagKit/AS/CY/CY.png" class="flagkit"> | Cyprus |
| <img src="/images/FlagKit/AS/GE/GE.png" class="flagkit"> | Georgia |
| <img src="/images/FlagKit/EU/RU/RU.png" class="flagkit"> | Russian Federation |
| <img src="/images/FlagKit/AS/TR/TR.png" class="flagkit"> | Turkey |

#### Island States

As island states lack contiguous territory on a continental landmass, they may at times elude classification by the test outlined above.

| Flag | Name  |
| :--: | :---- |
| <img src="/images/FlagKit/OC/CX/CX.png" class="flagkit"> | Christmas Island |
| <img src="/images/FlagKit/OC/CC/CC.png" class="flagkit"> | Cocos (Keeling) Islands |
| <img src="/images/FlagKit/NA/GL/GL.png" class="flagkit"> | Greenland |

#### Antarctica and Outlying Islands

As an area populated only by research scientists is of little-to-no relevance for population statistics, the United Nations geoscheme opts not to classify countries within the Antarctica region.<sup>[2]</sup> Sovereign claims to all lands and ice shelves south of 60 degrees south latitude are held in abeyance under Article IV of the Antarctic Treaty and such claims may be maintained, but not enforced. Brand identity assets from any and all sovereign state claims – treated by the originating state as non-integral territory and based on activities occuring prior to 1961 – are to be stored, commingled and without prejudice to claimants with overlapping territorial claims, within a sub-directory labelled with the ISO 3166-1 code for Antarctica: `AQ`.

*NBN* employs a broader definition of the Antarctic area for the purposes of continental classification, asserting that all territories primarily devoted to scientific research and conservation south of the [Antarctic Convergence](https://www.grida.no/resources/5505) share more in common with one another and the lands governed by the Antarctic Treaty than any other region. In broadening its definition, *NBN* opts to extend classification to all entities within the Convention Area of the [CCAMLR](https://www.ccamlr.org/) as Antarctic territory. This includes several dependent island territories bearing ISO 3166-1 codes. <sup>[3]</sup> While directories for these areas originate from their region of M.49 classification, a redirect is included from the `AN` index to the target directory.

Listed below are the entities contained within the `AN` index:

| Flag | Name  | Redirects to |
| :--: | :---- | :----------: |
| <img src="/images/FlagKit/AN/AQ/AQ.png" class="flagkit"> | Antarctica (Lands and Ice Shelves Below 60° S) | `N/A` |
| <img src="/images/FlagKit/SA/BV/BV.png" class="flagkit"> | Bouvet Island | `SA` |
| <img src="/images/FlagKit/AF/TF/TF.png" class="flagkit"> | French Southern and Antarctic Territories | `AF` |
| <img src="/images/FlagKit/OC/HM/HM.png" class="flagkit"> | Heard Island and McDonald Islands | `OC` |
| <img src="/images/FlagKit/SA/GS/GS.png" class="flagkit"> | South Georgia and South Sandwich Islands | `SA` |

### Complete list of designated transcontinental countries

The following countries have been approved for cross-category linkages. 

| Flag  | Name  |
| :---: | :---- |
| <img src="/images/FlagKit/AS/AM/AM.png" class="flagkit"> | Armenia |
| <img src="/images/FlagKit/AS/AZ/AZ.png" class="flagkit"> | Azerbaijan |
| <img src="/images/FlagKit/SA/BV/BV.png" class="flagkit"> | Bouvet Island |
| <img src="/images/FlagKit/AS/CY/CY.png" class="flagkit"> | Cyprus |
| <img src="/images/FlagKit/AF/EG/EG.png" class="flagkit"> | Egypt |
| <img src="/images/FlagKit/AF/TF/TF.png" class="flagkit"> | French Southern and Antarctic Territories |
| <img src="/images/FlagKit/AS/GE/GE.png" class="flagkit"> | Georgia |
| <img src="/images/FlagKit/NA/GL/GL.png" class="flagkit"> | Greenland |
| <img src="/images/FlagKit/OC/HM/HM.png" class="flagkit"> | Heard Island and McDonald Islands |
| <img src="/images/FlagKit/EU/RU/RU.png" class="flagkit"> | Russian Federation |
| <img src="/images/FlagKit/SA/GS/GS.png" class="flagkit"> | South Georgia and South Sandwich Islands |
| <img src="/images/FlagKit/AS/TR/TR.png" class="flagkit"> | Turkey |

[← Back to User Guide](../guide.html)

___

<sup>[1]</sup> [Lewis and Wigen 1997, pp. 21-46.](http://www.jstor.org/stable/10.1525/j.ctt1pnv6t)
<sup>[2]</sup> [Takle and Vassenden 1998, p. 17.](https://www.unece.org/fileadmin/DAM/stats/documents/1998/03/migration/5.e.pdf)
<sup>[3]</sup> [Rothwell et al. 2012, p. 5.](https://www.routledge.com/9780415620253)

---

Page instantiated: 27 March 2017.
Date of last revision: 19 February 2019.