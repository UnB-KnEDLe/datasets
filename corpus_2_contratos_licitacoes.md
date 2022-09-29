# Source

Data extracted from the Diário Oficial do Distrito Federal (DODF) using [DODFMiner](https://dodfminer.readthedocs.io/) and manually annotated by volunteers associated with the KnEDLe project.

# Dataset Information

Datasets with info about personnel related acts and their respective entities. These datasets were validated by members of the KnEDLe project and can be used as a gold standard dataset.

The acts considered and their respective labels are presented below:

|                   Act                   |              Label            | 
|:---------------------------------------:|:-----------------------------:|
|Aviso de Licitação                       | AVISO_LICITACAO               |
|Aviso de Revogação/Anulação de Licitação | AVISO_ANUL_REV_LICITACAO      |
|Aviso de Suspensão de Licitação          | AVISO_SUSPENSAO_LICITACAO     |
|Extrato de Aditamento Contratual         | EXTRATO_ADITAMENTO_CONTRATUAL |
|Extrato de Contrato                      | EXTRATO_CONTRATO              |
|Extrato de Convênio                      | EXTRATO_CONVENIO              |

[More information](https://github.com/UnB-KnEDLe/tutorial_anotacao_contratos_licitacoes) about the annotation process and its labels.

# Version 0
**size:** 30376 rows

Annotations from Batch 1 and Experimental Batch. 

## Attribute Information 

|    Attribute  | Description | 
|:-------------:|:-------------------:|
|id_dodf        | identifier of the DODF from which the act was extracted |
|tipo_rel       | type of the act to which the entity belongs |
|id_rel         | relation-level annotation identifier |
|anotador_rel   | anonymized identifier of the annotator who created the relation-level annotation |
|tipo_ent       | entity type |
|id_ent         | entity-level annotation identifier |
|anotador_ent   | anonymized identifier of the annotator who created the entity-level annotation |
|offset         | character offset from the beginning of the document to the first character of the annotation |
|length         | length of the annotation in characters |
|texto          | text of the annotated entity |
|id_ato         | identifier of the act to which the entity belongs |

## Number of Labeled Acts

|    Class                       | Quantity | 
|:------------------------------:|:--------:|
| AVISO_LICITACAO                |       317|
| AVISO_ANUL_REV_LICITACAO       |        31|
| AVISO_SUSPENSAO_LICITACAO      |        26|
| EXTRATO_ADITAMENTO_CONTRATUAL  |      1260|
| EXTRATO_CONTRATO               |      1223|
| EXTRATO_CONVENIO               |        18|
|Total                           |      2875|

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/1o4_ycHyyTZAPMXistI3-Ll-48a7MU-u9/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/1lalUjFuDX7GJ4gDej3JkJ7gqXXxSoGDL?usp=sharing)

# Version 1
**size:** 41044 rows

- Added the entity codigo_siggo to the acts of type REL_EXTRATO_CONTRATO and REL_ADITAMENTO_CONTRATO.
- Added the annotations from the Validation Batch.

## Attribute Information 

|    Attribute  | Description | 
|:-------------:|:-------------------:|
|id_dodf        | identifier of the DODF from which the act was extracted |
|tipo_rel       | type of the act to which the entity belongs |
|id_rel         | relation-level annotation identifier |
|anotador_rel   | anonymized identifier of the annotator who created the relation-level annotation |
|tipo_ent       | entity type |
|id_ent         | entity-level annotation identifier |
|anotador_ent   | anonymized identifier of the annotator who created the entity-level annotation |
|offset         | character offset from the beginning of the document to the first character of the annotation |
|length         | length of the annotation in characters |
|texto          | text of the annotated entity |
|id_ato         | identifier of the act to which the entity belongs |

## Number of Labeled Acts

|    Class                       | Quantity | 
|:------------------------------:|:--------:|
| AVISO_LICITACAO                |       638|
| AVISO_ANUL_REV_LICITACAO       |        46|
| AVISO_SUSPENSAO_LICITACAO      |        68|
| EXTRATO_ADITAMENTO_CONTRATUAL  |      1537|
| EXTRATO_CONTRATO               |      1542|
| EXTRATO_CONVENIO               |        24|
|Total                           |      3855|

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/1x-3C0ew_UoNddM3Sb40r7V5_cFKAaJaq/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/1fMNGGUutW8hVMpTBJ9Y1HLtvyJ5_XxVQ?usp=sharing)

# Relevant Papers
