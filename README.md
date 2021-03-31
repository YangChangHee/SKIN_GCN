# SKIN_GCN
Skin-detection(Using GCN)
## Copyright / End User License
* SFA (Skin-nonSkin dataset) - Citation : CASATI, J. P. B. ; MORAES, D. R. ; RODRIGUES, E. L. L. . SFA: A Human Skin Image Database based on FERET and AR Facial Images. In: IX Workshop de Visão Computacional, 2013, Rio de Janeiro. Anais do VIII Workshop de Visão Computacional, 2013.
* If you want to use this Dataset, go to URL : http://www.sel.eesc.usp.br/sfa/ (I don`t upload the SFA file Because it could be a problem)
* I am currently writting a paper with this code, If it is completed, I will also post my thesis
* If you use it commercially, please contact my email, If you use it in github or other open source in a project, please provide a source.
## Contact Information
* qazw5741@naver.com & YangChangHee2251@gamil.com
## Installation Process
* numpy
* matplotlib
* pandas
* tqdm
* pytorch
* hashlib
* json
* os
* torchvision
* argparse
* seaborn
## Directions for use
* Step 1. Make_dataset (https://github.com/YangChangHee/SKIN_GCN/blob/main/Make_dataset/step%201.%20make%20dataset.ipynb)

Check SFA file and make adjacency Matrix

3-dimension RGB =>(Convert) 5-dimension R,G,B,Cb,Cr


adjacency Matrix => ![adjacency Matrix](https://user-images.githubusercontent.com/59610723/113120090-2de3b680-924c-11eb-8e1f-52a20d833be8.jpg)

* Step 2. make_parameta (https://github.com/YangChangHee/SKIN_GCN/blob/main/make_parameta/step%202.%20make_parameta.ipynb)

I put a neighboring matrix in class

Change Markdown to code to see how dimensions decrease

If you look at In[5], In[6], (making random matrix)Apply parameta

* Step 3. test_basic model (https://github.com/YangChangHee/SKIN_GCN/blob/main/make_parameta/step%203.%20test_basic%20model.ipynb)

The GPU used is the RTX-2080TI

I Checked Whether Step1 and Step2 can be used properly.

* Step 4. Large data make datafile (https://github.com/YangChangHee/SKIN_GCN/blob/main/Make_dataset/step%204.%20large%20data%20make%20datafile.ipynb

The data we will use should be refined. So we use a new data form , .npy

The back is a method of applying the loaded data to the model

* Step 5. load data and model define (https://github.com/YangChangHee/SKIN_GCN/blob/main/Define_Model/step%205.%20load%20data%20and%20model%20define.ipynb)

I tried increasing the model hidden dims

Tqdm was used to determine how long the traing took

Finally, we applied it to the general image.

* Step 6. GCN deep (https://github.com/YangChangHee/SKIN_GCN/blob/main/Define_Model/step%206.%20GCN%20deep.ipynb)

Increasing model hidden dims(2 => 3)

* Step 7. GCN Result (https://github.com/YangChangHee/SKIN_GCN/blob/main/%EB%B3%B4%EA%B3%A0%EC%84%9C/Step%207.%20GCN%20Result.ipynb)

Hidden dim 1 => [10], Hidden dim 2 => [15, 20, 25, 30], Hidden dim 3 => [20, 30, 40, 50]


Result 


![1](https://user-images.githubusercontent.com/59610723/113123551-a7c96f00-924f-11eb-84b1-5ac032200988.png)
![2](https://user-images.githubusercontent.com/59610723/113123572-ab5cf600-924f-11eb-9ed1-ba92f9f893c5.png)
![3](https://user-images.githubusercontent.com/59610723/113123586-ae57e680-924f-11eb-9c20-0d20f7aff7a6.png)



* Step 8. GCN Result (https://github.com/YangChangHee/SKIN_GCN/blob/main/%EB%B3%B4%EA%B3%A0%EC%84%9C/Step%208.%20GCN%20Result.ipynb)

Add Visualize Function 

Result (Change Imagesize [imagesize] => [180,180])

![4](https://user-images.githubusercontent.com/59610723/113123899-eeb76480-924f-11eb-9e53-a1257b818a59.png)

