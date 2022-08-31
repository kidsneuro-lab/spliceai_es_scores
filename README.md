# spliceai_es_scores

Pre computed Splice AI scores for essential splice sites

* This is in the form of a BED file

* `spliceai_es_scores.bed.gz` and `spliceai_es_scores.bed.gz.tbi` can be easily dowloaded and visualised in IGV or integrated into bioinformatics pipelines

* The score represents the SpliceAI reference score of a given Donor or Acceptor (based on those annotated in RefSeq)

<img width="1124" alt="image" src="https://user-images.githubusercontent.com/1222657/187672426-433353fd-6eb8-48ef-9f95-f673bb328d53.png">

Steps to convert VCF to BED

1. Run Python notebook

2. Run commands below

```
bgzip spliceai_es_scores.bed
tabix -f -S 1 -p bed spliceai_es_scores.sorted.bed.gz
```
