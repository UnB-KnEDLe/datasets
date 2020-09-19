


[Download (segmentation_aposentadoria.zip)](https://drive.google.com/drive/folders/1Uq7jslcHH21FCChhpw_8MTdU3tMfUlRI)


# Source

Ground truth provided by TCDFT (Tribunal de Contas do Distrito Federal e Territórios)

Preprocessing done by: 
- José Reinaldo da C. S. A. V. da S. Neto

# Dataset Information
- Dataset with annotated retirement segments (A retirement act may be composed of multiple sentences).
- To create this dataset we split DODFs into blocks using the DODFminer extraction option -blocks. Each block is split into sentences (separated by '.' characters) and those sentences related to a retirement act are annotated.

*Note: Data wasn't split into train-valid-test sets (I forgot, will do later)*

**Format:**
Similar to the CoNLL format, each line in the txt file will consist of a label (I, O, B) followed by space, followed by a sentence that corresponds to that tag. Empty lines indicate end of a block (sequence of sentences).

Example:

"B hoje eu vou a faculdade" -> tag is "B", sentence is "hoje eu vou a faculdade"

*Important: There are blocks in many DODFs where '.' characters are adjacent to each other (and during sentence splitting it returns an empty list) and that makes it so that some lines in the dataset come with a tag followed by only space characters*

**size:** 
- full dataset: 214574 blocks 

# Attribute Information
The number of entities per class in each set (train/test) are presented below:

| Tags |                     Meaning                    | Frequency on the dataset |
|:----:|:----------------------------------------------:|:------------------------:|
|   B  |  Sentence is the beggining of a retirement act |           5.382          |
|   I  | Sentence is a continuation of a retirement act |           16.107         |
|   O  |     Sentence isn't part of a retirement act    |          1.714.904       |

# Relevant Papers

# Papers That Cite This Dataset
