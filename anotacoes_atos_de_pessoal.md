


[Download Version 0 (**Restricted**) ](https://drive.google.com/file/d/1zxM1tDKoNPXgu9z7qdT_m3w5QDFUe1L4/view?usp=sharing)




# Source

Data extracted from the Diário Oficial do Distrito Federal (DODF) using [DODFMiner](https://dodfminer.readthedocs.io/) and manually annotated by volunteers associated with the KnEDLe project.

# Dataset Information

Datasets with info about personnel related acts. These datasets were validated by members of the KnEDLe project and can be used as a gold standard dataset.

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

A [dataset with info about Acts of Retirement](https://github.com/UnB-KnEDLe/datasets/blob/master/atos_aposentadoria.md) was provided by the Tribunal de Contas do Distrito Federal (TCDF);

[More information](https://github.com/UnB-KnEDLe/tutorial_annotation_teamtat) about the annotation process and its labels.

# Version 0
**size:** 13924 rows

## Attibute Information 

|    Attribute  | Description | 
|:-------------:|:-------------------:|
|id_ato         | act identifier |
|id_dodf        | identifier of the DODF from which the act was extracted |
|num_doc_dodf   | number of the DODF from which the act was extracted |
|data_doc_dodf  | data of the DODF from which the act was extracted |
|tipo_rel       | type of the act to which the entity belongs|
|id_rel         | relation-level annotation identifier |
|anotador_rel   | who annotated the relation used to represent the act|
|texto_rel      | full text of the act |
|tipo_ent       |entity type |
|id_ent         | entity-level annotation identifier |
|anotador_ent   | who annotated the entity |
|texto_ent      | entity |

## Files
- [CSV (**Restricted**) ](https://drive.google.com/file/d/1zxM1tDKoNPXgu9z7qdT_m3w5QDFUe1L4/view?usp=sharing)
- [XML (**Restricted**) ](https://drive.google.com/drive/folders/1Ih6YfXn2CnnmBMxXoycS8beihJvIzJZz?usp=sharing)



# Relevant Papers

# Papers That Cite This Dataset
