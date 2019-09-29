# DEM co-registration tutorial

## 1. Cloning the repository

To get started with the exercises, you'll need to create a `conda` environment containing the packages needed to run the co-registration functions in `python`, and __clone__ this repository to either your course folder on __lagringshotell__, or your M: drive, or your own personal computer. You can do this in one of two ways:

1. Above this message, click the green "clone or download" button, and select "download ZIP" at the bottom of the menu. Once it's downloaded, unzip the file and move on to the next step.
2. __On the lab computers__ Open __Git Bash__ (from the __Start__ menu), then navigate to your folder for the course. Create a new folder called "python\_labs" (`mkdir -p python_labs`), and navigate to that folder (`cd python_labs`). Now, execute the following command: `git clone https://github.com/iamdonovan/dem-coregistration.git`. You should see some messages about downloading/unpacking files, and the repository should be set up.
3. __On a computer where you have administrative access__: If you have already installed __git__ on your laptop, you can use it directly. Otherwise, install __git__, then clone the repository into a given folder with the command `git clone https://github.com/iamdonovan/dem-coregistration.git`. More information about installing and using __git__ can be found [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

## 2. Creating the environment

Once you have the repository, you can create the `conda` environment using the __environment.yml__ file provided. You can do this in one of the following ways, depending on which computer you're running this exercise on:

### 2.1 On one of the lab computers

On your M: drive, create a folder called ".conda" and a folder in ".conda" called "envs", if it does not already exist. Next, open up __Anaconda Prompt__, and type the following command:

```
C:\> conda create --prefix M:\.conda\envs\geo4520 -f path\to\repository\environment.yml
```

making sure to replace path\to\repository with the actual path to the git repostory you cloned in Step 1.

This will probably take some time (so feel free to catch up on Facebook or whatever kids do nowadays), but fortunately you only have to do this once (though you will have to do this again if you want to work on your personal computer). In the future, when you want to open the labs on a computer on the University network, you can just type `activate M:\.conda\envs\geo4520` at the __Anaconda command prompt__, then navigate to the folder where you have your labs and open jupyter-notebook, without having to re-install the conda environment each time.


### 2.2 On a Windows computer where you have administrative access
If you haven't already, install [Anaconda](https://www.anaconda.com/distribution/). Open up __Anaconda Prompt__, then type the following command:

```
C:\> conda create --prefix geo4520 -f path\to\repository\environment.yml
```

making sure to replace path\to\repository\ with the actual path to the git repository you cloned in Step 1.

Once you have installed a conda environment, you can type `activate geo4520` at the __Anaconda Prompt__, navigate to the folder where you have cloned the git repository, and type `jupyter-notebook.exe` to launch jupter-notebook.

### 2.3 On a Linux computer where you have administrative access
If you haven't already, install [Anaconda](https://www.anaconda.com/distribution/). From the command line, type the following command:

```
conda create --prefix geo4520 -f path/to/repository/environment.yml
```

making sure to replace path/to/repository/ with the actual path to the git repository you cloned in Step 1.

## 3. Launching the tutorial

From the command line (__Anaconda Prompt__ on Windows), activate your conda environment if you haven't already (`activate geo4520` on Windows/`conda activate geo4520` on Linux). Then, navigate to the folder where you have cloned the git repository in Step 1 and launch jupyter-notebook (`jupyter-notebook.exe` on Windows, `jupyter-notebook` on Linux/Mac).

