# SKIN_GCN
Skin-detection(Using GCN)
## Copyright / End User License
* SFA (Skin-nonSkin dataset) - Citation : CASATI, J. P. B. ; MORAES, D. R. ; RODRIGUES, E. L. L. . SFA: A Human Skin Image Database based on FERET and AR Facial Images. In: IX Workshop de Visão Computacional, 2013, Rio de Janeiro. Anais do VIII Workshop de Visão Computacional, 2013.
* If you want to use this Dataset, go to URL : http://www.sel.eesc.usp.br/sfa/ (I don`t upload the SFA file Because it could be a problem)
* I am currently writting a paper with this code, If it is completed, I will also post my thesis
## Contact Information
* qazw5741@naver.com & YangChangHee2251@gamil.com
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
