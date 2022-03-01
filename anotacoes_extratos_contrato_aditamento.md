

# Source

Data extracted from the Diário Oficial do Distrito Federal (DODF)  and manually annotated and reviewed by undergraduate students associated with the KnEDLe project.

# Dataset Information

Datasets with with labeled entities of acts of contract and contract amendment texts. These datasets were validated and reviewed by members of the KnEDLe project and can be used as a gold standard dataset.

# Labeled Acts
**size:** 948 rows

Manually labeled acts consisting of Acts of Contract and Contract Amendment. The labeled entities were made upon those labeled texts.

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

|    Class                              | Quantity | 
|:-------------------------------------:|:----:|
|extrato_de_contrato_ou_convenio        |   475|
|extrato_de_aditamento_contratual       |   256|
|aviso_de_aditamento_contratual         |   217|
|Total                                  |   948|

*Note: "extrato_de_aditamento_contratual" and "aviso_de_aditamento_contratual" have the same entities and are viewed both as Contract Amendment.*

## Files
- [PARQUET](https://drive.google.com/file/d/1pFbMpH7JR8KJ292oPuRDQ1jb_VxC3NKv/view?usp=sharing)

# Labeled Entities
**size:** 6499 rows

Manually labeled entities of Acts of Contract and Contract Amendment texts.

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

|    Class                                          | Quantity | 
|:-------------------------------------------------:|:----:|
|Órgão contratante                                  |   896|
|Número do contrato                                 |   491|
|Objeto do ajuste                                   |   472|
|Objeto do aditamento contratual                    |   472|
|Processo do GDF                                    |   464|
|Número do ajuste                                   |   442|
|Entidade contratada                                |   442|
|Vigência do ajuste                                 |   433|
|Número do termo aditivo                            |   426|
|Data de assinatura do ajuste                       |   404|
|Valor do ajuste                                    |   369|
|Programa de trabalho                               |   293|
|Nota de empenho                                    |   248|
|Natureza da despesa                                |   223|
|Código da unidade orçamentária                     |   196|
|Número da licitação que gerou o contrato           |   131|
|Entidades convenentes                              |    31|
|Fundamento legal da dispensa ou inexigibilidade    |    31|
|Dispensa de licitação                              |    13|
|Dispensa de inexigibilidade                        |    12|
|Número da licitação                                |     4|
|Órgão/entidade licitante                           |     3|
|Órgão gerenciador da ata                           |     1|
|Data de abertura da licitação                      |     1|
|Objeto da licitação                                |     1|
|Total                                              |  6499|

## Files
- [PARQUET](https://drive.google.com/file/d/1mUlsF0_tqnG5haaZB6W_onwxYHbq1MTL/view?usp=sharing)


# Tokenized Acts
**size:** 943 rows

Tokenized texts of acts, based on the labeled entities.

## Attribute Information 

|    Attribute     | Description | 
|:----------------:|:-------------------:|
|file_id           | file used during the labeling process |
|tokenized_text    | list of tokenized words of the act text |
|text              | treated text used for the tokenization |

## Tokenized Entities

| Act Type                        | Entity Label                                       |            Token | 
|:--------------------------------|---------------------------------------------------:|:----------------:|
|Extrato de contrato              | Processo do GDF                                    |          PROCESSO|
|Extrato de contrato              | Número do ajuste                                   |        NUM_AJUSTE|
|Extrato de contrato              | Órgão contratante                                  |       CONTRATANTE|
|Extrato de contrato              | Entidade contratada                                |        CONTRATADA|
|Extrato de contrato              | Entidades convenentes                              |        CONVENENTE|
|Extrato de contrato              | Objeto do ajuste                                   |        OBJ_AJUSTE|
|Extrato de contrato              | Data de assinatura do ajuste                       |   DATA_ASSINATURA|
|Extrato de contrato              | Vigência do ajuste                                 |          VIGENCIA|
|Extrato de contrato              | Valor do ajuste                                    |             VALOR|
|Extrato de contrato              | Código da unidade orçamentária                     |         CODIGO_UO|
|Extrato de contrato              | Programa de trabalho                               |                PT|
|Extrato de contrato              | Natureza da despesa                                |                ND|
|Extrato de contrato              | Nota de empenho                                    |                NE|
|Extrato de contrato              | Órgão/entidade licitante                           |   ORGAO_LICITANTE|
|Extrato de contrato              | Número da licitação que gerou o contrato           |     NUM_LICITACAO|
|Extrato de contrato              | Órgão gerenciador da ata                           |            OG_ATA|
|Extrato de contrato              | Identificação de dispensa                          |    IDENT_DISPENSA|
|Extrato de contrato              | Fundamento legal da dispensa ou inexigibilidade    |     FUND_DISPENSA|
|Aditamento contratual            | Órgão contratante                                  |       CONTRATANTE|
|Aditamento contratual            | Número do contrato                                 |      NUM_CONTRATO|
|Aditamento contratual            | Número do termo aditivo                            |       NUM_ADITIVO|
|Aditamento contratual            | Objeto do aditamento contratual                    |       OBJ_ADITIVO|

## Files
- [PARQUET](https://drive.google.com/file/d/1M1nRD9GZvJlbz5wFLfvJRuzjFDaypvtL/view?usp=sharing)

# Relevant Papers

# Papers That Cite This Dataset
