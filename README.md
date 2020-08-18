# data-augmentation-0818



<br><br>
### 1.original data + timestretch
#### [DenseNet0818.ipynb](https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/DenseNet0818.ipynb)
<br>

<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/data.png" height=500px width=700px> </img>


처음 zero padding 된 data 1000개 + zero padding 제거한 data 1000개로 학습한 결과입니다.
<br>
training data : 1800개
validation data : 200개
<br><br>
training<br>
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/training_dataset_confusion_matrix.png" height=400px width=450px> </img>
96.750%
<br>
validation<br>
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/validation_dataset_confusion_matrix.png" height=400px width=450px> </img>
93.000%
<br><br><br>



### 2. timestretch + reversed data
#### [inputdata.ipynb](https://github.com/Kang-Dong-Hwi/data-augmentation/blob/master/inputdata.ipynb)
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/data2.png" height=1200px width=700px> </img>


처음 zero padding 된 data 1000개 + zero padding 제거한 data 1000개 + 좌우반전 data 2000개<br>
총 4000개로 학습한 결과입니다.
<br>
training data : 3800개
validation data : 200개
<br><br>
training<br>
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/training_dataset_confusion_matrix2.png" height=400px width=450px> </img>
99.1667%
<br>
validation<br>
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/validation_dataset_confusion_matrix2.png" height=400px width=450px> </img>
97.000%
<br><br><br>



### 3. phase제거

2. 4000개 data에서 left, right magnitude만 입력으로 해 주었을 때 결과입니다.<br>
                  (4000, 2, 257, 382)
<br>
training data : 3800개
validation data : 200개
<br><br>
training<br>
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/training_dataset_confusion_matrix2-1.png" height=400px width=450px> </img>
99.1053%
<br>
validation<br>
<img src="https://github.com/Kang-Dong-Hwi/data-augmentation-0818/blob/master/Screenshots/validation_dataset_confusion_matrix2-1.png" height=400px width=450px> </img>
95.000%
<br><br><br>

