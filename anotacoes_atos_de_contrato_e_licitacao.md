

# Source

Data extracted from the Diário Oficial do Distrito Federal (DODF)  and manually annotated and reviewed by undergraduate students associated with the KnEDLe project.

# Dataset Information

Datasets with with labeled entities. These datasets were validated and reviewed by members of the KnEDLe project and can be used as a gold standard dataset.

# Labeled Acts
**size:** 1168 rows

Manually labeled acts consisting of Extratos de Contrato, Aditamento Contratual, Aviso de Licitação, Aviso de Suspensão de Licitação and Aviso de Revogação/Anulação de Licitação. The labeled entities were made upon those labeled texts.

## Attribute Information 

|    Attribute  | Description | 
|:-------------:|:-------------------:|
|file_id        | file used during the labeling process |
|dodf_id        | DODF edition in which the act is located |
|act_type       | act's type to which the entity is related |
|raw_text       | raw text used in the labeling process |
|treated_text   | treated text of the labeling process|
|labeler_act    | labeler's name of the act |
|reviewer_act   | reviewer's name of the labeled act |

## Number of Labeled Acts

|    Class                                    | Quantity | 
|:-------------------------------------------:|:--------:|
|aviso_de_aditamento_contratual               |       463|
|extrato_de_contrato_ou_convenio              |       442|
|aviso_de_licitacao                           |       235|
|aviso_de_revogacao_anulacao_de_licitacao     |        16|
|aviso_de_suspensao_de_licitacao              |        12|
|Total                                        |      1168|

## Files
- [PARQUET](https://drive.google.com/file/d/1NJC58r89eJ58aJxA6LIKehahujqlK8tV/view?usp=sharing)

# Labeled Entities
**size:** 7946 rows

Manually labeled entities.

## Attribute Information 

|    Attribute  | Description | 
|:-------------:|:-------------------:|
|file_id        | file used during the labeling process |
|act_type       | act's type to which the entity is related |
|title_ent      | entity title |
|val_ent        | entity value |
|text_ent       | entity text|
|loc_begin      | begining position of the entity in the act text (attribute raw_text) |
|loc_end        | ending position of the entity in the act text (attribute raw_text) |
|labeler_ent    | labeler's name of the entity |
|reviewer_ent   | reviewer's name of the labeled entity |

## Number of Labeled Entities

|    Class                                             | Quantity | 
|:----------------------------------------------------:|:--------:|
|Órgão contratante                                     |       857|
|Processo do GDF                                       |       664|
|Objeto do aditamento contratual                       |       460|
|Número do contrato                                    |       457|
|Objeto do ajuste                                      |       442|
|Número do ajuste                                      |       432|
|Entidade contratada                                   |       413|
|Número do termo aditivo                               |       412|
|Vigência do ajuste                                    |       408|
|Data de assinatura do ajuste                          |       381|
|Valor do ajuste                                       |       348|
|Programa de trabalho                                  |       277|
|Modalidade de licitação                               |       265|
|Número da licitação                                   |       264|
|Objeto da licitação                                   |       236|
|Nota de empenho                                       |       234|
|Tipo de objeto                                        |       225|
|Natureza da despesa                                   |       211|
|Data de abertura da licitação                         |       209|
|Código da unidade orçamentária                        |       184|
|Sistema de compras utilizado                          |       173|
|Número da licitação que gerou o contrato              |       124|
|Valor estimado da contratação                         |        71|
|Órgão/entidade licitante                              |        50|
|Código da licitação no sistema de compras utilizado   |        43|
|Entidades convenentes                                 |        31|
|Fundamento legal da dispensa ou inexigibilidade       |        30|
|Identificação de dispensa                             |        24|
|Identificação revogação/anulação                      |        16|
|Decisão do TCDF que determinou a suspensão            |         2|
|Prazo da suspensão                                    |         2|
|Órgão gerenciador da ata                              |         1|
|Total                                                 |      7946|

## Files
- [PARQUET](https://drive.google.com/file/d/1HQ48kPD0erHNZDtFX3TKfWryC5jvYleV/view?usp=sharing)


# Tokenized Acts
**size:** 1168 rows

Tokenized texts of acts, based on the labeled entities.

The IOB tagging was made with all types of acts and all listed entities. The script in which the tagging was made is located at [here](https://github.com/UnB-KnEDLe/experiments/blob/master/members/ciriatico/ground_truth_dataset/iob_labeled_entities.ipynb), and it can be changed using the Labeled Acts and Labeled Entities dataset.

## Attribute Information 

|    Attribute     | Description | 
|:----------------:|:-------------------:|
|file_id           | file used during the labeling process |
|tokenized_text    | list of tokenized words of the act text |
|text              | treated text used for the tokenization |

## Tokenized Entities

| Act Type                                    | Entity Label                                           |                         Token | 
|:--------------------------------------------|-------------------------------------------------------:|:-----------------------------:|
|Extrato de contrato                          | Processo do GDF                                        |                       PROCESSO|
|Extrato de contrato                          | Número do ajuste                                       |                     NUM_AJUSTE|
|Extrato de contrato                          | Órgão contratante                                      |                    CONTRATANTE|
|Extrato de contrato                          | Entidade contratada                                    |                     CONTRATADA|
|Extrato de contrato                          | Entidades convenentes                                  |                     CONVENENTE|
|Extrato de contrato                          | Objeto do ajuste                                       |                     OBJ_AJUSTE|
|Extrato de contrato                          | Data de assinatura do ajuste                           |                DATA_ASSINATURA|
|Extrato de contrato                          | Vigência do ajuste                                     |                       VIGENCIA|
|Extrato de contrato                          | Valor do ajuste                                        |                          VALOR|
|Extrato de contrato                          | Código da unidade orçamentária                         |                      CODIGO_UO|
|Extrato de contrato                          | Programa de trabalho                                   |                             PT|
|Extrato de contrato                          | Natureza da despesa                                    |                             ND|
|Extrato de contrato                          | Nota de empenho                                        |                             NE|
|Extrato de contrato                          | Órgão/entidade licitante                               |                ORGAO_LICITANTE|
|Extrato de contrato                          | Número da licitação que gerou o contrato               |                  NUM_LICITACAO|
|Extrato de contrato                          | Órgão gerenciador da ata                               |                         OG_ATA|
|Extrato de contrato                          | Identificação de dispensa                              |                 IDENT_DISPENSA|
|Extrato de contrato                          | Fundamento legal da dispensa ou inexigibilidade        |                  FUND_DISPENSA|
|Aditamento contratual                        | Órgão contratante                                      |                    CONTRATANTE|
|Aditamento contratual                        | Número do contrato                                     |                   NUM_CONTRATO|
|Aditamento contratual                        | Número do termo aditivo                                |                    NUM_ADITIVO|
|Aditamento contratual                        | Objeto do aditamento contratual                        |                    OBJ_ADITIVO|
|Aviso de licitação                           | Órgão/entidade licitante                               |                ORGAO_LICITANTE|
|Aviso de licitação                           | Número da licitação                                    |                  NUM_LICITACAO|
|Aviso de licitação                           | Objeto da licitação                                    |                  OBJ_LICITACAO|
|Aviso de licitação                           | Modalidade de licitação                                |           MODALIDADE_LICITACAO|
|Aviso de licitação                           | Processo do GDF                                        |                       PROCESSO|
|Aviso de licitação                           | Valor estimado da contratação                          |                 VALOR_ESTIMADO|
|Aviso de licitação                           | Data de abertura da licitação                          |                  DATA_ABERTURA|
|Aviso de licitação                           | Sistema de compras utilizado                           |                SISTEMA_COMPRAS|
|Aviso de licitação                           | Código da licitação no sistema de compras utilizado    |         CODIGO_SISTEMA_COMPRAS|
|Aviso de licitação                           | Tipo de objeto                                         |                       TIPO_OBJ|
|Aviso de revogação/anulação de licitação     | Órgão/entidade licitante                               |                ORGAO_LICITANTE|
|Aviso de revogação/anulação de licitação     | Número da licitação                                    |                  NUM_LICITACAO|
|Aviso de revogação/anulação de licitação     | Modalidade de licitação                                |           MODALIDADE_LICITACAO|
|Aviso de revogação/anulação de licitação     | Identificação revogação/anulação                       |       IDENT_REVOGACAO_ANULACAO|
|Aviso de suspensão de licitação              | Órgão/entidade licitante                               |                ORGAO_LICITANTE|
|Aviso de suspensão de licitação              | Número da licitação                                    |                  NUM_LICITACAO|
|Aviso de suspensão de licitação              | Modalidade de licitação                                |           MODALIDADE_LICITACAO|
|Aviso de suspensão de licitação              | Prazo da suspensão                                     |                PRAZO_SUSPENSAO|
|Aviso de suspensão de licitação              | Decisão do TCDF que determinou a suspensão             |                   DECISAO_TCDF|

## Files
- [PARQUET](https://drive.google.com/file/d/1I3rpmr3oIZvGVF2VBlua1kwVuY7rGo3B/view?usp=sharing)

# Relevant Papers

# Papers That Cite This Dataset
