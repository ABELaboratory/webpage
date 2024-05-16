---
title: "Test suite"
description: ""
date: "2024-04-23"
draft: false 
---


<p>To test if the identified remediation tools offer functionalities to fix the identified accessibility issues,
  we’ve built a set of test files, one for each starting format (EPUB 2, EPUB 3, EPUB Fixed Layout, PDF). We
  used these test files to carry out functional tests to assess which functionalities were present in a tool and
  which were missing. In these files, we included all the most recurrent accessibility issues according to our
  analysis of the publisher's provided ebook backlist.</p>
<p>The test suite is composed of   five files:</p>

* an EPUB 2 file, to be used to check the features of the remediation tools that claim to turn inaccessible
      EPUB 2 into accessible EPUB 3. [Download test-suite-epub2.epub](https://github.com/ABELaboratory/publications/raw/main/remediation-test-files/Test-suite-epub2.epub).
* an EPUB 3 file, to be used to check the features of the remediation tools that claim to turn inaccessible
      EPUB 3 into accessible EPUB 3. [Download test-suite-common.epub](https://github.com/ABELaboratory/publications/raw/main/remediation-test-files/Test-suite-common.epub)
* an EPUB 3 with multimedia (audio and video) only. [Download test-suite-multimedia.epub](https://github.com/ABELaboratory/publications/raw/main/remediation-test-files/Test-suite-multimedia.epub)
* an EPUB 3 Fixed Layout, to be used for the remediation workflows from EPUB 3 Fixed Layout to “accessible”
      EPUB 3 Fixed Layout and from EPUB 3 Fixed Layout to EPUB 3 reflowable. [Download Test-suite-multimedia.epub](https://github.com/ABELaboratory/publications/raw/main/remediation-test-files/Test-suite-multimedia.epub)
* a PDF file to be used to test the tools that convert a PDF file into a PDF/UA file or in an EPUB 3 file. [Download Test-suite.pdf](https://rawcdn.githack.com/ABELaboratory/publications/be37c899e3d27dead36725d0d471de45e76de15e/remediation-test-files/Test-suite.pdf)
    </p>
  </li>
</ol>