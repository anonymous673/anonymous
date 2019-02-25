# Supplementary materials

### SAI dataset
Sample images of SAI dataset. Red rectangles indicate the location of the defective region. Upper row is for normal cases and lower row is for defect cases for each inspection class. (a) Sim Tray, (b) Cam Hole, (c) USB Hole, (d) Ear Hole, (e) Spk Hole, (f) Mic Hole (inside), (g) Mic Hole (outside), (h) Edge

![GitHub Logo](/figure1.png)


### Consturcting reference interpretation (RI) during the training process
We extracted Grad-CAMs from ResNet-50 trained by SAI dataset, and RI was constructed by averaging Grad-CAMs of negative samples.
We observed four RI from the layer 10, 22, 40 and 49 each epoch. (a) RI from layer49, (b) RI from layer40, (c) RI from layer22, (d) RI from layer10.

![GitHub Logo](/figure2.png)


### Grad-CAMs of the defective samples from the proposed model
We can see that Grad-CAM activates on the defective region. Grad-CAMs are activated in a narrow region from a wide region as it proceeds from layer49 to layer10 (Fine to coarse).

![GitHub Logo](/figure3.png)
