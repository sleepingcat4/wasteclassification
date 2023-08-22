## Introduction

 A YOLOv5 model trained on modified **TACO** dataset to perform object detection on waste and rubbish. Receiving an accuracy as high as *87.6%*, it can confidently predict a wide variety of recyclable rubbish lying around us.  

### How was it trained? 

Modified official YOLOv5 training script was used to train the model, for 100 Epochs. **(Best results are at 200)** 

##### Releasing weights and models

In the repository, I have attached the trained weights in the form of ```“best.pt”``` file, which was later used to perform inference via ```torch.load```. 

And a number of different flavours of saved versions of the model was attached with this repository as well. 

### Dataset
We used a modified TACO dataset. This version of the dataset was created by @manaporkun. A special thanks to him for making it open source. 
<a href="https://universe.roboflow.com/alpha-tauri/plastic-project">
    <img src="https://app.roboflow.com/images/download-dataset-badge.svg"></img>
</a>

### Performing inference

Inference has always been a headache, ugh! Even with Gradio and Streamlit, it doesn’t get better. Which is why, we resorted to load and make a web application (flask as backend) to perform inference. 

### Shabby Coding Boo bOo! 

I always prefer clear code than shabby coding where authors try to make everything complex and stranded me with only !python <filename> command. Like W!! Which is why, I used Flask as a backend to perform inference while using honey sweet pytorch **(Love!)**

(Jupyter Notebooks are provided for learners to learn) 
(Experts run app.py) :P (CPU is fine, I love hot GPU air)

### Navigating through repository
Quite simple! I have stored all the notebooks, I used both for `training` and `interference`. 
* 'notebooks/hufload_pytorch.ipynb' -> inteference notebook
* `notebooks/yolo5_trash.ipynb` -> training notebook

##### Running Flask
* Open `terminal`
* Navigate to the repository
* Inside the repo run `python app.py`

### Upcoming

- [ ] Labelling TrashNet dataset for Object Detection. (Stanford Version)
- [ ]  Releasing TrashNet weights
- [ ] Finding waste food costs :P 
- [ ] DarkNet (haha! _)

Special thanks to Roboflow for such wonderful free support! Couldn’t make the dataset without you.

#### Acknowledgement
A project developed by me under my team Alpha Tauri. Licenced under Open Source **GPL**. 
<blockquote>
 We believe in developing human friendly Software!
</blockquote>
