# How to get setup  
(we assume the user is using Windows operating system)  

## Download and set up repository
1. Select the green 'Code' button at the top
2. Select 'Download ZIP'

After download is finished:
1. Unzip the downloaded file
2. Rename the unzipped file (which should be a normal folder now) to 'bbox'
3. **Move the folder to your desktop**

## Download and set up Miniconda
1. Follow the [Miniconda](https://docs.conda.io/en/latest/miniconda.html) link, and download the latest 64-bit Windows version.
2. Install Miniconda.
3. Go to your start menu, and type in 'Anaconda'
4. Select 'Anaconda Prompt (Miniconda3)'
5. Once opened (should be a black command line window), right click the Anaconda Prompt icon on your task bar, and select 'Pin to taskbar'
6. Navigate back to the Prompt window, and click inside it make sure it's active.
7. Type in the following, hit enter (then type in 'y' if asked to do so), and wait for updates to finish. 
~~~~shell
conda update conda
~~~~  
8. **Close the prompt window** (VERY Important) after updates finish. 
9. **Re-open the prompt window.** 
10. Type in the following, hit enter (then type in 'y' if asked to do so), and wait for prompt to finish. 
~~~~shell
conda create --name bbox
~~~~ 
11. Type in the following, and hit enter. You should see the text '(base)' change to '(bbox)'
~~~~shell
conda activate bbox
~~~~  
12. Type in the following, hit enter (then type in 'y' if asked to do so), and wait for prompt to finish. 
~~~~shell
conda install -c conda-forge jupyterlab seaborn opencv
~~~~ 

## Start Jupyter Lab
1. If you have not already done so, type in the following, and hit enter.
~~~~shell
conda activate bbox
~~~~  
2. Type in the following, and hit enter.
~~~~shell
cd Desktop\bbox
~~~~  
3. Type in the following, and hit enter.
~~~~shell
jupyter lab
~~~~  

A window should open up in your default web browser with this URL:  
http://localhost:8888/lab  
You should be able to see the Jupyter Lab GUI.  

On the left hand side of the GUI, double-click the file **draw_bboxes.ipynb**
Follow the instructions.  

## Optional
if you wish to modify the config.py file (in jupyter lab), right click the config.py file, select 'Open With' then select 'Editor'  
After making your modifications use Ctrl + S to save the changes.  
Close the tab.
