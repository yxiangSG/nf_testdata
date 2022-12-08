# nf_testdata

```mermaid
graph TD;
  Input-->TrimGlore;
  TrimGlore--> BWA-Meth_align;
  BWA-Meth_align-->PICARD-deduplication;
  PICARD-deduplication-->MethylDackel;
  TrimGlore-->MultiQC;
  PICARD-deduplication-->MultiQC;
  BWA-Meth_align-->MultiQC;
  MethylDackel-->MultiQC;
```


```mermaid
graph TD;
  Input-->TrimGlore;
  TrimGlore--> STAR+Samtools;
  STAR+Samtools-->Salmon;
  Salmon-->Deseq2;
  Deseq2-->MultiQC;
  STAR+Samtools-->PICARD;
  PICARD-->MultiQC;
  STAR+Samtools-->MultiQC;
  STAR+Samtools-->RSeQC;
  RSeQC-->MultiQC;
```
