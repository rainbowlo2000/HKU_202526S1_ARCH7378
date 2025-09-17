# HKU_202526S1_ARCH7378


#### IT IS IMPORTANT THAT YOU HAVE WINDOWS INSTALLED ON YOUR COMPUTER TO MAKE THE MOST OUT OF THE SOFTWARE & PLUGINS EXPOSED IN THIS CLASS! ####

## [Setup Python]

### Clone this Repository

Download [GitHub Desktop] (https://desktop.github.com/)

After installation, clone the class repository by clicking the green button ```<> Code```, and then pressing ```Open with GitHub Desktop```.

Make a note on where the repository is saved in your hard drive!!!

### Install Package Manager

Download and install [Anaconda](https://docs.anaconda.com/free/anaconda/install/windows/).

After installation, open ```Anaconda Prompt``` in Windows or ```Terminal``` on MacOS.

We will begin by creating a new environment:
```bash
conda create -n hku_arch_7378 python=3.9
```

Verify that the environment has been installed properly as follows:

```bash
conda activate hku_arch_7378
```

To open your Python interpreter, simply type:

```bash
python
```

You should see the following:
```
Python 3.8.18 | packaged by XX | (default, XX XX 20XX, XX:XX:XX)
[XX] on XX
Type "help", "copyright", "credits" or "license" for more information.
```

To exit, simply type:

```bash
exit()
```

### Install Python Packages

> [!NOTE]
> VERY IMPORTANT!!! 非常重要！！！

Always make sure you are in the right environment when installing Python packages:

```bash
conda activate hku_arch_7378
```

Please install Jupyter Notebook into your environment:

```bash
conda install jupyter
```

Install Scientific Libraries
* conda install numpy scipy matplotlib

Install Data Visualisation
* conda install matplotlib

Install Machine Learning Libraries
* conda install pandas scikit-learn
* [PyTorch](https://pytorch.org/get-started/locally/)
