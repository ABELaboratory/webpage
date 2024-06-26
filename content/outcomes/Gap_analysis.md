---
title: "Gap Analysis"
description: ""
date: "2023-10-30"
draft: false
---

*This deliverable initially published by october 2023 was completed with an addendum on april 2024*

*This HTML page is an extract of the deliverable "Report on Backlist Data and gap analysis" available to download as <a href="https://github.com/ABELaboratory/publications/raw/main/public-deliverables/report-on-backlist-data-and-gap-analysis/Report_on_Backlist_Data_and_gap_analysis.pdf" aria-label="Download PDF Report on Backlist Data and gap analysis">PDF (1.6 mo)</a> or <a href="https://github.com/ABELaboratory/publications/raw/main/public-deliverables/report-on-backlist-data-and-gap-analysis/Report_on_Backlist_Data_and_gap_analysis.epub" aria-label="Download EPUB Report on Backlist Data and gap analysis">EPUB (800 ko)</a>.*
<hr/>

<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page22"
aria-label="Page 22"></span>
</p>

<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page23"
aria-label="Page 23"></span>The objective of this section of the report is to share results on the identification of recurrent accessibility issues per categories of ebooks that will need remediation to fit EAA requirements. We’ll first define the target, our methodology and the scoring threshold established for this analysis, as well as the identified biases and limits. Then we’ll present the results we deemed useful for the next steps of the ABE Lab project, with a list of recurrent accessibility issues detected. Lastly, we’ll define the outcomes of this work and the ebook classification we developed which will be used to test remediation tools and workflows.</p>
<section
id="target">



## Target

<p>
The 
<a
href="https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882">
<u>
<u>
European Accessibility Act (EAA)
</u>
</u>
</a>
<a
href="#fn1"
class="footnote-ref"
id="fnref1"
epub:type="noteref"
role="doc-noteref">
<sup>1</sup>
</a>
requirements for ebooks are listed in 
<a
href="https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882#d1e32-100-1">
<u>
<u>
Annex I
</u>
</u>
</a>
sections III and IV Linea f). 
<a
href="https://www.w3.org/TR/epub-a11y-eaa-mapping/">
<u>
<u>
EPUB Accessibility - EU Accessibility Act Mapping
</u>
</u>
</a>
<a
href="#fn2"
class="footnote-ref"
id="fnref2"
epub:type="noteref"
role="doc-noteref">
<sup>2</sup>
</a>
is a W3C group note that shows how EPUB files conforming to EPUB accessibility guidelines (
<a
href="https://www.w3.org/TR/epub-a11y-11/">
<u>
<u>
EPUB Accessibility 1.1
</u>
</u>
</a>
and 
<a
href="https://www.w3.org/TR/WCAG21/">
<u>
<u>
WCAG 2.1
</u>
</u>
</a>
AA) are responding to the European Accessibility Act requirements. Those two documents help us define our target and basis to establish the accessibility deficiencies. 
</p>
<p>
Pre-paginated ebooks (like PDFs and Fixed Layout EPUBs) do not comply with the EAA requirements for the criterion of 
<i>
flexibility and choice in the presentation of the content
</i>
<a
href="#fn3"
class="footnote-ref"
id="fnref3"
epub:type="noteref"
role="doc-noteref">
<sup>3</sup>
</a>
, a key functionality for persons facing cognitive difficulties (like dyslexia) or with sight impairments. As remediation for these types of ebooks would mean a change of format, we choose to introduce middle-way target remediation to allow the study of remediation to today's format state and possibilities offered by remediation tools. The target for these documents will be compliance with the Web Content Accessibility Guidelines (WCAG) 2.1
<a
href="#fn4"
class="footnote-ref"
id="fnref4"
epub:type="noteref"
role="doc-noteref">
<sup>4</sup>
</a>
. In addition, PDFs will have to reach PDF/UA conformity, a dedicated standard registered as ISO
<a
href="#fn5"
class="footnote-ref"
id="fnref5"
epub:type="noteref"
role="doc-noteref">
<sup>5</sup>
</a>
.
</p>
</section>
<section
id="methodology">


## Methodology
<p>The backlist data analysis allowed us to define a wish list of categories of files to collect in order to represent the backlist composition in a small but consistent sample. We had a target objective of 200 files from 5 countries. This objective was exceeded, with 351 files collected from 7 EU countries (Denmark, Finland, France, Germany, Italy, the Netherlands, Spain), additionally including some samples also from the United Kingdom. We used the Thema codes as our reference for classification. Some provided samples were classified to different Thema categories by the publisher. As it was not possible to separate the Thema categories, we chose to multiplicate these samples (one per Thema code, i.e. a book with Thema codes D, F was analysed two times, one as D and one as F), resulting in a total of 376 units to analyse.</p>
<p>We added to this sample one accessible EPUB3 target file<a
href="#fn6"
class="footnote-ref"
id="fnref6"
epub:type="noteref"
role="doc-noteref"><sup>6</sup></a>, to be sure that the gap emerging from our analysis was fitting the reality and that files already made accessible would not be considered as files with remediation needs. This target file was produced by LIA as born accessible in 2023.</p>
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page24"
aria-label="Page 24"></span>We first established a list of key points indicators (KPI) we wanted to evaluate and from them, we could determine the data to extract from the samples. We verified which of these data were available from existing reporting tools (EPUBCheck, ACE, and RGTK for EPUB files; VeraPDF and PDFIX for PDF files, see annex <a
href="#id__heading=h.st7dyjwk9xkw"><i><u><u>Tools used in the automated analysis</u></u></i></a> for a brief description of these tools) and determined the missing ones. Fondazione LIA developed a script to extract the missing data, aggregate all the data, and export a unified report. The details of the tests are available in the <i>Detailed evaluation of the tests made on ebooks</i> document, available for project partners and contributing publishers. 15 iterations of the script were made to refine data extraction and the exported reports. We started from a large number of data collected to stretch to a minimum necessary point.</p>
<p>The report was then used to develop calculation methods to define remediation complexity indicators<a
href="#fn7"
class="footnote-ref"
id="fnref7"
epub:type="noteref"
role="doc-noteref"><sup>7</sup></a>. Iterations were needed for this step as well, as data visualisation produced helped us identify biases, missings and non-relevant information. The results of the evaluation are presented and commented on within this document.</p>
</section>
<section
id="scoring">


## Scoring
<p>Usually, providers of remediation services classify the ebooks per complexity: a book with more images, tables or pages will get a higher score. This method is relevant if the whole set of ebooks to classify is produced from a known production workflow. Looking at the European level, we know that publishers’ workflows differ in the quality of files they produce, which consequently may be totally different in terms of accessibility features, accessibility information and, therefore, remediation needs.</p>
<p>That is why in this project we established a new classification related to remediation complexity, considering that an ebook may be very complex but already produced in accordance with accepted accessibility standards, thus resulting in a very low remediation complexity score. To be sure that the scoring was truly reflecting the remediation needs, we referred to our target file known to be fully accessible and with no remediation needs. With some iterations on scoring, we made sure that the target got a score of zero.</p>
<p>Capturing remediation complexities in relation to different file formats was one of the main challenges of the process. PDFs and Fixed-layout EPUBs are known to be the most complex to remediate as the technologies and languages used to build them imply more complexities and a higher level of programmatic abstraction. That’s why we decided to represent them apart.</p>
<p>One bias we had to deal with is that PDF format allows for less structure and metadata, resulting in less possibilities for analyses, which resulted in abnormally low scores for files in this format. To address this bias, we had to establish a complementary scoring calculation to apply to these files.</p>
<p>Therefore, each format has specificities related to contents found in the files and accessibility related features missing. To find the correct marker, a threshold of calculated key indicators has been established thru iterations.</p>
</section>
<section
id="identified-limits-and-bias">
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page25"
aria-label="Page 25"></span>
</p>


## Identified limits and bias
<p>As previously commented, files in PDF format do not have the same accessibility possibilities as files in the EPUB format. Therefore, the comparison between the two formats must be done very consciously and should not lead to categorical formulas.</p>
<p>Most of the publishers providing samples are de facto aware of the accessibility subject and therefore the collection we have might be a biased representation of the backlist. A way to verify that would be to do a similar analysis on a large number of files not specifically selected for this type of test. This analysis perspective has been discussed with three members of EDRLab (Beletrina, De Marque and Hachette Livres) and we hope to be able to provide it as a complementary ABE Lab publication in the future.</p>
<p>At the time of writing this report, some remediation needs can not be spotted automatically, but as technological improvements are occurring very fast, we expect that a better gap analysis could be produced in the coming years. Examples of accessibility problems that cannot be automatically detected are incorrect, non-meaningful or insufficient image descriptions and wrong metadata claims, for which we were not able to establish a valid calculation method during this work.</p>
</section>
<section
id="results">
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page26"
aria-label="Page 26"></span>
</p>


## Results
<section
id="per-format"
class="level3">


### Per format
<p>The sample contains 84% (316 files) of reflowable EPUB (RFL); 9% (33 files) of pre-paginated EPUB3 Fixed Layout (FXL) and 7% (26 files) of PDFs. This, actually, does not properly represent any of the market segmentations observed in the backlist data analysis.</p>
<p>The low number of pre-paginated files in the sample limits the analysis pertinence. It may be interpreted as an interest of the publishers providing samples to have accurate analysis on the remediation needs of reflowable EPUB files rather than PDF and EPUB3 FXL files, as many ebooks coexist in both reflowable and pre-paginated formats.</p>
<p>The radar diagram and the data table in the next page show the results of the scoring. We resume here the main trendings per format:</p>
<ul>
<li>
<p>PDF scoring ranges from 29 to 68 with representation in Thema categories A (The Arts), J (Society and Social Sciences), K (Economics, Finance, Business and Management), L (Law, ), M (Medicine and Nursing), P (Mathematics and Science) T (Technology, Engineering, Agriculture, Industrial processes) and V (Health, Relationships and Personal development).</p>
</li>
<li>
<p>EPUB3 Fixed Layout (FXL) average scoring ranges from 24 to 64 with representation in Thema categories A (The Arts,), C (Language and Linguistics), D (Biography, Literature and Literary studies), P (Mathematics and Science), S (Sports and Active outdoor recreation), T (Technology, Engineering, Agriculture, Industrial processes), W (Lifestyle, Hobbies and Leisure), X (Graphic novels, Comic books, Manga, Cartoons) and Y (Children’s, Teenage and Educational) ;</p>
</li>
<li>
<p>EPUB3 reflowable average scoring ranges from 4 to 77 with representation in all Thema categories except X (Graphic novels, Comic books, Manga, Cartoons).</p>
</li>
</ul>
<p>This overview shows a concrete difference in ranges, where reflowable formats are almost all below a score of 50 and pre-paginated formats are all over 50. As commented before, the lack of information provided in PDF files might lead to minoring the remediation complexity. We tried to compensate for that in our scoring threshold, but remediation testing will have to establish if the compensation is enough or misleading.</p>
<p>We also detected that pre-paginated are not represented in every Thema code, while reflowables are missing only for category X: <i>Graphic novels, Comic books, Manga, and Cartoons</i>. This shows that, except for visual narratives, all types of books can be produced in a reflowable format.</p>
<p>From these results, it seems legit to treat remediation of pre-paginated files apart from the reflowable ones. This result will be represented in our remediation classification through the establishment of a first level of complexity related to file format.</p>
<p>
<span
id="id__Toc149567649"
class="anchor"></span>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page27"
aria-label="Page 27"></span></p>
<figure>
<figcaption>Figure 6: Radar chart showing three curves for PDF (blue continuous line), EPUB Fixed-Layout (orange dashed line) and EPUB reflowable (violet dotted line)</figcaption>
<p>
<img
src="/images/media24/file9.jpg" alt=" Radar chart"/>
</p>
</figure>

<p>
<span
id="id__Toc149567629"
class="anchor"></span></p>
<table>
<caption>Table 4: Average score per format (rows) and Thema codes (columns). “-” represents absence of files in the sample collection for given format and Thema category</caption>
<thead>
<tr
class="header">
<th
scope="col">Thema code</th>
<th
scope="col">
<i>
<b>A</b>
</i>
</th>
<th
scope="col">
<i>
<b>C</b>
</i>
</th>
<th
scope="col">
<i>
<b>D</b>
</i>
</th>
<th
scope="col">
<i>
<b>F</b>
</i>
</th>
<th
scope="col">
<i>
<b>J</b>
</i>
</th>
<th
scope="col">
<i>
<b>K</b>
</i>
</th>
<th
scope="col">
<i>
<b>L</b>
</i>
</th>
<th
scope="col">
<i>
<b>M</b>
</i>
</th>
<th
scope="col">
<i>
<b>N</b>
</i>
</th>
<th
scope="col">
<i>
<b>P</b>
</i>
</th>
<th
scope="col">
<i>
<b>Q</b>
</i>
</th>
<th
scope="col">
<i>
<b>R</b>
</i>
</th>
<th
scope="col">
<i>
<b>S</b>
</i>
</th>
<th
scope="col">
<i>
<b>T</b>
</i>
</th>
<th
scope="col">
<i>
<b>U</b>
</i>
</th>
<th
scope="col">
<i>
<b>V</b>
</i>
</th>
<th
scope="col">
<i>
<b>W</b>
</i>
</th>
<th
scope="col">
<i>
<b>X</b>
</i>
</th>
<th
scope="col">
<i>
<b>Y</b>
</i>
</th>
</tr>
</thead>
<tbody>
<tr
class="odd">
<td>
<i>
<b>PDF</b>
</i>
</td>
<td>
<i>66</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>50</i>
</td>
<td>
<i>63</i>
</td>
<td>
<i>57</i>
</td>
<td>
<i>67</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>68</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>73</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>67</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
</tr>
<tr
class="even">
<td>
<i>
<b>RFL</b>
</i>
</td>
<td>
<i>35</i>
</td>
<td>
<i>43</i>
</td>
<td>
<i>30</i>
</td>
<td>
<i>19</i>
</td>
<td>
<i>24</i>
</td>
<td>
<i>37</i>
</td>
<td>
<i>17</i>
</td>
<td>
<i>48</i>
</td>
<td>
<i>26</i>
</td>
<td>
<i>33</i>
</td>
<td>
<i>20</i>
</td>
<td>
<i>50</i>
</td>
<td>
<i>46</i>
</td>
<td>
<i>36</i>
</td>
<td>
<i>35</i>
</td>
<td>
<i>32</i>
</td>
<td>
<i>29</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>32</i>
</td>
</tr>
<tr
class="odd">
<td>
<i>
<b>FXL</b>
</i>
</td>
<td>
<i>62</i>
</td>
<td>
<i>66</i>
</td>
<td>
<i>49</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>61</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>64</i>
</td>
<td>
<i>65</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>-</i>
</td>
<td>
<i>60</i>
</td>
<td>
<i>61</i>
</td>
<td>
<i>50</i>
</td>
</tr>
</tbody>
</table>
</section>
<section
id="focus-on-reflowable-epub3"
class="level3">
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page28"
aria-label="Page 28"></span>
</p>


### Focus on reflowable EPUB3
<p>As reflowable EPUB3 is the format allowing full compliance to the EAA requirements, we judged it essential to dive deeper in the analysis of the remediation complexity of files in this format. In the collected samples files we found scores from 4 to 73 points. The vast majority have a score between 10 and 30.</p>
<p>The following charts and tables give a full representation. We will summarise here the key information we found:</p>
<ul>
<li>
<p>most of the files have a medium remediation complexity, but there is also a good number of files with high scores (fig. 4);</p>
</li>
<li>
<p>images to fix (meaning textual alternatives to establish) are the heaviest error affecting strongly all categories except for L (Laws) and F (Fiction) (fig. 5);</p>
</li>
<li>
<p>most of the categories have a large amplitude of errors per file, meaning that the Thema category alone is not sufficient to establish a segmented average remediation cost (fig. 6).</p>
</li>
</ul>
<p>
<span
id="id__Toc149567650"
class="anchor"></span>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page29"
aria-label="Page 29"></span></p>
<figure>
<figcaption>Figure 7: Bar chart showing the number of files as ordinate by scoring as abscissa.</figcaption>
<p>
<img
src="/images/media24/file10.jpg"
alt="Bar chart showing a bimodal distribution."/>
</p>
</figure>
<p>List data: number of files per score</p>
<ul>
<li>
<p>Score 0: 1 files</p>
</li>
<li>
<p>Score 1: 0 files</p>
</li>
<li>
<p>Score 2: 0 files</p>
</li>
<li>
<p>Score 3: 0 files</p>
</li>
<li>
<p>Score 4: 1 files</p>
</li>
<li>
<p>Score 5: 6 files</p>
</li>
<li>
<p>Score 6: 0 files</p>
</li>
<li>
<p>Score 7: 3 files</p>
</li>
<li>
<p>Score 8: 4 files</p>
</li>
<li>
<p>Score 9: 5 files</p>
</li>
<li>
<p>Score 10: 13 files</p>
</li>
<li>
<p>Score 11: 4 files</p>
</li>
<li>
<p>Score 12: 1 files</p>
</li>
<li>
<p>Score 13: 5 files</p>
</li>
<li>
<p>Score 14: 2 files</p>
</li>
<li>
<p>Score 15: 6 files</p>
</li>
<li>
<p>Score 16: 18 files</p>
</li>
<li>
<p>Score 17: 12 files</p>
</li>
<li>
<p>Score 18: 12 files</p>
</li>
<li>
<p>Score 19: 15 files</p>
</li>
<li>
<p>Score 20: 24 files</p>
</li>
<li>
<p>Score 21: 18 files</p>
</li>
<li>
<p>Score 22: 11 files</p>
</li>
<li>
<p>Score 23: 15 files</p>
</li>
<li>
<p>Score 24: 7 files</p>
</li>
<li>
<p>Score 25: 4 files</p>
</li>
<li>
<p>Score 26: 5 files</p>
</li>
<li>
<p>Score 27: 0 files</p>
</li>
<li>
<p>Score 28: 1 files</p>
</li>
<li>
<p>Score 29: 6 files</p>
</li>
<li>
<p>Score 30: 3 files</p>
</li>
<li>
<p>Score 31: 3 files</p>
</li>
<li>
<p>Score 32: 6 files</p>
</li>
<li>
<p>Score 33: 5 files</p>
</li>
<li>
<p>Score 34: 3 files</p>
</li>
<li>
<p>Score 35: 3 files</p>
</li>
<li>
<p>Score 36: 5 files</p>
</li>
<li>
<p>Score 37: 1 files</p>
</li>
<li>
<p>Score 38: 2 files</p>
</li>
<li>
<p>Score 39: 4 files</p>
</li>
<li>
<p>Score 40: 7 files</p>
</li>
<li>
<p>Score 41: 5 files</p>
</li>
<li>
<p>Score 42: 5 files</p>
</li>
<li>
<p>Score 43: 4 files</p>
</li>
<li>
<p>Score 44: 0 files</p>
</li>
<li>
<p>Score 45: 3 files</p>
</li>
<li>
<p>Score 46: 4 files</p>
</li>
<li>
<p>Score 47: 3 files</p>
</li>
<li>
<p>Score 48: 3 files</p>
</li>
<li>
<p>Score 49: 1 files</p>
</li>
<li>
<p>Score 50: 9 files</p>
</li>
<li>
<p>Score 51: 4 files</p>
</li>
<li>
<p>Score 52: 3 files</p>
</li>
<li>
<p>Score 53: 4 files</p>
</li>
<li>
<p>Score 54: 2 files</p>
</li>
<li>
<p>Score 55: 4 files</p>
</li>
<li>
<p>Score 56: 3 files</p>
</li>
<li>
<p>Score 57: 2 files</p>
</li>
<li>
<p>Score 58: 2 files</p>
</li>
<li>
<p>Score 59: 3 files</p>
</li>
<li>
<p>Score 60: 8 files</p>
</li>
<li>
<p>Score 61: 6 files</p>
</li>
<li>
<p>Score 62: 19 files</p>
</li>
<li>
<p>Score 63: 8 files</p>
</li>
<li>
<p>Score 64: 2 files</p>
</li>
<li>
<p>Score 65: 1 files</p>
</li>
<li>
<p>Score 66: 5 files</p>
</li>
<li>
<p>Score 67: 5 files</p>
</li>
<li>
<p>Score 68: 4 files</p>
</li>
<li>
<p>Score 69: 2 files</p>
</li>
<li>
<p>Score 70: 1 files</p>
</li>
<li>
<p>Score 71: 0 files</p>
</li>
<li>
<p>Score 72: 3 files</p>
</li>
<li>
<p>Score 73: 5 files</p>
</li>
</ul>
<p>
<span
id="id__Toc149567651"
class="anchor"></span>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page30"
aria-label="Page 30"></span></p>
<figure>
<figcaption>Figure 8: Bar chart showing level and repartition of errors per Thema code categories</figcaption>
<p>
<img
src="/images/media24/file11.jpg" alt="Bar chart"/>
</p>
</figure>

<p>
<span
id="id__Toc149567630"
class="anchor"></span></p>
<table>
<caption>Table 5: level and repartition of errors per Thema code categories</caption>
<thead>
<tr
class="header">
<th
scope="col">
<b>Thema</b>
</th>
<th
scope="col">
<b>Publications</b>
</th>
<th
scope="col">
<b>images to fix</b>
</th>
<th
scope="col">
<b>unique ACE issues</b>
</th>
<th
scope="col">
<b>possibly wrong language</b>
</th>
<th
scope="col">
<b>files without headings</b>
</th>
</tr>
</thead>
<tbody>
<tr
class="odd">
<td>A</td>
<td>6</td>
<td>26,7</td>
<td>2,7</td>
<td>1,0</td>
<td>2,2</td>
</tr>
<tr
class="even">
<td>C</td>
<td>4</td>
<td>30,0</td>
<td>4,3</td>
<td>2,3</td>
<td>3,8</td>
</tr>
<tr
class="odd">
<td>D</td>
<td>30</td>
<td>19,3</td>
<td>2,1</td>
<td>2,8</td>
<td>2,4</td>
</tr>
<tr
class="even">
<td>F</td>
<td>68</td>
<td>10,0</td>
<td>2,4</td>
<td>1,1</td>
<td>2,3</td>
</tr>
<tr
class="odd">
<td>J</td>
<td>23</td>
<td>13,5</td>
<td>2,6</td>
<td>2,7</td>
<td>2,1</td>
</tr>
<tr
class="even">
<td>K</td>
<td>26</td>
<td>24,6</td>
<td>4,1</td>
<td>3,0</td>
<td>2,0</td>
</tr>
<tr
class="odd">
<td>L</td>
<td>11</td>
<td>6,4</td>
<td>3,1</td>
<td>3,5</td>
<td>0,8</td>
</tr>
<tr
class="even">
<td>M</td>
<td>20</td>
<td>39,0</td>
<td>3,3</td>
<td>2,0</td>
<td>1,9</td>
</tr>
<tr
class="odd">
<td>N</td>
<td>16</td>
<td>15,0</td>
<td>2,9</td>
<td>2,9</td>
<td>1,8</td>
</tr>
<tr
class="even">
<td>P</td>
<td>22</td>
<td>21,4</td>
<td>3,9</td>
<td>2,6</td>
<td>2,1</td>
</tr>
<tr
class="odd">
<td>Q</td>
<td>11</td>
<td>10,9</td>
<td>2,1</td>
<td>3,3</td>
<td>0,8</td>
</tr>
<tr
class="even">
<td>R</td>
<td>5</td>
<td>40,0</td>
<td>4,0</td>
<td>0,8</td>
<td>3,0</td>
</tr>
<tr
class="odd">
<td>S</td>
<td>4</td>
<td>35,0</td>
<td>4,5</td>
<td>0,0</td>
<td>3,8</td>
</tr>
<tr
class="even">
<td>T</td>
<td>3</td>
<td>23,3</td>
<td>5,3</td>
<td>2,0</td>
<td>3,0</td>
</tr>
<tr
class="odd">
<td>target</td>
<td>1</td>
<td>0,0</td>
<td>0,0</td>
<td>0,0</td>
<td>0,0</td>
</tr>
<tr
class="even">
<td>U</td>
<td>5</td>
<td>24,0</td>
<td>4,0</td>
<td>2,4</td>
<td>2,8</td>
</tr>
<tr
class="odd">
<td>V</td>
<td>14</td>
<td>22,1</td>
<td>3,1</td>
<td>2,2</td>
<td>1,4</td>
</tr>
<tr
class="even">
<td>W</td>
<td>13</td>
<td>20,0</td>
<td>2,6</td>
<td>2,2</td>
<td>1,2</td>
</tr>
<tr
class="odd">
<td>Y</td>
<td>33</td>
<td>23,6</td>
<td>2,5</td>
<td>0,8</td>
<td>2,0</td>
</tr>
</tbody>
</table>
<p>
<span
id="id__Toc149567652"
class="anchor"></span>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page31"
aria-label="Page 31"></span></p>
<figure>
<figcaption>Figure 9: Candlestick chart showing number of publications, minimum, average and maximum scores per Thema codes</figcaption>
<p>
<img
src="/images/media24/file12.jpg" alt="Candlestick chart, see data below."/>
</p>
</figure>

<p>
<span
id="id__Toc149567631"
class="anchor"></span>Table 6: number of publications, minimum, average and maximum scores per Thema codes.</p>
<table
style="width:100%;">
<caption>tblHeader</caption>
<colgroup>
<col />
<col />
<col />
<col />
<col />
<col />
</colgroup>
<thead>
<tr
class="header">
<th>
<b>Thema code</b>
</th>
<th>
<b>Publications</b>
</th>
<th>
<b>Average Score</b>
</th>
<th>
<b>Standard Deviation</b>
</th>
<th>
<b>Minimum Score</b>
</th>
<th>
<b>Maximum Score</b>
</th>
</tr>
</thead>
<tbody>
<tr
class="odd">
<td>A</td>
<td>6</td>
<td>35</td>
<td>17,87</td>
<td>16</td>
<td>58</td>
</tr>
<tr
class="even">
<td>C</td>
<td>4</td>
<td>43</td>
<td>14,11</td>
<td>31</td>
<td>61</td>
</tr>
<tr
class="odd">
<td>D</td>
<td>30</td>
<td>30</td>
<td>17,10</td>
<td>5</td>
<td>65</td>
</tr>
<tr
class="even">
<td>F</td>
<td>68</td>
<td>19</td>
<td>7,89</td>
<td>5</td>
<td>62</td>
</tr>
<tr
class="odd">
<td>J</td>
<td>23</td>
<td>24</td>
<td>15,05</td>
<td>5</td>
<td>66</td>
</tr>
<tr
class="even">
<td>K</td>
<td>26</td>
<td>37</td>
<td>20,54</td>
<td>11</td>
<td>66</td>
</tr>
<tr
class="odd">
<td>L</td>
<td>11</td>
<td>17</td>
<td>8,98</td>
<td>5</td>
<td>37</td>
</tr>
<tr
class="even">
<td>M</td>
<td>20</td>
<td>48</td>
<td>13,10</td>
<td>18</td>
<td>67</td>
</tr>
<tr
class="odd">
<td>N</td>
<td>16</td>
<td>26</td>
<td>16,76</td>
<td>5</td>
<td>63</td>
</tr>
<tr
class="even">
<td>P</td>
<td>22</td>
<td>33</td>
<td>17,32</td>
<td>10</td>
<td>77</td>
</tr>
<tr
class="odd">
<td>Q</td>
<td>11</td>
<td>20</td>
<td>9,63</td>
<td>9</td>
<td>36</td>
</tr>
<tr
class="even">
<td>R</td>
<td>5</td>
<td>50</td>
<td>16,77</td>
<td>20</td>
<td>61</td>
</tr>
<tr
class="odd">
<td>S</td>
<td>4</td>
<td>46</td>
<td>16,47</td>
<td>23</td>
<td>62</td>
</tr>
<tr
class="even">
<td>T</td>
<td>3</td>
<td>36</td>
<td>10,44</td>
<td>24</td>
<td>43</td>
</tr>
<tr
class="odd">
<td>target</td>
<td>1</td>
<td>0</td>
<td>0,00</td>
<td>0</td>
<td>0</td>
</tr>
<tr
class="even">
<td>U</td>
<td>5</td>
<td>35</td>
<td>21,25</td>
<td>4</td>
<td>59</td>
</tr>
<tr
class="odd">
<td>V</td>
<td>14</td>
<td>32</td>
<td>20,67</td>
<td>8</td>
<td>67</td>
</tr>
<tr
class="even">
<td>W</td>
<td>13</td>
<td>29</td>
<td>15,74</td>
<td>10</td>
<td>52</td>
</tr>
<tr
class="odd">
<td>Y</td>
<td>33</td>
<td>32</td>
<td>13,98</td>
<td>9</td>
<td>62</td>
</tr>
</tbody>
</table>
<p>
<span
id="id__Toc149567653"
class="anchor"></span>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page32"
aria-label="Page 32"></span></p>
<figure>
<figcaption>Figure 10: Bubble chart showing average score (X axis) per standard variation (Y axis), one bubble per Thema code, bubble size represents the number of publications in the sample.</figcaption>
<p>
<img
src="/images/media24/file13.jpg" alt="Bubble Chart, see data below."/>
</p>
</figure>

<p>
<span
id="id__Toc149567632"
class="anchor"></span></p>
<table>
<caption>Table 7: Average score, standard variation and number of publications per Thema code.</caption>
<colgroup>
<col />
<col />
<col />
<col />
</colgroup>
<thead>
<tr
class="header">
<th
scope="col">
<b>Thema code</b>
</th>
<th
scope="col">
<b>Publications</b>
</th>
<th
scope="col">
<b>Average Score</b>
</th>
<th
scope="col">
<b>Standard Deviation</b>
</th>
</tr>
</thead>
<tbody>
<tr
class="odd">
<td>A</td>
<td>6</td>
<td>35</td>
<td>17,87</td>
</tr>
<tr
class="even">
<td>C</td>
<td>4</td>
<td>43</td>
<td>14,11</td>
</tr>
<tr
class="odd">
<td>D</td>
<td>30</td>
<td>30</td>
<td>17,10</td>
</tr>
<tr
class="even">
<td>F</td>
<td>68</td>
<td>19</td>
<td>7,89</td>
</tr>
<tr
class="odd">
<td>J</td>
<td>23</td>
<td>24</td>
<td>15,05</td>
</tr>
<tr
class="even">
<td>K</td>
<td>26</td>
<td>37</td>
<td>20,54</td>
</tr>
<tr
class="odd">
<td>L</td>
<td>11</td>
<td>17</td>
<td>8,98</td>
</tr>
<tr
class="even">
<td>M</td>
<td>20</td>
<td>48</td>
<td>13,10</td>
</tr>
<tr
class="odd">
<td>N</td>
<td>16</td>
<td>26</td>
<td>16,76</td>
</tr>
<tr
class="even">
<td>P</td>
<td>22</td>
<td>33</td>
<td>17,32</td>
</tr>
<tr
class="odd">
<td>Q</td>
<td>11</td>
<td>20</td>
<td>9,63</td>
</tr>
<tr
class="even">
<td>R</td>
<td>5</td>
<td>50</td>
<td>16,77</td>
</tr>
<tr
class="odd">
<td>S</td>
<td>4</td>
<td>46</td>
<td>16,47</td>
</tr>
<tr
class="even">
<td>T</td>
<td>3</td>
<td>36</td>
<td>10,44</td>
</tr>
<tr
class="odd">
<td>target</td>
<td>1</td>
<td>0</td>
<td>0,00</td>
</tr>
<tr
class="even">
<td>U</td>
<td>5</td>
<td>35</td>
<td>21,25</td>
</tr>
<tr
class="odd">
<td>V</td>
<td>14</td>
<td>32</td>
<td>20,67</td>
</tr>
<tr
class="even">
<td>W</td>
<td>13</td>
<td>29</td>
<td>15,74</td>
</tr>
<tr
class="odd">
<td>Y</td>
<td>33</td>
<td>32</td>
<td>13,98</td>
</tr>
</tbody>
</table>
<p
style="text-align:left;"></p>
</section>
<section
id="recurrent-accessibility-issues-detected"
class="level3">
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page33"
aria-label="Page 33"></span>
</p>


### Recurrent accessibility issues detected
<p>As a complement to the Thema category level gap analysis, we listed the main known accessibility issues and tried to identify occurrences of these accessibility issues in the collected files. The following table resumes our findings. Results on each accessibility issue are detailed in the following sections.</p>
<p>
<span
id="id__Toc149567633"
class="anchor"></span></p>
<table>
<caption>Table 8: occurrences of main accessibility issues identified in collected files</caption>
<colgroup>
<col />
<col />
<col />
<col />
</colgroup>
<thead>
<tr
class="header">
<th
scope="col">
<b>Accessibility issue</b>
</th>
<th
scope="col">
<b>concern</b>
</th>
<th
scope="col">
<b>Number of files</b>
</th>
<th
scope="col">
<b>in % of the sample</b>
</th>
</tr>
</thead>
<tbody>
<tr
class="odd">
<td>
<b>Missing Accessibility Metadata</b>
</td>
<td>EPUB files</td>
<td>343</td>
<td>100</td>
</tr>
<tr
class="even">
<td>
<b>Non reflowable content</b>
</td>
<td>all formats</td>
<td>59</td>
<td>16</td>
</tr>
<tr
class="odd">
<td>
<b>Missing or bad textual alternative for non decorative graphical resources</b>
</td>
<td>all formats</td>
<td>312</td>
<td>83</td>
</tr>
<tr
class="even">
<td>
<b>Missing or bad Language Tag</b>
</td>
<td>EPUB files</td>
<td>227</td>
<td>66</td>
</tr>
<tr
class="odd">
<td>
<b>ACE Issues</b>
</td>
<td>EPUB files</td>
<td>319</td>
<td>93</td>
</tr>
</tbody>
</table>
<section
id="missing-accessibility-metadata"
class="level4">


#### Missing Accessibility Metadata
<ul>
<li>
<p
style="text-align:left;">
<b>Issue:</b> no accessibility metadata are present</p>
</li>
<li>
<p
style="text-align:left;">
<b>Rule:</b> EPUBaccessibility 1.1 section '2. Discoverability’</p>
</li>
<li>
<p
style="text-align:left;">
<b>Applies to:</b> EPUB files</p>
</li>
<li>
<p
style="text-align:left;">
<b>Problem:</b> the reader cannot know features or limitations they may experience while reading and the publication can’t be discovered through filtering</p>
</li>
<li>
<p
style="text-align:left;">
<b>Indicators:</b> calculated as follows: missing metadata - inferred metadata<a
href="#fn8"
class="footnote-ref"
id="fnref8"
epub:type="noteref"
role="doc-noteref"><sup>8</sup></a>, -3 (conformance metadata are counted as missing per ACE, but are not requested by the EAA). , minimum = 0</p>
</li>
<li>
<p
style="text-align:left;">
<b>Collected files affected:</b> 100%</p>
</li>
</ul>
</section>
<section
id="non-reflowable-content"
class="level4">


#### Non Reflowable content
<ul>
<li>
<p
style="text-align:left;">
<b>Issue:</b> the presentation of the content can’t be adjusted to fit the reader’s needs</p>
</li>
<li>
<p
style="text-align:left;">
<b>Rule:</b> EAA, Annex I, Section IV, f</p>
</li>
<li>
<p
style="text-align:left;">
<b>Applies to:</b> all formats</p>
</li>
<li>
<p
style="text-align:left;">
<b>Problem:</b> fixed displays impeach correct visual adaptation of the content</p>
</li>
<li>
<p
style="text-align:left;">
<b>Indicators:</b> pre-paginated formats</p>
</li>
<li>
<p
style="text-align:left;">
<b>Collected files affected:</b> 16%</p>
</li>
</ul>
</section>
<section
id="missing-or-bad-textual-alternative-for-non-decorative-graphical-resources"
class="level4">
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page34"
aria-label="Page 34"></span>
</p>


#### Missing or bad textual alternative for non decorative graphical resources
<ul>
<li>
<p
style="text-align:left;">
<b>Issue:</b> No textual alternative is provided for informative graphical contents or the alternative is recognized as not meaningful (file name or one word)</p>
</li>
<li>
<p
style="text-align:left;">
<b>Rule:</b> WCAG, Guideline 1.1 Text Alternatives, Success Criterion 1.1.1 Non-text Content, level A</p>
</li>
<li>
<p
style="text-align:left;">
<b>Applies to:</b> all formats</p>
</li>
<li>
<p
style="text-align:left;">
<b>Problem:</b> the non visual readers using TTS or assistive technologies will lose important information necessary to understand the content</p>
</li>
<li>
<p
style="text-align:left;">
<b>Indicators:</b> calculated as follows: content images – content images with alt-text (more than one word and not equal to filename) – contents images decorative</p>
</li>
<li>
<p
style="text-align:left;">
<b>Collected files affected:</b> 83%</p>
</li>
</ul>
</section>
<section
id="missing-or-bad-language-tag"
class="level4">


#### Missing or bad Language Tag
<ul>
<li>
<p
style="text-align:left;">
<b>Issue:</b> words in different languages from the one of the main content are not identified as such</p>
</li>
<li>
<p
style="text-align:left;">
<b>Rule:</b> WCAG, Guideline 3.1 Readable, Success Criterion 3.1.2 Language of Parts, level AA</p>
</li>
<li>
<p
style="text-align:left;">
<b>Applies to:</b> all formats, but no way was found to identify that in PDF</p>
</li>
<li>
<p
style="text-align:left;">
<b>Problem:</b> non-visual readers using TTS or assistive technologies will experience strange or not understandable reading because of mispronunciation, incorrect braille rendering and bad hyphenations</p>
</li>
<li>
<p
style="text-align:left;">
<b>Indicators:</b> the wrong language assertion is done through a dedicated algorithm. It targets two or more following words in a sentence</p>
</li>
<li>
<p
style="text-align:left;">
<b>Collected files affected:</b> 66%</p>
</li>
</ul>
</section>
<section
id="ace-issues"
class="level4">


#### ACE issues
<p>Issues reported by ACE. The following table shows the number of files and the corresponding percentage of the samples containing errors per severity level. We can note that very few (5% only) files have critical issues, but 92% have serious issues which will need to be evaluated for remediation.</p>
<p>
<span
id="id__Toc149567634"
class="anchor"></span>Table 9: number and percentage of collected files affected per ACE issues gravity level.</p>
<table>
<colgroup>
<col />
<col />
<col />
</colgroup>
<tbody>
<tr
class="even">
<td>
<b>ACE issue</b>
</td>
<td>
<b>Number of files</b>
</td>
<td>
<b>% of the samples</b>
</td>
</tr>
<tr
class="odd">
<td>
<b>critical</b>
</td>
<td>19</td>
<td>5</td>
</tr>
<tr
class="even">
<td>
<b>serious</b>
</td>
<td>343</td>
<td>92</td>
</tr>
<tr
class="odd">
<td>
<b>moderate</b>
</td>
<td>132</td>
<td>35</td>
</tr>
<tr
class="even">
<td>
<b>minor</b>
</td>
<td>172</td>
<td>46</td>
</tr>
</tbody>
</table>
<p>A larger table of unique ACE issues has been produced for the use of the project and the building of testing files. The details of those errors are reported in the following tables. One shows the errors for which we proposed a detailed remediation complexity KPI, while the second shows the errors that are not addressed by a specific calculation.</p>
<p>
<span
id="id__Toc149567635"
class="anchor"></span>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page35"
aria-label="Page 35"></span>Table 10: percentage of the sample affected by ACE errors for which a detailed remediation complexity KPI has been established.</p>
<table>
<colgroup>
<col />
<col />
</colgroup>
<tbody>
<tr
class="even">
<td>ACE Issue</td>
<td>% of the samples affected</td>
</tr>
<tr
class="odd">
<td>Epub-Lang:Serious</td>
<td>82.83</td>
</tr>
<tr
class="even">
<td>Metadata-Accessmode:Serious</td>
<td>46.81</td>
</tr>
<tr
class="odd">
<td>Metadata-Accessmodesufficient:Moderate</td>
<td>71.75</td>
</tr>
<tr
class="even">
<td>Metadata-Accessibilityfeature:Serious</td>
<td>49.03</td>
</tr>
<tr
class="odd">
<td>Metadata-Accessibilityhazard:Serious</td>
<td>52.91</td>
</tr>
<tr
class="even">
<td>Metadata-Accessibilitysummary:Moderate</td>
<td>71.47</td>
</tr>
<tr
class="odd">
<td>Image-Alt:Critical</td>
<td>23.82</td>
</tr>
</tbody>
</table>
<p>
<span
id="id__Toc149567636"
class="anchor"></span>Table 11: percentage of the sample affected by ACE errors for which no detailed remediation complexity KPI has been established.</p>
<table>
<colgroup>
<col />
<col />
</colgroup>
<tbody>
<tr
class="even">
<td>ACE Issue</td>
<td>% of the samples affected</td>
</tr>
<tr
class="odd">
<td>Empty-Table-Header:Minor</td>
<td>45.19</td>
</tr>
<tr
class="even">
<td>Empty-Heading:Minor</td>
<td>69.25</td>
</tr>
<tr
class="odd">
<td>Heading-Order:Moderate</td>
<td>47.33</td>
</tr>
<tr
class="even">
<td>Html-Has-Lang:Serious</td>
<td>51.07</td>
</tr>
<tr
class="odd">
<td>Link-In-Text-Block:Serious</td>
<td>68.98</td>
</tr>
<tr
class="even">
<td>Color-Contrast:Serious</td>
<td>27.01</td>
</tr>
<tr
class="odd">
<td>Metadata-Accessibilityhazard-Invalid:Moderate</td>
<td>28.88</td>
</tr>
<tr
class="even">
<td>Aria-Allowed-Role:Minor</td>
<td>29.41</td>
</tr>
<tr
class="odd">
<td>Aria-Roles:Minor</td>
<td>23.80</td>
</tr>
<tr
class="even">
<td>Epub-Pagelist-Broken:Serious</td>
<td>5.08</td>
</tr>
<tr
class="odd">
<td>Epub-Type-Has-Matching-Role:Minor</td>
<td>8.02</td>
</tr>
<tr
class="even">
<td>Landmark-Unique:Moderate</td>
<td>22.99</td>
</tr>
<tr
class="odd">
<td>Epub-Toc-Order:Serious</td>
<td>27.54</td>
</tr>
<tr
class="even">
<td>Link-Name:Serious</td>
<td>26.20</td>
</tr>
<tr
class="odd">
<td>Document-Title:Serious</td>
<td>15.24</td>
</tr>
<tr
class="even">
<td>Metadata-Accessibilityfeature-Invalid:Minor</td>
<td>12.57</td>
</tr>
</tbody>
</table>
</section>
</section>
<section
id="potential-accessibility-issues-undetectable-through-automated-analysis"
class="level3">


### Potential accessibility issues undetectable through automated analysis
<p>The following are issues that cannot be detected automatically and will require ad hoc human testing.</p>
<section
id="reflowable-restrictions"
class="level4">


#### Reflowable restrictions
<ul>
<li>
<p
style="text-align:left;">
<b>Issue:</b> adjusting the presentation leads to letters or sentences overlapping or making the content visually unreadable in any way</p>
</li>
<li>
<p
style="text-align:left;">
<b>Rule:</b> EAA, Annex I, Section IV, f</p>
</li>
<li>
<p
style="text-align:left;">
<b>Applies to:</b> reflowable EPUB</p>
</li>
<li>
<p
style="text-align:left;">
<b>Problem:</b> fixed styles impeach correct visual adaptation of the content</p>
</li>
</ul>
</section>
<section
id="specific-contents-to-be-verified-manually-if-found-in-files"
class="level4">
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page36"
aria-label="Page 36"></span>
</p>


#### Specific contents to be verified manually if found in files 
<p>Some very specialised contents such as forms, scripts, maths, videos and audios are not usually used in ebooks, but as this may happen, it will be necessary to include them in remediation testing. The following table shows that very few occurrences were found in the sample collection.</p>
<p>
<span
id="id__Toc149567637"
class="anchor"></span>Table 12: number and percentage of collected files per specific content.</p>
<table>

<thead>
<tr
class="header">
<th
scope="col">Content</th>
<th
scope="col">
<b>Number of files</b>
</th>
<th
scope="col">
<b>in % of the samples</b>
</th>
</tr>
</thead>
<tbody>
<tr
class="odd">
<td>
<b>Forms</b>
</td>
<td>1</td>
<td>0.3</td>
</tr>
<tr
class="even">
<td>
<b>Scripts</b>
</td>
<td>17</td>
<td>5</td>
</tr>
<tr
class="odd">
<td>
<b>Maths contents</b>
</td>
<td>7</td>
<td>2</td>
</tr>
<tr
class="even">
<td>
<b>Video contents</b>
</td>
<td>0</td>
<td>0</td>
</tr>
<tr
class="odd">
<td>
<b>Audio contents</b>
</td>
<td>7</td>
<td>2</td>
</tr>
</tbody>
</table>
</section>
</section>
</section>
<section
id="classification-for-remediation">



## Classification for remediation

<p>The following classification aims to list the remediation workflows to test. A list of six elements is spread across the different categories, here is a summary of it:</p>
<ol
type="1">
<li>
<p>PDF to PDF/UA (compliant to WCAG 2.1, level AA)</p>
</li>
<li>
<p>PDF to Reflowable EPUB3 (compliant EPUB Accessibility 1.1, WCAG 2.1, level AA)</p>
</li>
<li>
<p>FXL to «accessible» FXL (compliant EPUB Accessibility 1.1, WCAG 2.1, level AA)</p>
</li>
<li>
<p>FXL to Reflowable EPUB3 (compliant EPUB Accessibility 1.1, WCAG 2.1, level AA)</p>
</li>
<li>
<p>EPUB2 to EPUB3 (compliant EPUB Accessibility 1.1, WCAG 2.1, level AA)</p>
</li>
<li>
<p>Reflowable EPUB to Reflowable EPUB3 (compliant EPUB Accessibility 1.1, WCAG 2.1, level AA)</p>
</li>
</ol>
<section
id="pdfs"
class="level3">


### PDFs
<p>As a representation of the printed page, the PDF format accessibility features are limited in term of flexibility and choice in the presentation of the content (For details about the format and it’s known limitations, refer to the Annex <a
href="#id__heading=h.l9tqzvg5sm75"><u><u>Ebooks files formats</u></u></a>).</p>
<p>We see two possible remediation options for the PDF files:</p>
<ol
type="1">
<li>
<p>improve the file to reach PDF/UA standard with WCAG 2.1 AA conformance, allowing the file to support the text zoom functionality provided by most of the reading applications. These files will not totally comply with the EAA's requisites, but will provide state-of-the-art compliance.</p>
</li>
<li>
<p>convert the file to a reflowable EPUB to reach full compliance with EAA requirements.</p>
</li>
</ol>
</section>
<section
id="fixed-layout-epubs"
class="level3">


### Fixed Layout EPUBs
<p>Fixed layout EPUBs are subject to the same visual adjustment limitations as PDF: changing font type and spaces between letters, words, lines, or paragraphs is not possible. The possible remediations are:</p>
<ol
start="3"
type="1">
<li>
<p>
<span
epub:type="pagebreak"
role="doc-pagebreak"
id="page37"
aria-label="Page 37"></span>improve the file to reach WCAG 2.1 AA and EPUB accessibility 1.1. As in the case of PDF files, in Fixed Layout EPUB some accessibility features are supported and others are not. If the file is made according to the specifications, however, it must support text zoom functionality provided by most of the reading applications.</p>
</li>
<li>
<p>convert the file to a reflowable EPUB to reach full compliance with EAA requirements.</p>
</li>
</ol>
</section>
<section
id="reflowable-epubs"
class="level3">


### Reflowable EPUBs
<p>Reflowable EPUBs are known to be fully compliant with EAA requirements<a
href="#fn9"
class="footnote-ref"
id="fnref9"
epub:type="noteref"
role="doc-noteref"><sup>9</sup></a> if they conform to WCAG 2.1 AA (or superior) and EPUB accessibility 1.1. e found different types of remediation needs:</p>
<ol
start="5"
type="1">
<li>
<p>EPUB2 files need to be converted to reflowable EPUB3;</p>
</li>
<li>
<p>Reflowable EPUB3 files need to become compliant with WCAG 2.1 AA and the EPUB accessibility 1.1 .</p>
</li>
</ol>
</section>
</section>
<section
id="outcomes-1">


## Outcomes
<p>From this gap analysis, we were able to establish a classification of remediation needs and build test files for each of the classifications.</p>
<p>Direct outcomes of this work are</p>
<ul>
<li>
<p>a remediation complexity assessment methodology applicable to collections of files;</p>
</li>
<li>
<p>a view of the remediation complexity per Thema category;</p>
</li>
<li>
<p>a view of main accessibility issues detected.</p>
</li>
</ul>
<p>The heavy presence of images and visual resources appears to be the main criteria of demarcation between categories that will reclaim more efforts to remediate (Medicine, Earth sciences and Sports) and others (Fiction, Philosophy, Religion and Law) that will be easier to remediate.</p>
<p>As per the following steps of the ABE Lab project, it allows us to establish a testing classification and methodology as well as building meaningful files to test for remediation tools.</p>
</section>
</section>
<section
id="footnotes"
class="footnotes footnotes-end-of-document"
epub:type="footnotes">
<hr />
<ol>
<li
id="fn1">
<p>A detailed list of <a
href="#id__heading=h.6uy11yd7h6wv"><u>Norms and Standards</u></a> is available as annex to this document.<a
href="#fnref1"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn2">
<p>Available at https://www.w3.org/TR/epub-a11y-eaa-mapping/<a
href="#fnref2"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn3">
<p>EAA Annex I, Section IV, f) iii) available at<br /><a
href="https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882#d1e32-100-1"><u>https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882#d1e32-100-1</u></a><a
href="#fnref3"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn4">
<p>On October 5, 2023 version 2.2 of the WCAG was officially released as a W3C recommendation. This update does not impact or compromise the analysis, research work and testing carried out in the context of the ABE Lab project.<a
href="#fnref4"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn5">
<p>PDF/UA standard, ISO 14289-1:2014: <a
href="https://www.iso.org/standard/64599.html"><u>https://www.iso.org/standard/64599.html</u></a>.<a
href="#fnref5"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn6">
<p>Target file publicly available at<br /><a
href="https://www.fondazionelia.org/wp-content/uploads/2023/10/European_Stories_2023_EUPL.epub"><u>https://www.fondazionelia.org/wp-content/uploads/2023/10/European_Stories_2023_EUPL.epub</u></a>.<a
href="#fnref6"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn7">
<p>Remediation complexity indicators are available for the publishers partners of the project.<a
href="#fnref7"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn8">
<p>Inferred metadata are found per RGTK, meaning that we are able to see an accessibility feature in the file even if the information about it was not provided by the publisher. Therefore no remediation need is necessary except for informing about it, which is already automated per RGTK.<a
href="#fnref8"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
<li
id="fn9">
<p>See <a
href="https://www.w3.org/TR/epub-a11y-eaa-mapping/"><u>EPUB Accessibility - EU Accessibility Act Mapping</u></a> Group note established by W3C.<a
href="#fnref9"
class="footnote-back"
role="doc-backlink">↩︎</a></p>
</li>
</ol>
</section>

<section>
<h1 id="annexes-gap-analysis">Annexes</h1>
</section>

<section>
<h1 id="addendum---per-year-analysis">Addendum - Per year
analysis</h1>
<p style="text-align:left;">As part of the elaborations to define the gap analysis
between the accessibility requirements of the EAA and the accessibility
issues of the ebooks in the backlist, we also checked the breakdown by
year to see if we were able to identify meaningful patterns. Due to the
context of our research, this part was not considered so relevant and
therefore was not published in the initial version of this report. For
clarification and completion of the information related to the study, we
have decided to add this information as an Addendum by May 2024.</p>
<p style="text-align:left;">In the context of the ABE Lab research, the per-year
analysis resulted in being fewly relevant because all Thema categories
of books are present for most of the years, leading to averages scores
per year variation from 20 to 37. This does not indicate that a per-year
analysis is not relevant and we suggest that it should be done on
defined collections. We expect that a refined per-year analysis crossed
with Thema categories done on higher numbers of samples would help to
identify errors patterns. This was confirmed by publishers who already
started the remediation of their backlists.</p>
<p>This analysis showed that our sample is composed of a third of files
produced after 2021, which will probably be the case for most of the
ebooks that will be considered to be made accessible to comply with the
EAA. It showed higher levels of complexity around the years 2017 to
2020, mainly because the samples collected for those years have a larger
number of images.</p>

<figure>
<figcaption>
<p>Table A1: reflowable EPUBs, per year, number of publications and
scoring.</p>
</figcaption>
<table style="width:100%;">
<thead>
<tr>
<th><b>Year</b></th>
<th><b>Publications</b></th>
<th><b>Average Score</b></th>
<th><b>Standard Deviation</b></th>
<th><b>Minimum Score</b></th>
<th><b>Maximum Score</b></th>
</tr>
<thead>
<tbody>
<tr class="even">
<td>2007</td>
<td>3</td>
<td>20</td>
<td>4,58</td>
<td>16</td>
<td>25</td>
</tr>
<tr class="odd">
<td>2008</td>
<td>2</td>
<td>34</td>
<td>0,71</td>
<td>33</td>
<td>34</td>
</tr>
<tr class="even">
<td>2009</td>
<td>3</td>
<td>22</td>
<td>4,04</td>
<td>18</td>
<td>26</td>
</tr>
<tr class="odd">
<td>2010</td>
<td>12</td>
<td>34</td>
<td>19,69</td>
<td>8</td>
<td>61</td>
</tr>
<tr class="even">
<td>2011</td>
<td>23</td>
<td>30</td>
<td>11,54</td>
<td>20</td>
<td>56</td>
</tr>
<tr class="odd">
<td>2012</td>
<td>6</td>
<td>32</td>
<td>16,24</td>
<td>20</td>
<td>62</td>
</tr>
<tr class="even">
<td>2013</td>
<td>3</td>
<td>31</td>
<td>16,20</td>
<td>21</td>
<td>50</td>
</tr>
<tr class="odd">
<td>2014</td>
<td>5</td>
<td>28</td>
<td>15,87</td>
<td>16</td>
<td>55</td>
</tr>
<tr class="even">
<td>2015</td>
<td>11</td>
<td>25</td>
<td>13,74</td>
<td>14</td>
<td>55</td>
</tr>
<tr class="odd">
<td>2016</td>
<td>12</td>
<td>29</td>
<td>17,54</td>
<td>9</td>
<td>67</td>
</tr>
<tr class="even">
<td>2017</td>
<td>8</td>
<td>37</td>
<td>17,50</td>
<td>20</td>
<td>63</td>
</tr>
<tr class="odd">
<td>2018</td>
<td>33</td>
<td>33</td>
<td>15,48</td>
<td>16</td>
<td>66</td>
</tr>
<tr class="even">
<td>2019</td>
<td>15</td>
<td>32</td>
<td>16,15</td>
<td>10</td>
<td>62</td>
</tr>
<tr class="odd">
<td>2020</td>
<td>10</td>
<td>36</td>
<td>16,07</td>
<td>10</td>
<td><p>55</p>
<p></p></td>
</tr>
<tr class="even">
<td>2021</td>
<td>24</td>
<td>30</td>
<td>20,05</td>
<td>4</td>
<td>77</td>
</tr>
<tr class="odd">
<td>2022</td>
<td>104</td>
<td>27</td>
<td>17,90</td>
<td>5</td>
<td>67</td>
</tr>
<tr class="even">
<td>2023</td>
<td>38</td>
<td>27</td>
<td>18,08</td>
<td>0</td>
<td>66</td>
</tr>
</tbody>
</table>
</figure>
<figure>
<figcaption>
<p>Table A2: level and repartition of errors per year.</p>
</figcaption>
<table>
<thead>
<tr>
<th><b>Year</b></th>
<th><b>Publications</b></th>
<th><b>images to fix</b></th>
<th><b>Unique ACE issues</b></th>
<th><b>Possibly wrong language</b></th>
<th><b>files without headings</b></th>
</tr>
</thead>
<tbody>
<tr class="even">
<td>2007</td>
<td>3</td>
<td>10,0</td>
<td>2,0</td>
<td>1,3</td>
<td>3,3</td>
</tr>
<tr class="odd">
<td>2008</td>
<td>2</td>
<td>20,0</td>
<td>3,0</td>
<td>4,5</td>
<td>2,5</td>
</tr>
<tr class="even">
<td>2009</td>
<td>3</td>
<td>13,3</td>
<td>2,0</td>
<td>0,0</td>
<td>3,0</td>
</tr>
<tr class="odd">
<td>2010</td>
<td>12</td>
<td>22,5</td>
<td>1,7</td>
<td>2,5</td>
<td>3,0</td>
</tr>
<tr class="even">
<td>2011</td>
<td>23</td>
<td>17,8</td>
<td>5,7</td>
<td>1,0</td>
<td>3,0</td>
</tr>
<tr class="odd">
<td>2012</td>
<td>6</td>
<td>20,0</td>
<td>1,5</td>
<td>2,3</td>
<td>4,2</td>
</tr>
<tr class="even">
<td>2013</td>
<td>3</td>
<td>20,0</td>
<td>1,7</td>
<td>2,0</td>
<td>4,0</td>
</tr>
<tr class="odd">
<td>2014</td>
<td>5</td>
<td>20,0</td>
<td>1,6</td>
<td>2,6</td>
<td>1,2</td>
</tr>
<tr class="even">
<td>2015</td>
<td>11</td>
<td>16,4</td>
<td>1,7</td>
<td>1,8</td>
<td>1,1</td>
</tr>
<tr class="odd">
<td>2016</td>
<td>12</td>
<td>18,3</td>
<td>2,9</td>
<td>2,5</td>
<td>1,5</td>
</tr>
<tr class="even">
<td>2017</td>
<td>8</td>
<td>25,0</td>
<td>3,3</td>
<td>1,8</td>
<td>3,0</td>
</tr>
<tr class="odd">
<td>2018</td>
<td>33</td>
<td>22,4</td>
<td>4,0</td>
<td>1,7</td>
<td>2,8</td>
</tr>
<tr class="even">
<td>2019</td>
<td>15</td>
<td>22,0</td>
<td>2,7</td>
<td>2,3</td>
<td>1,9</td>
</tr>
<tr class="odd">
<td>2020</td>
<td>10</td>
<td>28,0</td>
<td>2,8</td>
<td>2,1</td>
<td>0,9</td>
</tr>
<tr class="even">
<td>2021</td>
<td>24</td>
<td>20,0</td>
<td>2,7</td>
<td>2,1</td>
<td>2,4</td>
</tr>
<tr class="odd">
<td>2022</td>
<td>104</td>
<td>17,8</td>
<td>2,7</td>
<td>2,3</td>
<td>1,3</td>
</tr>
<tr class="even">
<td>2023</td>
<td>38</td>
<td>16,6</td>
<td>2,6</td>
<td>2,1</td>
<td>1,8</td>
</tr>
</tbody>
</table>
</figure>
<figure>
<figcaption>
<p>Figure A1: Bar chart showing level and repartition of errors per year
(visual representation of the data presented in table A2).</p>
</figcaption>
<img
src="C:\Users\gauti\OneDrive\Bureau\Update_Report_on_Backlist_Data_and_gap_analysis_word/media/image16.png" alt=""/>
</figure>
</section>