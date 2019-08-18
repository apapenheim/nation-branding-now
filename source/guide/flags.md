---
title: Flags
---


In navigation of *NBN*, one will come across numerous signalling devices taking on the appearance of flags, such as: national flags, international flags, house-made identification aids, and vexilloids. This page will assist the reader in making sense of what they see, as well as provide guidance on selecting flags for incorporation into the project.

## FlagKit

*NBN* utilizes a house-made fork of the [FlagKit](https://github.com/madebybowtie/FlagKit) project by [Bowtie](http://bowtie.se/) of Sweden <img src="/images/FlagKit/EU/SE/SE.png" class="flagkit">.

#### What is FlagKit?

FlagKit is a repository of graphic assets, offering over 250 national flags as icons for use in projects. The whole set is available under the [MIT License](https://github.com/madebybowtie/FlagKit/blob/master/LICENSE). *It is good stuff, why not check it out?*

#### What did we change?

While FlagKit is commendably comprehensive in coverage and offers suitable breadth, it was not produced with the depth of *NBN* in mind. Our expansion of FlagKit includes flags of sub-national administrative divisions, the flags of international organizations, and certain less-than-official identifiers. Our flags are also under made available MIT License, so go ahead: modify and distribute away!

## Flags Representing an Area or Organization

### National Flags

In terms of storage, national flags follow [the same hierarchical structure as continents](continent-coding.html).

### Administrative Divisions

Some administrative divisions of larger states have their own vexillological tradition, and *NBN* intends to honour that. As an example, this project hosts a full set of flags for the Mexican <img src="/images/FlagKit/NA/MX/MX.png" class="flagkit"> states :

![Thumbnails of flags from Mexican states](/images/guide/mx_thumbs.jpg)

Other regions do not customarily identify themselves with flags. In such cases, the "Flag" field can populated either with a null example <img src="/images/FlagKit/NULL.png" class="flagkit">, or a set of house-made geographical icons in FlagKit style can be developed. For a case of such geographical icons in use, see the administrative divisions of Québec <img src="/images/FlagKit/NA/CA/QC/QC.png" class="flagkit"> :

![Thumbnails of maps of Québec administrative regions](/images/guide/qc_thumbs.jpg)

If a regional flag is documented to be used or acknowledged by a recognized and legitimate government, either regional or national in scope, *avoid custom icons and defer to an official representation*.

### Less-than-official Identifying Markers

In some cases, the flag of a piece of territory depends largely upon who one asks. An administrative division with a flag in widespread, customary use may lack any sort of official recognition for such a device. While *NBN* derives strength from deference to the most authoritative sources available, that must be reconciled with a mission statement of accurately representing the identity of a place and its people. In many areas, an unofficial banner serves an important, fundamentally definitive role. In that spirit, certain unofficial devices are not only permitted, but **encouraged** within the project.

## Flags Aiding in Classification

*NBN* optionally supports folkscanomy through category flagging with "CatFlags." As an entirely voluntary process, not all records on NBN will have tag information denoted with CatFlags. If you would like to assist in tagging records, consider submitting a pull request on the relevant index page.

While by no means professing to be a perfect system of categorization, the tagging of identity projects is intended to allow the reader to discern the purpose of a branding effort at-a-glance. In making a categorization on a branding project, it is helpful to look at *which agency it came from* and *the substance of the materials the identity is applied to*.

| CatFlag | Description |
| :-----: | :-----: |
| ![01](/images/guide/catflag_01.png) | Governmental Identification `(/images/cat_flags/01.png)` |
| ![02](/images/guide/catflag_02.png) | Tourism `(/images/cat_flags/02.png)` |
| ![03](/images/guide/catflag_03.png) | Political, primarily associated with a party or a person `(/images/cat_flags/03.png)` |
| ![04](/images/guide/catflag_04.png) | Economic Development `(/images/cat_flags/04.png)` |
| ![05](/images/guide/catflag_05.png) | Something Else `(/images/cat_flags/05.png)` |

## Best Practices
* Make every effort to adhere to FlagKit v1 style. *NBN* assets are forked from [FlagKit v1.1.1](https://github.com/madebybowtie/FlagKit/releases/tag/v1.1.1), and Sketch files are available in the release package on the FlagKit repo.
* Respect the graphic standards and/or construction documents of the most authoritative source available. A government's web presence is good, while a ratified instrument of legislation is better.
* Some highly complex flags do not minify particularly well. One is welcome – but not strictly required – to simplify complicated graphic elements in order to improve graphics at small sizes. Refer to the pre-constructed examples in the FlagKit sketch file for guidance in reducing the number of points in complex shapes.
* When in doubt, go without. The null flag <img src="/images/FlagKit/NULL.png" class="flagkit"> is located at `/images/FlagKit/NULL.png`
* With respect to quasi-official signalling devices: **No passion projects.**

[← Back to User Guide](../guide.html)

---

Page instantiated: 11 October 2018.
Date of last revision: 12 October 2018.