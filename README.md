single task score

|            | Accuracy | Precision | Recall |  F1   |
| :--------: | :------: | :-------: | :----: | :---: |
| aggression |  0.924   |   0.786   | 0.786  | 0.787 |
|   attack   |  0.945   |   0.808   | 0.793  | 0.800 |
|  toxicity  |  0.940   |   0.823   | 0.837  | 0.830 |



multi task score                                                                                                                  model 8600

|            | Accuracy | Precision | Recall |  F1   |
| :--------: | :------: | :-------: | :----: | :---: |
| aggression |  0.928   |   0.822   | 0.760  | 0.790 |
|   attack   |  0.936   |   0.806   | 0.803  | 0.805 |
|  toxicity  |  0.939   |   0.848   | 0.793  | 0.820 |



改进

1. label embedding 用CNN加入了字符信息
2. attention改了激活函数
3. 每个task的loss加上权重后再求和

|            | Accuracy | Precision | Recall |  F1   |
| :--------: | :------: | :-------: | :----: | :---: |
| aggression |  0.930   |   0.830   | 0.763  | 0.795 |
|   attack   |  0.938   |   0.814   | 0.808  | 0.811 |
|  toxicity  |  0.943   |   0.861   | 0.802  | 0.831 |