README.txt
24 January 2019
Updated: 11 April 2019
Eleanor Chodroff, Alessandra Golden, and Colin Wilson

###########################
Please cite the following for use of this data: 
Chodroff, E., Golden, A., and Wilson, C. (2019). Cross-linguistic covariation of stop VOT: Evidence for a universal constraint on phonetic realization: covariation of stop voice onset time across languages. The Journal of the Acoustical Society of America, 145(1). EL1–EL7.

@article{ChodroffEtAl2019,
author = {Chodroff, Eleanor and Golden, Alessandra and Wilson, Colin},
doi = {10.1121/1.5088035},
journal = {The Journal of the Acoustical Society of America},
number = {1},
pages = {EL109--EL115},
title = {Covariation of stop voice onset time across languages : {E}vidence for a universal constraint on phonetic realization},
volume = {145},
year = {2019}
}
########################### 

This directory accompanies the manuscript "Cross-linguistic covariation of stop VOT: Evidence for a universal constraint on phonetic realization: covariation of stop voice onset time across languages" in JASA Express Letters.

The directory contains the following items:

1) ChodroffGoldenWilson2019_vot.csv: The VOT values collected from the literature. The values are typically averages over tokens and frequently groups of speakers, though the primary source should be consulted for verification. The columns within this dataset are as follows:
	family: language family obtained from WALS
	language: obtained from source
	dialect: obtained from source, if specified
	source: location of collected VOT value, please refer to *_references.pdf for the full citations
	primary.source: original location of collected VOT value (NA indicates that the source is indeed the primary source)
	poa.narrow: narrow place of articulation, provided by the source
	poa.broad: broad place of articulation (labial, coronal, dorsal), specified by authors, please refer to primary text for description
	voice: voice specification from the source
	vot.category: broad VOT category (long.lag, short.lag, lead), specified by authors, please refer to primary text for description
	vot: voice onset time (VOT) value
	voice.contrast: yes/no indicating whether the language has a voice contrast, obtained from WALS or in cases of omission, from the source of the VOT value
	notes: additional notes regarding the materials or speakers in the cited study
	voice.narrow: approximate label of laryngeal category obtained from the literature. Some additional post-processing was applied to this column to ensure that the category label for each language and laryngeal category was constant. This primary purpose of this label was to ensure that stops classified within the same laryngeal category from a given language variety were kept together. Note that we do not necessarily endorse the label as a true reflection of the laryngeal category or voicing state of a given language variety.
	in.ChodroffGoldenWilson2019: yes or no indicator for whether the data point was included in Chodroff, Golden, & Wilson (2019, JASA-EL). 
	

2) ChodroffGoldenWilson2019_vot_avg.csv: The VOT means averaged within each language-dialect pairing for each place of articulation and VOT category (long-lag, short-lag, lead). The columns within this dataset are as follows:
	family: language family obtained from WALS
	language: obtained from source
	dialect: obtained from source, if specified
	poa.broad: broad place of articulation (labial, coronal, dorsal), specified by authors based on poa.narrow (see ChodroffGoldenWilson2019_vot.csv)
	vot.category: broad VOT category (long.lag, short.lag, lead), specified by authors, please refer to primary text for description
	vot.mu: voice onset time (VOT) mean within each language-dialect pairing per broad place of articulation and vot.category

This dataset is re-generated after each update to ChodroffGoldenWilson2019_vot.csv. If interested in analyzing the exact dataset reported in Chodroff, Golden, & Wilson (2019), please use the data in ChodroffGoldenWilson2019_vot.csv with values marked as 'yes' within the column in.ChodroffGoldenWilson2019 to regenerate the language and dialect-specific averages. 


3) ChodroffGoldenWilson2019_vot.R: Code for reading in the homonymous dataset, adjusting the threshold between broad laryngeal categories, and creating the dataset with VOT values averaged by language variety (as in ChodroffGoldenWilson2019_vot_avg.csv)


4) ChodroffGoldenWilson2019_vot_avg.R: Code for reading in the homonymous dataset and running analyses presented in Chodroff, Golden, and Wilson (2019). 


5) ChodroffGoldenWilson2019_references.docx: References for the collected VOT values.


6) ChodroffGoldenWilson2019_references.pdf: References for the collected VOT values. 


7) /original_published_data: sub-directory containing only those VOT values and references included in the original manuscript

The sub-directory /original_published_data contains the original versions of (1) and (2), which are the VOT data in its original form and the means for each language and dialect, as well as the original reference lists. The structure of each file is the same as the corresponding files in the main directory. 





