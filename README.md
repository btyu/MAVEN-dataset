# MAVEN-dataset-expansion
This repo adds more information onto [the MAVEN dataset](https://github.com/THU-KEG/MAVEN-dataset), such as lemma, PoS, dependency parsing, etc.

## Data

The expanded dataset is based on the MAVEN dataset published on Oct. 26, 2020, and  can be obtained from [release](https://github.com/btyu/MAVEN-dataset-expansion/releases). Those added tags are obtained via [Stanza](https://stanfordnlp.github.io/stanza). The data format is introduced in [this document](DataFormat.md), where we only add the "token_info" field in contrast to the original one. 

For the descriptions of the added fields (upos, xpos, etc.), please refer to the Stanza doc. 

The label types of upos, xpos and deprel are listed in [label_types](/label_types). Note that the types are based on the annotation results on MAVEN ([Code](statistics.ipynb)), so they may not be the universal sets.

For the original MAVEN dataset, please refer to the original repo.

## Codes

[This file](maven_expansion.ipynb) is the script to do this expansion.

