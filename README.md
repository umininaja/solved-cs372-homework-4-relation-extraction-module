Download Link: https://assignmentchef.com/product/solved-cs372-homework-4-relation-extraction-module
<br>
The U.S. National Library of Medicine (NLM) maintains a database called MEDLINE that contains more than 25 million references to journal articles in biomedicine, whose access is mediated by PUBMED. In this homework assignment, you are asked to go through the following steps for biomedical relation extraction: (1) Search the MEDLINE abstracts to collect 100 sentences, each of which contains at least one of the five verbs below (including their inflected forms), (2) provide annotations to these sentences for triples &lt;X, ACTION, Y&gt; to extract, (3) develop a relation extraction module based on a randomly selected set of 80 sentences and assess its performance, and (4) apply the module to the remaining (annotated but unseen) 20 sentences and assess its performance.

Additional constraints are shown below:

<ul>

 <li>There is no need for an automated method to collect such sentences from MEDLINE. However, you must include the verbs activate, inhibit, and bind, together with another verb with positive actions, such as accelerate, augment, induce, stimulate, require, and up-regulate, and another verb with negative actions, such as abolish, block, down-regulate, and prevent, with 20 sentences for each of the five distinct verbs. You should also prefer recency of publication, starting with the year 2020, limiting up to 30 sentences per year, up to 10 sentences per journal, and up to two sentences per organization, as identified by the affiliation of the corresponding author.</li>

 <li>The following shows some guidelines for your annotation of expected triples.

  <ol>

   <li>Inorganic phosphate inhibited HPr kinase but activated HPR phosphatase.</li>

  </ol></li>

</ul>

&lt;Inorganic phosphate, inhibited, HPr kinase&gt;,

&lt;Inorganic phosphate, activated, HPR phosphatase&gt;

<ol>

 <li>All vasodilators activated K-Cl cotransport in LK SRBCs and HYZ in VSMCs, and this activation was inhibited by calyculin and genistein, two inhibitors of K-Cl cotransport.</li>

</ol>

&lt;All vasodilators, activated, K-CI cotransport&gt;

&lt;All vasodilators, activated, HYZ&gt;

&lt;this activation, was inhibited by, calyculin&gt; <strong>OR</strong> &lt;calyculin, inhibited, this activation&gt;

&lt;this activation, was inhibited by, genistein&gt; <strong>OR</strong> &lt;genistein, inhibited, this activation&gt;  &lt;this activation, was inhibited by, two inhibitors&gt; <strong>OR</strong> &lt;two inhibitors, inhibited, this activation&gt;

<ul>

 <li>In developing a relation extraction module, you should not use any of the thirdparty modules for coreference resolution, NER, relation extraction, event extraction, or parsers specifically made available for biomedicine, except for the NER module in NLTK. You should not use any of the external corpora for training.</li>

</ul>

Report the performance in terms of Precision/Recall/F-score for (3) and (4).

As before, you should use techniques that can be implemented in Python and NLTK.

<ul>

 <li><u>Write a Python code</u> for relation extraction.</li>

 <li><u>Show 100 sentences</u>, annotated with expected triples, together with tags for 80 sentences.</li>

 <li><u>Discuss your results</u>, to explain how you addressed the goal, and to suggest how you can improve the quality of the results further. This document must be in English.</li>

</ul>

All the requirements as underlined above must be composed by yourself and without help from anyone else. Any similarity of the results will be flagged for plagiarism and, if found sufficiently similar, penalized, up to, but not limited to, a failure to this homework.