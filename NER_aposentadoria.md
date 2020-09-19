


[Download (NER_aposentadoria.zip)](https://drive.google.com/drive/folders/1Uq7jslcHH21FCChhpw_8MTdU3tMfUlRI)




# Source

Ground truth provided by TCDFT (Tribunal de Contas do Distrito Federal e Territórios)

Preprocessing done by: 
- José Reinaldo da C. S. A. V. da S. Neto
- Leonardo Maffei

# Dataset Information
- Dataset with retirement related named entity annotations in CoNLL format. 
- Train-test split was done in chronological order of DODFs, so as to not split entities of the same DODF into different sets. 

*Note: If validation set is required, do not shuffle the training set for the split to prevent spliting sentences of the same DODF into different sets.*


**size:** 
- train set: 3861 sentences
- test set: 1655 sentences

# Attribute Information
The number of entities per class in each set (train/test) are presented below:

|    Entity types   | Number on train set | Number on test set |
|:-----------------:|:-------------------:|:------------------:|
|        ATO        |         3860        |        1655        |
|      NOME_ATO     |         3861        |        1655        |
| COD_MATRICULA_ATO |         3853        |        1654        |
|       CARGO       |         3851        |        1655        |
|       CLASSE      |         1912        |         835        |
|       PADRAO      |         3471        |        1488        |
|     FUND_LEGAL    |         3861        |        1654        |
|      PROCESSO     |         3575        |        1638        |
|       QUADRO      |         3535        |        1500        |
|    EMPRESA_ATO    |         1717        |         788        |

# Relevant Papers

# Papers That Cite This Dataset
