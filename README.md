# BeCat
### You can see your cat version and what breed is!
![VNATMCGQF4CN1IE8NW2IDHUPNK1D441H_0](https://user-images.githubusercontent.com/32739719/146375797-99a76b3b-8675-4b78-b69b-69284a284826.png)

<img width="396" alt="스크린샷 2021-12-16 오후 9 51 53" src="https://user-images.githubusercontent.com/32739719/146375543-8eab5b6b-8c43-449d-9508-e2736051b65c.png">


### 　
### 　


**What is BeCat**
------------

BeCat is model that consists of 2 model. One is Twin-Gan model that is unsupervised image translation model, the other is Classification model that used transfer learning from Resnet50. So, You can use two models at the same time in this project script. 

I was wondering that whether model can do their jobs on generated data. So, I tried. In this project, if you put in human image, Twin-Gan generates artificial cat's image that is similar to human image. And the next, Classification model classifies the cats what breed is. So You can see your cat's version and what breed you are. 

### 　

**Requires**
------------
- python 3.7
- tensorflow 2.0>=
- torchvision
- sklearn
- cv2
- numpy
- pillow
- matplotlib

### 　

**Data**
------------

In this project, the kaggle data used for classification. [Cats and Dogs Breeds Classification Oxford Dataset](https://www.kaggle.com/zippyz/cats-and-dogs-breeds-classification-oxford-dataset/). That dataset consists of cat and dog data. So, I preprocessed the dataset only for cat data. You can access my preprocessed dataset [here](https://drive.google.com/file/d/1WGS4Xo0MmvXFDxHgA-RxKIoJCLfCeXTO/view?usp=sharing). It has 12 breed classes. It is seperated by 8:1:1 for training:validation:test. Or you can use your own data. Plus, if the generated result is awful, check the input image. Cropped image that is focused on face is good for result



### 　

**To use twin-gan**
------------
I modified twin-gan's code to run in tensorflow version 2. So just put this [weight](https://drive.google.com/file/d/1UJEqlH_1sfdmWs6MXKV4H69NGad0rdUB/view) in TwinGan directory. like 'BeCat/twin_gan/TwinGAN/128'. This pretrained model is offered by [Twin-gan](https://github.com/jerryli27/TwinGAN).
Plus, you put your human image in '/TwinGan/Demo/inference_input'. That's it.


### 　

**Training**
------------
If you want to train, Execute the cell in next order. 1_2_3_4_5_6_7_8_9_10.




### 　

**Inference**
------------
If you want to run without train, Execute the cell in next order. 1_2_3_4_5_6_7_10.
And you have to put [this pretrained](https://drive.google.com/file/d/1mIWybmuB12LXGIyGAyqqqvoWzNeu0LGw/view?usp=sharing) in BeCat Directory.




### 　




**Reference**
-------------
[Twin-Gan](https://github.com/jerryli27/TwinGAN)

### 　

**Who** 
------------

**Minkuk Kim**<br/>-Department of computer engineering, Undergraduate, Kyung Hee University<br/>https://github.com/Geppa

