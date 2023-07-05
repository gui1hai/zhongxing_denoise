## 2022 中兴捧月大赛（多媒体赛道）-图像去噪Uformer

### Tree  
demo_code/  
data/  
|-- dataset/  
|-- |-- ground truth/  
|-- |-- noisy/  
|-- result/  
|-- |-- algorithm/  
|-- |-- data/  
|-- testset/  
|-- valset/  
|-- |-- ground truth/  
|-- |-- noisy/  
models/  

### Train  
python train.py  
### Test  
cd ..  
python ./demo_code/testTorch.py --input_path data/testset/ --ground_path data/testset/  
python ./demo_code/testTorch.py --input_path ./data/valset/noisy/ --ground_path ./data/valset/ground_truth/  
### 图像有点大，在cpu上进行测试的  
### 模型训练加载好多次得到最后的结果  
