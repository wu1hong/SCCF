The batch sizes are specified in the following table:

| Model | Beauty | Gowalla | Yelp2018 | Pinterest |
|-------|--------|---------|----------|-----------|
| BPR   | 256    | 256     | 256      | 256       |
| DAU   | 256    | 1024    | 1024     | 1024      |
| SCCF  | 10000  | 100000  | 100000   | 60000     |

For DAU, we follow the setting of the original paper.


We also provide how the batch size affects SCCF performance on the Amazon-Beauty dataset.

| Batch size | Recall@20 | NDCG@20 |
|------------|-----------|---------|
| 4096       | 0.1427    | 0.0699  |
| 10000      | 0.1470    | 0.0713  |
| 60000      | 0.1507    | 0.0729  |
