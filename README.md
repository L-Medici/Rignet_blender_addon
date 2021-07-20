# Rignet_blender_addon
Adopting https://github.com/zhan-xu/RigNet neural network we created an addon in blender for an intuitive and easy rigging of their existing template characters

We strongly advise to use the latest version of blender available in order to use the addons

1)Setup of Anaconda that emulates our environment on Windows 64x
--------
Install Anaconda

Open anaconda navigator interface

Go into environments

Create a new environment with python 3.7

Press the play button next to the created environment, open terminal

```
pip install numpy==1.20.2

pip install scipy==1.7.0

pip install matplotlib==3.4.2

pip install tensorboard==2.5.0

pip install open3d==0.9.0

pip install opencv-python==4.5.2.54

pip install rtree==0.9.7

pip install trimesh[easy]

conda install pytorch torchvision cudatoolkit=10.1 -c pytorch
```

Minimize the console window, check on Anaconda the version of pytorch and make sure it's 1.7.1 or above after you clicked the button "update index". When we explicit the version within the "pip install" command for some reason it generates errors lately. According to the version installed, simply modify the four following pip installs with your current version "torch-#.#.#+cu101.html":

```
pip install torch-scatter==2.0.7 -f https://pytorch-geometric.com/whl/torch-1.7.1+cu101.html

pip install torch-sparse==0.6.9 -f https://pytorch-geometric.com/whl/torch-1.7.1+cu101.html

pip install torch-spline-conv==1.2.1 -f https://pytorch-geometric.com/whl/torch-1.7.1+cu101.html

pip install torch-cluster==1.5.9 -f https://pytorch-geometric.com/whl/torch-1.7.1+cu101.html

pip install torch-geometric
```

If you are working on Linux you can skip this last step. Download from https://www.lfd.uci.edu/~gohlke/pythonlibs/#rtree the file named "Rtree‑0.9.7‑cp37‑cp37m‑win_amd64.whl" and paste it into C:\Users\<your_pc>. Then run on the console:

```
pip install Rtree‑0.9.7‑cp37‑cp37m‑win_amd64.whl
```

If any of the above ends up in an error it is possible to browse the created environment directly in anaconda navigator and install the above mentioned packages



2)RigNet setup
--------
Download the code of https://github.com/zhan-xu/RigNet and unzip it

Download the folder "checkpoints" from https://umass.box.com/s/l7dxfayrubf5qzxcyg7can715xnislwm and paste it within the folder "RigNet-master"

Download quick_start1.py from our github and paste it inside the folder RigNet-master (there is no need to delete the original quick_start.py within the folder)

To test that everything works, from the anaconda console go into RigNet-master folder and run:
```
python quick_start.py
```
It might take a while, don't panic and wait for the Network to finish working <3

When it finishes, a seagul should appear on a open3d window which gives you a preview of what the network did

3)Blender setup
--------
Once you downloaded the latest version of Blender, open the anaconda environment terminal again

Change folder path with
```
cd C:\Program Files\Blender Foundation\Blender 2.93
```

Run "blender"

Blender should open on its own, from here go to "edit", "preferences", "addons", install

Browse your folder till you find the zipped folder "Addon_rignet.zip" downloaded from our github

Select it. After a short delay it should appear next to a box which turns on the addon


4)Using the addon
--------
Press "N" to open the addon panel

Select the path where "RigNet-Master" is within your computer

Select from the list of objects the one you choose to add inside blender

Run. The process may take a while depending on the complexity of the the object chose for the rigging

After a while the preview of the rigged model will appear on the open3d window. Close this window to allow the code to proceed

Later on the object will appear at the center of the world in Blender, centered in the cursor. If you don't see it it's because the object is very small, just zoom in until you see it

5)Expandind the addon with new objects to rig
--------
In theory, https://github.com/zhan-xu/RigNet explains that it is possible to create new objects for the RigNet to work on. For any consideration related to the topic we advice the reader to check https://github.com/zhan-xu/RigNet because we don't know how to do it yet :p

![Alt Text](https://media.giphy.com/media/SGE99T0iY2GE3svuKv/giphy.gif)
![Alt Text](https://media.giphy.com/media/xQZUNJ1kZ3OGsxLM94/giphy.gif)

Licence
--------
The Rignet is a product of the University of Massachusetts, see the LICENSE README.txt file in this directory or in https://github.com/zhan-xu/RigNet for complete text.
