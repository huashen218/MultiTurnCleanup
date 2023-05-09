

# MultiTurnCleanup: A Benchmark for Multi-Turn SpokenConversational Transcript Cleanup

MultiTurnCleanup is a targeted dataset for multi-turn spoken conversational transcript cleanup. 

Detailed experiments and analyses can be found in our [paper]().

## Dataset Description
Disfl-QA consists of ~12k disfluent questions with the following train/dev/test splits:
| File      | #Conv   |  #Turns   |   #Tokens   |  #Cleanup  |
|-----|-----|-----|-----|-----|
|Train | 932 | 74k   |  1M  |  132k  |
|Dev  |  86 |  3.7k  | 60k   | 6.1k   |
|Test | 64 | 2.9k   |  43k  |  5k  |
|Sum | 1082 | 81k   |  1.1M  |  143k  |





## Citation
Please cite it as follows:

```
@inproceedings{gupta-etal-2021-disflqa,
    title = "{MultiTurnCleanup: A Benchmark for Multi-Turn SpokenConversational Transcript Cleanup}"
}
```

## License
<!-- MultiTurnCleanup dataset is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). -->

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
