# Supplementary materials

### SAI dataset (related to Section 1)
Sample images of SAI dataset. Red rectangles indicate the location of the defective region. The upper row is for normal cases, and the lower row is for defect cases for each inspection class. (a) Sim Tray, (b) Cam Hole, (c) USB Hole, (d) Ear Hole, (e) Spk Hole, (f) Mic Hole (inside), (g) Mic Hole (outside), (h) Edge

![GitHub Logo](/figure1.png)


### Consturcting reference interpretation (RI) during the training process (related to Section 3)
We extracted Grad-CAMs from ResNet-50 trained by SAI dataset, and RI was constructed by averaging Grad-CAMs of negative samples.
We observed four RI from layer 10, 22, 40 and 49 each epoch. (a) RI from layer49, (b) RI from layer40, (c) RI from layer22, (d) RI from layer10.

![GitHub Logo](/figure2.png)


### Other visualization results for interpretation consistency (related to Section 3)
1-D Plot for the DoI distributions of negative and positive samples. (a) Training data. (b) Test data. We can observe how two distributions are separated and formed according to training progress. 

![GitHub Logo](/figure7.png)

Grad-CAM visualizations for Spk Hole class. M(i) indicates Grad-CAM from i-th layer. (a) Negative. (b)  Positive. 

![GitHub Logo](/figure8.png)


### Grad-CAMs of the defective samples from the proposed model (related to Section 3)
We can see that Grad-CAM activates on the defective region. Grad-CAMs are activated in a narrow region from a wide region as it proceeds from layer49 to layer10 (Fine to coarse).

![GitHub Logo](/figure3.png)


### Comparison of confusion matrix between baseline and the proposed method (related to Section 5)
Confusion matrices for test dataset at 25% supervision. (a) Baseline, (b) Proposed method. 0 and 1 indicate negative and positive, respectively. Most critical error in industrial visual inspection task is false negative which means the failure of detecting defects because the primary objective of an inspection is to detect defective product to avoid delivering it to the customer. From these confusion matrices, we have overall 46 FNs over 408 samples (11.3%) with baseline, 31 FNs (7.6%) with the proposed method.

![GitHub Logo](/figure4.png)


### Comparison with VAT (related to Section 5)
AUC scores between the proposed method and VAT on supervision ratio 25%, 50%, and 75%. Our method outperforms VAT 5.7%, 6.4%, and 5.9%, respectively.

![GitHub Logo](/figure5.png)
![GitHub Logo](/figure6.png)


### Ablation study about L (related to Section 5)
We defined the set of layer L for extracting Grad-CAM from the model. We used L={10,22,40,49} for the standard settings of the experiments. In this section, the following results show the ablation studies about L.
When we use more layers for extracting Grad-CAM, performance increase slightly (1.6%, +0.015) from L={49} to L={10,22,40,49}. 

![GitHub Logo](/figure9.png)
![GitHub Logo](/figure10.png)
