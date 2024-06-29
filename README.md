# Unifying Graph Convolution and Contrastive Learning in Collaborative Filtering
The paper was accepted by SIGKDD 2024.

In this paper, we show the equivalence of graph convolutions and contrastive learning in collaborative filtering. Furthermore, we show naive embeddings with contrastive loss exhibit strong performance compared with GNN based models in collaborative filtering.

Below is the code for reproduction with the default hyperparameters.
```
# Amazon-Beauty
python run_recbole.py --model=SCCF --dataset=Beauty --learning_rate=10 --encoder=MF --train_batch_size=10000 --embedding_size=64 --learner='sgd' --temperature=0.25 --stopping_step=100
# Gowalla
python run_recbole.py --model=SCCF --dataset=Gowalla --learning_rate=10 --encoder=MF --train_batch_size=100000 --embedding_size=64 --learner='sgd' --temperature=0.1 --stopping_step=100
# Yelp
python run_recbole.py --model=SCCF --dataset=Yelp --learning_rate=10 --encoder=MF --train_batch_size=100000 --embedding_size=64 --learner='sgd' --temperature=0.2 --stopping_step=100
# Pinterest
python run_recbole.py --model=SCCF --dataset=pinterest --learning_rate=10 --encoder=MF --train_batch_size=60000 --embedding_size=64 --learner='sgd' --temperature=0.1 --stopping_step=100
```
For more detail, please refer to our paper. If you like our work, please cite
```
@article{wu2024unifying,
  title={Unifying Graph Convolution and Contrastive Learning in Collaborative Filtering},
  author={Wu, Yihong and Zhang, Le and Mo, Fengran and Zhu, Tianyu and Ma, Weizhi and Nie, Jian-Yun},
  journal={arXiv preprint arXiv:2406.13996},
  year={2024}
}
```
