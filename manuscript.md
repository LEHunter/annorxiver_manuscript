---
author-meta:
- David N. Nicholson
- Jane Roe
bibliography:
- content/manual-references.json
date-meta: '2020-06-24'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="citation_title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="og:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="twitter:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="dc.date" content="2020-06-24" />

  <meta name="citation_publication_date" content="2020-06-24" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="David N. Nicholson" />

  <meta name="citation_author_institution" content="Department of Systems Pharmacology and Translational Therapeutics, University of Pennsylvania" />

  <meta name="citation_author_orcid" content="0000-0003-0002-5761" />

  <meta name="twitter:creator" content="@None" />

  <meta name="citation_author" content="Jane Roe" />

  <meta name="citation_author_institution" content="Department of Something, University of Whatever" />

  <meta name="citation_author_institution" content="Department of Whatever, University of Something" />

  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />

  <link rel="canonical" href="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta property="og:url" content="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta property="twitter:url" content="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta name="citation_fulltext_html_url" content="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta name="citation_pdf_url" content="https://greenelab.github.io/annorxiver_manuscript/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://greenelab.github.io/annorxiver_manuscript/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://greenelab.github.io/annorxiver_manuscript/v/6a3d0fe401b756856d9528eb20bc672c951048c5/" />

  <meta name="manubot_html_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/6a3d0fe401b756856d9528eb20bc672c951048c5/" />

  <meta name="manubot_pdf_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/6a3d0fe401b756856d9528eb20bc672c951048c5/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- biorxiv
- preprints
- pubmed central
- natural language processing
- descriptive linguistics
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: Linguistic Analysis of the bioRxiv Preprint Landscape
...






<small><em>
This manuscript
([permalink](https://greenelab.github.io/annorxiver_manuscript/v/6a3d0fe401b756856d9528eb20bc672c951048c5/))
was automatically generated
from [greenelab/annorxiver_manuscript@6a3d0fe](https://github.com/greenelab/annorxiver_manuscript/tree/6a3d0fe401b756856d9528eb20bc672c951048c5)
on June 24, 2020.
</em></small>

## Authors



+ **David N. Nicholson**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-0002-5761](https://orcid.org/0000-0003-0002-5761)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [danich1](https://github.com/danich1)<br>
  <small>
     Department of Systems Pharmacology and Translational Therapeutics, University of Pennsylvania
     · Funded by GBMF4552; T32 HG00046
  </small>

+ **Jane Roe**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [janeroe](https://github.com/janeroe)<br>
  <small>
     Department of Something, University of Whatever; Department of Whatever, University of Something
  </small>



## Abstract {.page_break_before}




## Introduction
1. What is a preprint
2. Why are preprints important?
3. Mention how preprints are being integrated into scientist’s everyday workflow

1. Talk about biorxiv and discuss how it is one of the repositories that maintains preprints along with citation of others such as arxiv/medrxiv etc.
2. Discuss works that analyze biorxiv from an audience perspective (quantifying tweets etc.)
3. Mention the gap which consists of analysing the language of biorxiv preprints (first to do this)
4. ^ Why is this important? What will this allow for future research projects?
5. Provide list of contributions within this manuscript


## Methods

### Datasets

#### BioRxiv
BioRxiv [@doi:10.1101/833400] is a repository of biological and biomedical research preprints.
We downloaded an xml snapshot of this repository on February 3, 2020 from   bioRxiv's Amazon S3 resource [@https://www.biorxiv.org/tdm] that contained the full text and image content of 98,023 preprints.
Preprints on bioRxiv are versioned, and in our snapshot 26,905 of 98,023 contained more than one version.
When preprints had multiple versions, we used only the latest one. 
Preprints in this snapshot were grouped into one of twenty-nine different categories.
Each preprint was also classified as a new result, confirmatory finding, or contradictory finding.
Some preprints in this snapshot have been withdrawn from bioRxiv.
When a preprint is withdrawn, its content is replaced with the reason for withdrawal.
Because we used the latest version, withdrawn preprints in our analysis contained only statements indicating their removal.

#### PubMed Central
PubMed Central (PMC) [@doi:10.1073/pnas.98.2.381] is a repository that contains free-to-read articles.
PMC contains two types of contributions: closed access articles from research funded by the United States National Institutes of Health (NIH) appearing after an embargo period and articles published under Gold Open Access [@doi:10.1007/s12471-017-1064-2] publishing schemes.
Paper availability within PMC is largely dependent on the journal's participation level [@url:https://www.ncbi.nlm.nih.gov/pmc/about/submission-methods/].
Individual journals have can fully participate in submitting articles to PMC, selectively participate sending only a few few of papers to PMC, only submit papers according to NIH's public access policy [@url:https://grants.nih.gov/grants/policy/nihgps/html5/section_8/8.2.2_nih_public_access_policy.htm], or not participate at all.
As of September 2019, PMC had 5,725,819 articles available [@url:https://www.ncbi.nlm.nih.gov/pmc/about/intro/].
Out of these 5 million articles, about 3 million were open access and available for text processing systems [@doi:10.1093/bioinformatics/btz070;@doi:10.1093/nar/gkz389].
We downloaded a snapshot of this open access subset on January 31, 2020.
This snapshot contains papers such as literature reviews, book reviews, editorials, case reports, research articles and more; however, we used only the research articles.

### Comparing Corpora
We used gensim [@raw:rehurek_lrec] (version 3.8.1) to preprocess the bioRxiv and PubMed Central corpora.
We removed the 337 gensim-provided stopwords.
Throughout our analysis we encountered non-word symbols (e.g., $\pm$), so we refer to words and symbols as tokens to avoid confusion.

Following the cleaning process, we calculated the frequency of every token shared between both corpora.
Because many tokens were unique to one set or the other and observed at low frequency, we used the union of the top 100 most frequent tokens from each corpus to compare them.
We generated a contingency table and calculated the odds ratio for each token.
Furthermore, we also calculated the 95% confidence interval for each odds ratio [@https://www.ncbi.nlm.nih.gov/books/NBK431098/].

### Visualizing the Preprint Landscape

#### Generate Document Representation
We used gensim [@raw:rehurek_lrec] (version 3.8.1) to train a word2vec continuous bag of words (CBOW) [@arxiv:1301.3781] model over the bioRxiv corpus. 
Our neural network architecture had 300 hidden nodes, and we trained this model for 20 epochs.
We set a fixed random seed and otherwise used gensim's default settings.
Following training, we generated a document vector for every article within bioRxiv and PubMed Central.
This document vector is calculated by taking the average of every token present within a given article, ignoring those that were absent from the word2vec model.

#### Dimensionality Reduction of Document Embeddings
We used principal component analysis (PCA) [@doi:10.1111/1467-9868.00196] to project bioRxiv document vectors into a low dimensional space.
We trained this model using scikit-learn's [@raw:scikit-learn] implementation of a randomized solver [@arxiv:0909.4061] with a random seed of 100, output of 50 principal components, and default settings for all other parameters.
For each principal component we calculated its cosine similarity with  all tokens in our word2vec model's vocabulary.
We report the top 100 positive and negative scoring tokens in the form of  word clouds, where the size of each word corresponds to the magnitude of similarity and color represents positive (blue) or negative (orange) association.

### Journal Recommendation

We aimed to predict the journal a paper would eventually be published in based on its embedding representation.
We illustrate our recommendations as a short list along with a network visualization available at [website link here once available](link goes here when live).
Since we sought to examine if embeddings were related to publication venue, we used a simple k-nearest neighbors approach with Euclidean distance to recommend journals.

First, we filtered all journals that had fewer than 100 papers in the PMC dataset.
A subset of our PMC corpus was directly linked to papers in bioRxiv as they had been published as open access articles.
We held out this subset and treated it as our gold standard test set.
We used the remainder of the PMC corpus for training and initial evaluation via cross validation.
We considered a list of ten journal suggestions to be an appropriate number and we considered a prediction to be a true positive if the correct journal appeared within the ten closest neighbors of the query article.

Certain journals publish articles in a focused topic area, while others publish articles that cover many topics.
Likewise, some journals have a publication rate of at most hundreds of papers per year while others publish at a rate of at least ten-thousand papers per year.
Accounting for these characteristics, we designed two approaches for recommending journals.

The first approach is based on individual paper proximity, which enabled us to provide an example of the specific article or articles that led to the prediction.
Conversely, predictions using this technique could be biased due to the overrepresentation of general topic journals.
We call this approach the paper-based classifier.
This classifier takes a query article that has been projected onto the embedding space trained on bioRxiv preprints as input and reports the journals of the top ten closest papers.
The number of journals returned via this method could be less than ten as multiple papers in close proximity to query article may belong to the same journal. 

The second approach is based on close proximity to a journal's centroid.
This technique provides recommendations that are more focused on domain-specific publication venues.
We call this approach the journal-based classifier.
This classifier was trained by computing journal centroids via taking the average embedding of all papers published in each journal.
Following the centroid calculation, this classifier takes a query article projected onto the same embedding space as above for input and reports the top ten nearest journals centroids.
Both the paper-based classifier and the journal-based classifier were optimized via 10-fold cross validation.
Lastly, we evaluated performance of both classifiers on our gold standard test set of published preprints.


## Results

### Comparing bioRxiv to PubMed Central

#### bioRxiv Repository

![
Neuroscience and bioinformatics are the two most common topics for preprints on bioRxiv.
This bar chart depicts the number of preprints that fall into each author-selected topic area.
](https://raw.githubusercontent.com/greenelab/annorxiver/35d3ea0de3c9c78e3c524736bbaada00928c88fb/biorxiv/exploratory_data_analysis/output/figures/preprint_category.png){#fig:biorxiv_categories}

![
Most of bioRxiv's preprints report new research findings.

This bar chart depicts the number of articles categorized based on author-selected article types.
](https://raw.githubusercontent.com/greenelab/annorxiver/94874e0f1e35bd667bf3b7c3dc6416068779444f/biorxiv/exploratory_data_analysis/output/figures/preprint_headings.png){#fig:biorxiv_headings}

Each preprint on bioRxiv has an author-selected topic area, and the predominant area in past reports has been neuroscience [@doi:10.7554/eLife.45133].
Our analysis of the full text release of bioRxiv confirms this previous finding (Figure {@fig:biorxiv_categories}).
The author-selected topic area abundances that we found in the full text largely matched previous studies [@doi:10.7554/eLife.45133; @doi:10.1001/jama.2017.21168].
One exception was microbiology, which has a larger share of preprints than in a previous report from 2018 [@doi:10.7554/eLife.45133] (Figure {@fig:biorxiv_categories}).
Authors also select from three article types when they upload their preprints.
We found that most preprints are categorized as new results (Figure {@fig:biorxiv_headings}), which is consistent with previous findings [@doi:10.1001/jama.2017.21168].

#### Global View
1. Create a treemap visualization of top X terms that are different between bioRxiv and PubMed Central (based on odds ratio)

#### Published Preprint Differences
![
Top scoring tokens for preprints are focused on figure citations whereas their published versions are more focused on data availability.
The plot on the left (A) is a point range plot of the odds ratio with respect to preprints.
Values greater than one indicate a high association with preprints while values less than one indicate a high association with published articles.
The dotted line provides a breaking point between both categories.
The plot on the right (B) is a barchart of token frequency appearing in preprints and published versions of preprints respectively.
](https://raw.githubusercontent.com/greenelab/annorxiver/e32661b855cc6622cc1138fcd1606ef3500f0ff9/biorxiv/corpora_comparison/output/figures/preprint_published_comparison.png){#fig:biorxiv_pmc_pre_published_comp}

A preprint's linguistic style can change once a preprint has undergone the revision process prior to being published.
We quantified this linguistic difference by calculating the odds ratio of tokens appearing in the union in bioRxiv preprints and their published counterparts within PMC.
Tokens with an odds ratio greater than one are mainly centered on paper/figure references and research specific terms (Figure {@fig: biorxiv_pmc_pre_published_comp}).
Tokens with an odds ratio of less than one are focused on data availability, and research measurements such as number of cases and controls or significance testing (Figure {@fig: biorxiv_pmc_pre_published_comp}).

### The bioRxiv Preprint Landscape
1. Provide the tSNE figure of the bioRxiv 
2. Discuss the results of the tSNE figure and highlight that there are category clusters within the figure

### Topic Analysis of Principal Components
1. Provide an example of the word cloud for principal components
2. Show plot of the principal components and the scatterplot
3. Mention that the word clouds can be found at xyz

### Journal Recommendations/Audience Associations
1. Title will change once analysis is finished 
2. Provide key figure for this section and take-home message


## Discussion


## Conclusion


## Acknowledgements


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>