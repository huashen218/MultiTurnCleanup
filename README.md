
# MultiTurnCleanup: A Benchmark for Multi-Turn Spoken Conversational Transcript Cleanup

[![Arxiv](https://img.shields.io/badge/Arxiv-2304.01002-blue)](https://arxiv.org/pdf/2304.01002.pdf)
[![Data](https://img.shields.io/badge/Data-.tsv-red)](https://github.com/huashen218/MultiTurnCleanup)

This repository includes the MultiTurnCleanup dataset and [paper](https://arxiv.org/abs/2305.12029) accepted in the [EMNLP 2023](https://2023.emnlp.org/program/) main conference.

MultiTurnCleanup is a targeted dataset for multi-turn spoken conversational transcript cleanup. 
Detailed experiments and analyses can be found in our [paper](https://hua-shen.org/assets/files/google_multi_turn_cleanup.pdf).



## Citation
If you find this repo helpful to your research, please cite the paper:

```
@article{shen2023multiturncleanup,
  title={MultiTurnCleanup: A Benchmark for Multi-Turn Spoken Conversational Transcript Cleanup},
  author={Shen, Hua and Zayats, Vicky and Rocholl, Johann C and Walker, Daniel D and Padfield, Dirk},
  journal={arXiv preprint arXiv:2305.12029},
  year={2023}
}
```

## Dataset Description
MultiTurnCleanup consists of ~143k multi-turn cleanup labels with the following train/dev/test splits:
| File      | #Conv   |  #Turns   |   #Tokens   |  #Cleanup  |
|-----|-----|-----|-----|-----|
|Train | 932 | 74k   |  1M  |  132k  |
|Dev  |  86 |  3.7k  | 60k   | 6.1k   |
|Test | 64 | 2.9k   |  43k  |  5k  |
|**Sum** | **1082** | **81k**   |  **1.1M**  |  **143k**  |





## License
MultiTurnCleanup dataset is licensed under [LDC](https://www.ldc.upenn.edu/data-management/using/licensing).



## Contact

Please create an issue in this repository or contact the authors directly.





<!-- 

Each CSV file consists of original question (SQuAD-v2) and disfluent question (Disfl-QA) in the following format:
```
{ 
  "squad_v2_id":
  {
    "original": Original question from SQuAD-v2,
    "disfluent": Disfluent question from Disfl-QA
  }, ...
}
```
**Note**: The `squad_v2_id` corresponds to the unique  `data.paragraphs.qas.id` in SQuAD-v2 development set.  

Here's an example from the dataset:
```json
 {
  "56ddde6b9a695914005b9628": {
    "original": "In what country is Normandy located?",
    "disfluent": "In what country is Norse found no wait Normandy not Norse?"
  },
  "56ddde6b9a695914005b9629": {
    "original": "When were the Normans in Normandy?",
    "disfluent": "From which countries no tell me when were the Normans in Normandy?"
  },
  "56ddde6b9a695914005b962a": {
    "original": "From which countries did the Norse originate?",
    "disfluent": "From which Norse leader I mean countries did the Norse originate?"
  },
  "56ddde6b9a695914005b962b": {
    "original": "Who was the Norse leader?",
    "disfluent": "When I mean Who was the Norse leader?"
  },
  "56ddde6b9a695914005b962c": {
    "original": "What century did the Normans first gain their separate identity?",
    "disfluent": "When no what century did the Normans first gain their separate identity?"
  },
 }
``` -->
