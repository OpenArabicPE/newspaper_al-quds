---
title: "newspapers_al-quds: read me"
author: Till Grallert
date: 2017-05-17 11:40:05 +0200
---

This repository contains bibliographic metadata for the newspaper *al-Quds* published by Jirjī Ḥabīb Ḥanāniyā in Jerusalem between 1908 and 1914. The Center for Palestine Studies at Columbia University scanned issues 1 to 391 and put them [online](http://www.palestine.mei.columbia.edu/alquds-issues/2017/3/9/al-quds). Currently these issues can only be accessed through their issue number and nested sub pages. I therefore began producing machine-actionable bibliographic metadata including volume and issue numbers, as well as dates in all three calendars mentioned in the paper's masthead.

# current state

- 2017-05-16: Issues #1 to #110 are now available
- 2017-05-17: Issues #111 to #200 are now available

# some technical details

This repository contains a single [TEI XML][source] file containing one `<biblStruct>` for each issue. This file is produced through automatic iteration making use of [this code](https://www.github.com/OpenArabicPE/generate_metadata-through-iteration) and manual validation against the digital facsimiles.

The TEI is then [automatically converted](https://www.github.com/OpenArabicPE/convert_tei-to-mods) to [MODS XML][mods] for integration into reference management software etc (such as Zotero).

# notes on the digital facsimiles

- errors
    - The purported scan of [#142](http://www.palestine.mei.columbia.edu/alquds-issues/2017/2/21/issue-142) is indeed a duplicate of [#141](http://www.palestine.mei.columbia.edu/alquds-issues/2017/2/21/issue-141)
    - No file displayed for [#168](http://www.palestine.mei.columbia.edu/alquds-issues/2017/2/21/issue-168), [#170](http://www.palestine.mei.columbia.edu/alquds-issues/2017/2/21/issue-170). Instead these pages show "Hello world".
    - The right side of page 3 of [#45](http://www.palestine.mei.columbia.edu/alquds-issues/2017/2/21/issue-45), [#49](http://www.palestine.mei.columbia.edu/alquds-issues/2017/2/21/issue-49) has been cut off making the first column illegible.

[source]: tei/al-quds.TEIP5.xml
[mods]: metadata/al-quds.MODS.xml