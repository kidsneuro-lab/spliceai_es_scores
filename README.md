# spliceai_es_scores

Pre computed Splice AI scores for essential splice sites

* This is in the form of a BED file

* `spliceai_es_scores.bed.gz` and `spliceai_es_scores.bed.gz.tbi` can be easily dowloaded and visualised in IGV or integrated into bioinformatics pipelines

* The score represents the SpliceAI reference score of a given Donor or Acceptor (based on those annotated in RefSeq)





Steps to convert VCF to BED

1. Run Python notebook

2. Run commands below

```
bgzip spliceai_es_scores.bed
tabix -f -S 1 -p bed spliceai_es_scores.sorted.bed.gz
```
