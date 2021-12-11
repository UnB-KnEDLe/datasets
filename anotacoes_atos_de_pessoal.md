


[Download Version 3 (**Restricted**) ](https://drive.google.com/file/d/19ZSHK24LFkK3VYLlKuItjzSh8fLBOmGW/view?usp=sharing)




# Source

Data extracted from the Diário Oficial do Distrito Federal (DODF) using [DODFMiner](https://dodfminer.readthedocs.io/) and manually annotated by volunteers associated with the KnEDLe project.

# Dataset Information

Datasets with info about personnel related acts and their respective entities. These datasets were validated by members of the KnEDLe project and can be used as a gold standard dataset.

The acts considered and their respective labels are presented below:

|    Act  | Label | 
|:-------------:|:-------------------:|
| Abono de permanência             | Ato_Abono_Permanencia|
|Cessão                            | Ato_Cessao|
|Exenoração de Cargo Comissionado  | Ato_Exoneracao_Comissionado|
|Exonoração de Cargo Efetivo       | Ato_Exoneracao_Efetivo|
|Nomeação de Cargo Comissionado    | Ato_Nomeacao_Comissionado|
|Nomeação de Cargo Efetivo         | Ato_Nomeacao_Efetivo|
|Retificação de Cargo Comissionado | Ato_Retificacao_Comissionado|
|Retificação de Cargo Efetivo      | Ato_Retificacao_Efetivo|
|Reversão                          | Ato_Reversao    |
|Substituição                      | Ato_Substituicao|
|Tornado sem efeito atos de aposentadoria | Ato_Tornado_Sem_Efeito_Apo|
|Tornado sem efeito atos de exoneração ou nomeação | Ato_Tornado_Sem_Efeito_Exo_Nom|

*Note: A [dataset with info about Acts of Retirement](https://github.com/UnB-KnEDLe/datasets/blob/master/atos_aposentadoria.md) was provided by the Tribunal de Contas do Distrito Federal (TCDF).*

[More information](https://github.com/UnB-KnEDLe/tutorial_annotation_teamtat) about the annotation process and its labels.

# Version 0
**size:** 13924 rows

Annotations from Batch 3. 

## Attribute Information 

|    Attribute  | Description | 
|:-------------:|:-------------------:|
|id_ato         | act identifier |
|id_dodf        | identifier of the DODF from which the act was extracted |
|num_doc_dodf   | number of the DODF from which the act was extracted |
|data_doc_dodf  | date of the DODF from which the act was extracted |
|tipo_rel       | type of the act to which the entity belongs|
|id_rel         | relation-level annotation identifier |
|anotador_rel   | who annotated the relation used to represent the act|
|texto_rel      | full text of the act |
|tipo_ent       | entity type |
|id_ent         | entity-level annotation identifier |
|anotador_ent   | who annotated the entity |
|texto_ent      | entity |

## Number of Labeled Acts

|    Class                       | Quantity | 
|:------------------------------:|:----:|
|Ato_Substituicao                |   502|
|Ato_Nomeacao_Comissionado       |   303|
|Ato_Retificacao_Efetivo         |   238|
|Ato_Exoneracao_Comissionado     |   236|
|Ato_Retificacao_Comissionado    |    39|
|Ato_Tornado_Sem_Efeito_Exo_Nom  |    29|
|Ato_Nomeacao_Efetivo            |    15|
|Ato_Exoneracao_Efetivo          |    10|
|Ato_Reversao                    |    10|
|Ato_Abono_Permanencia           |     6|
|Ato_Tornado_Sem_Efeito_Apo      |     1|
|Ato_Cessao                      |     0|
|Total                           |  1389|

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/1zxM1tDKoNPXgu9z7qdT_m3w5QDFUe1L4/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/11hkfYFfPZmOPFbV1Bm8FZkt1thIS5Ulz?usp=sharing)

# Version 1
**size:** 36040 rows

Added annotations from Batch 1 and Validation Batch.

## Attribute Information 

The attributes of this version are the same as in the previous version.

## Number of Labeled Acts

|    Class                       | Quantity | 
|:------------------------------:|:----:|
|Ato_Substituicao                |  1251|
|Ato_Nomeacao_Comissionado       |   789|
|Ato_Exoneracao_Comissionado     |   675|
|Ato_Retificacao_Efetivo         |   441|
|Ato_Tornado_Sem_Efeito_Exo_Nom  |    90|
|Ato_Retificacao_Comissionado    |    89|
|Ato_Cessao                      |    77|
|Ato_Abono_Permanencia           |    61|
|Ato_Exoneracao_Efetivo          |    29|
|Ato_Reversao                    |    26|
|Ato_Nomeacao_Efetivo            |    20|
|Ato_Tornado_Sem_Efeito_Apo      |    11|
|Total                           |  3559|

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/1CyYlpewhdN7SRAZSCrtQQDIuItQdognA/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/11hkfYFfPZmOPFbV1Bm8FZkt1thIS5Ulz?usp=sharing)

# Version 2
**size:** 52805 rows

Added annotations from Batch 2, with the exception of the annotations from documents 70 and 71 due to technical problems.

## Attribute Information 

The attributes of this version are the same as in the previous version.

## Number of Labeled Acts

|    Class                       | Quantity | 
|:------------------------------:|:----:|
|Ato_Substituicao                |  1636|
|Ato_Nomeacao_Comissionado       |  1359|
|Ato_Exoneracao_Comissionado     |  1142|
|Ato_Retificacao_Efetivo         |   578|
|Ato_Tornado_Sem_Efeito_Exo_Nom  |   135|
|Ato_Retificacao_Comissionado    |   131|
|Ato_Exoneracao_Efetivo          |   105|
|Ato_Cessao                      |    88|
|Ato_Abono_Permanencia           |    74|
|Ato_Nomeacao_Efetivo            |    56|
|Ato_Reversao                    |    36|
|Ato_Tornado_Sem_Efeito_Apo      |    13|
|Total                           |  5353|

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/1G4rkRK8XTgn7g9yQR5KyN-t1peCuPYBz/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/11hkfYFfPZmOPFbV1Bm8FZkt1thIS5Ulz?usp=sharing)

# Version 3
**size:** 93916 rows

Added annotations from Batch NIDO, with the exception of the annotations from document 70 due to technical problems.

## Attribute Information 

The attributes of this version are the same as in the previous version.

## Number of Labeled Acts

|    Class                       | Quantity | 
|:------------------------------:|:----:|
|Ato_Substituicao                |  2423|
|Ato_Exoneracao_Comissionado     |  2380|
|Ato_Nomeacao_Comissionado       |  2314|
|Ato_Retificacao_Efetivo         |  1241|
|Ato_Exoneracao_Efetivo          |   303|
|Ato_Cessao                      |   267|
|Ato_Tornado_Sem_Efeito_Exo_Nom  |   251|
|Ato_Retificacao_Comissionado    |   201|
|Ato_Abono_Permanencia           |   137|
|Ato_Nomeacao_Efetivo            |    79|
|Ato_Reversao                    |    62|
|Ato_Tornado_Sem_Efeito_Apo      |    21|
|Total                           |  9679|

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/19ZSHK24LFkK3VYLlKuItjzSh8fLBOmGW/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/11hkfYFfPZmOPFbV1Bm8FZkt1thIS5Ulz?usp=sharing)


# Relevant Papers

# Papers That Cite This Dataset
