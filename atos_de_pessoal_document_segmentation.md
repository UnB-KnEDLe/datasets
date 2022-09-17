# Source

Data extracted from the [Anotações - Atos de Pessoal](https://github.com/UnB-KnEDLe/datasets/blob/master/corpus_2_contratos_licitacoes.md) dataset, using data extracted from the Diário Oficial do Distrito Federal (DODF) using [DODFMiner](https://dodfminer.readthedocs.io/) and manually annotated by volunteers associated with the KnEDLe project.

# Dataset Information

Datasets with info about personnel related acts. The acts serve as sections of the document segmenation. These datasets were validated by members of the KnEDLe project.

The acts considered and their respective labels are presented below:

|                   Act                   |              Label              | 
|:---------------------------------------:|:-------------------------------:|
|Abono de Permanênica                     | Ato_Abono_Permanencia           |
|Cessão                                   | Ato_Cessao                      |
|Exoneração Comissionado                  | Ato_Exoneracao_Comissionado     |
|Exoneração Efetivo                       | Ato_Exoneracao_Efetivo          |
|Nomeação Comissionado                    | Ato_Nomeacao_Comissionado       |
|Nomeação Efetivo                         | Ato_Nomeacao_Efetivo            |
|Retificação Comissionado                 | Ato_Retificacao_Comissionado    |
|Retificação Efetivo                      | Ato_Retificacao_Efetivo         |
|Reversão                                 | Ato_Reversao                    |
|Substituição                             | Ato_Substituicao                |
|Tornado Sem Efeito Apo                   | Ato_Tornado_Sem_Efeito_Apo      |
|Tornado Sem Efeito Exo/Nom               | Ato_Tornado_Sem_Efeito_Exo_Nom  |

[More information](https://github.com/UnB-KnEDLe/tutorial_anotacao_contratos_licitacoes) about the annotation process and its labels.

# Version 0
**size:** 9058 rows

Annotations from Batch X. 

## Attribute Information 

|    Attribute  | Description                               | 
|:-------------:|:-----------------------------------------:|
|type_act       | type of the act to which the text belongs |
|text           | text of the annotated act                 |
|n_dodf         | number of the DODF's edition              |
|day            | day the document was published            |
|month          | month the document was published          |
|year           | year the document was published           |

## Number of Labeled Acts

|    Type                           | Quantity | 
|:---------------------------------:|:--------:|
| Ato_Abono_Permanencia             |       134|
| Ato_Cessao                        |       265|
| Ato_Exoneracao_Comissionado       |      2009|
| Ato_Exoneracao_Efetivo            |       241|
| Ato_Nomeacao_Comissionado         |      2313|
| Ato_Nomeacao_Efetivo              |        46|
| Ato_Retificacao_Comissionado      |       198|
| Ato_Retificacao_Efetivo           |      1214|
| Ato_Reversao                      |        58|
| Ato_Substituicao                  |      2312|
| Ato_Tornado_Sem_Efeito_Apo        |        20|
| Ato_Tornado_Sem_Efeito_Exo_Nom    |       248|
|Total                              |      9058|

## Files
- [CSV (**Public**) ](X)

# Relevant Papers
