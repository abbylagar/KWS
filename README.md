# Key Word Spotting 
> created by : Abegail Lagar

Tools used:
```
Pytorch Lightning
Wandb
tkinter
PyAudio
torchaudio
```
### Folder Structure
    .
    ├── checkpoints               # Pretrained weights
    ├── outputs                   # recorded voice folder
    ├── samples                   # Raw video
    ├── datasets                  # Dataset folder
    │   └── python          
    │         └── drinks          # Drinks Dataset
    ├── train.py                  # training code
    ├── infer.py                  # run keyword spotting app
    └── README.md
    

### Set-up procedures:
steps before training and testing the model

### 1. Clone the repository:
```
!git clone https://github.com/abbylagar/objectdetection.git
```

### 2. Go to your project directory
```
%cd <project_folder>/objectdetection/KWS
```

### 3. Install the requirements
```
!pip install -r requirements.txt
```



### Testing the model
Datasets and pretrained model during this part.

Sample run in the Drinks_detection.ipynb
```
!python3 test.py
```
Output metrics:


![image](https://user-images.githubusercontent.com/67377766/166150634-35123488-34a6-481f-909a-76b7d593b449.png)

### Training the model
Sample run in the train.ipynb .  
If wandb visualization prompts ,
enter 2 (Use an existing W&B account , project name:  KWS)
enter 3 (No visualization)
```
!python3 train.py
```
Max accuracy after 35 epochs 

![image](https://user-images.githubusercontent.com/67377766/166149359-fd1f2af6-2444-4f56-ac29-5583a53ee5c3.png)


### Sample Video 
Sample video of keyword spotting GUI in outputs folder filename: sample.mp4

```
!python3 infer.py 
```


![image](https://user-images.githubusercontent.com/67377766/166147798-7cacd8d7-eb02-45e4-834d-11a782d92170.png)
