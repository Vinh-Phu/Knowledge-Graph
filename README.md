# Building a Knowledge Graph via Vietnamese Relation Extraction

With the increasing growth of data, the demand for text retrieval and processing has become increasingly important. In this context, the main objective of this project is to construct a knowledge graph dataset to enhance text querying models for the Vietnamese language. Through this, we aim to build a linked knowledge graph that stores query information through semantic relationships, creating a useful information organizational structure.

# Instruction

### Yêu Cầu

- Python 3.7+
- ```pip isntall requirements.txt```

### Dataset

Please contact VLSP 2020 Organizers for the dataset. You can follow their guide at: https://vlsp.org.vn/resources
And Follow guide Zalo AI challenge for question answering dataset at : https://challenge.zalo.ai/portal/e2e-question-answering

## Usage 

If you have data from VLSP 2020 
run 
`python data_converter.py --overwrite_output_dir --input_dir ./data/VLSP2020_RE_training --output_dir preprocessed_data/VLSP2020_RE_training`

`python data_converter.py --overwrite_output_dir --input_dir ./data/VLSP2020_RE_dev --output_dir preprocessed_data/VLSP2020_RE_dev`

`python semeval_converter.py  --input_dir ./preprocessed_data/VLSP2020_RE_training --output_dir ./data/VLSP2020_RE_SemEvalFormat`

`python semeval_converter.py  --input_dir ./preprocessed_data/VLSP2020_RE_dev --output_dir ./data/VLSP2020_RE_SemEvalFormat`
