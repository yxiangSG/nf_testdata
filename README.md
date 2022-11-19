# nf_testdata

```mermaid
 %%{init: { 'theme':'dark', 'sequence': {'useMaxWidth':false} } }%%
graph TD;
Input-->TrimGlore;
TrimGlore-->BWA-Meth;
TrimGlore-->MultiQC;
BWA-Meth-->MultiQC;
BWA-Meth-->PICARD;
PICARD-->MultiQC;
PICARD-->MethylDackel;
MethylDackel-->MultiQC;
```
