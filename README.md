# DLH

In order to run the main report, after cloning this repo, run everything from the DL4H_Team_159.ipynb. It should work out of the box. Make sure to run the '!pip install' in the file. If you are having any additional trouble, run the setup:

## Setup (Optional)
In order to run the main report, after cloning this repo, run everything from the DL4H_Team_159.ipynb. 

Step 1: Change the current working directory to the location where you want to install/clone this repo.

Step 2: Clone the repository using git command

```git clone https://github.com/davegii/DLH```

Step 3: Create virtual environment using Anaconda3 (Read Anaconda3 install guide) and activate the virtual environment

```conda create --name deep_env python=3.6```

```conda activate deep_env```

Step 4: Install required packages, then install tensorflow.

```pip install --upgrade pip && pip install numpy==1.16.2 && pip install pandas==0.24.2 && pip install scipy==1.2.1 && pip install scikit-learn==0.20.3 && pip install matplotlib==3.0.3 && pip install psutil==5.6.1 && pip install keras==2.2.4```

If your machine is not equipped with GPU, install tensorflow CPU version. (In my case I just installed CPU version because I was not able to install the previous command)

```pip install tensorflow==1.13.1```

If it is equipped with GPU, then install tensorflow GPU version

```pip install tensorflow-gpu==1.13.1```

Step 5: Run the ipynb file, but setting the environment as the deep_env environment you created above.

## Ablations:
In order to run the ablations, follow the instructions of cloning DeepMicro: https://github.com/minoh0201/DeepMicro/tree/master  (Most of it is already done)

After which, then swap out their DM.py file with the one in this repository. In the anaconda navigator's CMD.exe, Run the code based on their instructions, for example: 

```python DM.py -d marker_WT2D --ae -dm 256```
