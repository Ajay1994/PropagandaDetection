Dataset Details : https://zenodo.org/record/3271522#.XrD3b6gzZPZ

Train Dataset : https://zenodo.org/record/3271522/files/proppy_1.0.train.tsv?download=1
Dev Dataset : https://zenodo.org/record/3271522/files/proppy_1.0.dev.tsv?download=1
Test Dataset : https://zenodo.org/record/3271522/files/proppy_1.0.test.tsv?download=1

This is the corpus used in the paper "Proppy: Organizing the News Based on Their Propagandistic Content"

The corpus contains 52k articles from 100+ news outlets. Each article is
labeled as either “propagandistic” (positive class) or “non-propagandistic”
(negative class). The labeling was done indirectly using a technique known as
distant supervision, i.e. an article is considered propagandistic if it comes
from a news outlet that has been labeled as propagandistic by human annotators.

## Data format

We provide the corpus in three tsv files, including training, development, and
testing partitions.

The data is tab-separated. Each line represents one article, with the following
information:

1. article_text: the text of the article retrieved via newspaper3k package.
2. event_location: the geographical location - collected from GDELT.
3. average_tone: measures the impact of the event - collected from GDELT
4. article_date: article's publish date - collected from GDELT.
5. article_ID: GDELT ID , unique among the dataset's articles.
6. article_URL: the direct URL for the published article in its source website.
7. MBFC_factuality_label: factuality label for the source from MBFC
8. article_URL
9. MBFC_factuality_label   
10. URL_to_MBFC_page        
11. source_name     
12. MBFC_notes_about_source
13. MBFC_bias_label
14. source_URL
15. propaganda_label


## About

The corpus was downloaded using MBFC metadata to identify propagandistic vs
non-propagandistic sources. Specific URLs where then gathered with GDELT and
contents downloaded with newspaper3k
