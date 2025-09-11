# HKU_202425S1_ARCH7378


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


## Setup Rhino & Grasshopper Packages

### General

There are three methods to install Grasshopper plugins.   We will use all three at various points.  So it is helpful to go over their process:

1. By dedicated installers.  Usually, they have extensions 'exe' or 'msi'.  Simply step through the installation process.

2. If the provided file has extension 'gha', copy and paste them to Grasshopper's component folders.  You can find them via ```File > Special Folders > Components Folder``` under Grasshopper.

3. Occasionally, a 'gh' file is provided.  In these cases, just open them directly in Grasshopper and it will trigger an installation process.

For case 1 and 2, make sure you close and restart Rhino and Grasshopper after installation.  Otherwise, your plug-ins will not be available.

### Karamba


0. Install Karamba3D, download from here:
https://karamba3d.com/get-started/


> [!NOTE]
> The files ```Karamba3D_LicensePlugin_Zoo6.dll``` and ```Karamba3DGetLicense``` are contained inside this repository at ```hku_arch_7378_DESN3002_ARCH3738/Grasshopper/Karamba3D/License```.

1. Copy ```Karamba3D_LicensePlugin_Zoo6.dll``` to RHINO_INSTALL_PATH\Plug-ins.
   (Replace the placeholder RHINO_INSTALL_PATH accordingly)

2. Start Rhino as Administrator. (Right click program icon > ```More``` > ```Run as Administrator``` )

3. Load Grasshopper by inputting ```grasshopper``` to the ```Command Prompt``` of Rhino.

4. Add the component ```License (Karamba3D)``` to the Grasshopper canvas.
  (To find the component, double click empty space on the canvas anywhere.  This brings up a search prompt (i.e. 'Enter a search keyword...') where you can then type ```License (Karamba3D)``` to bring up the component.)

6. Right click the component ```License (Karamba3D)``` and then select ```Load license file```.  Next, locate and select the file ```licensePRO.lic```.

7. In Rhino's ```Command Prompt```, type ```Karamba3DGetLicense``` and then key in the Zoo license server: ```apps.ad.arch.hku.hk```.  If the license is recognised properly, you will see the following output from the prompt:


```
---
Zoo Server license initialized
---
 Licenser: Clemens Preisinger
 Edition: Educational
 User: FacultyofArchitecture-TheUniversityofHongKong
 End of Support Period: 2022-Nov-19
```

8. Now, restart Rhino (as normal). THIS IS IMPORTANT: Make sure you initialise your license with ```Karamba3DGetLicense``` via the ```Command Prompt``` each time BEFORE you start Grasshopper.
