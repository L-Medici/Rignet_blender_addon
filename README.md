# Rignet_blender_addon
Adopting https://github.com/zhan-xu/RigNet neural network we created an addon in blender for an intuitive and easy rigging of their existing template characters 
We strongly advise to use the latest version of blender available in order to use the addons

1)setup of anaconda that emulates our environment on windows 64x
--------
-Install anaconda.

-open anaconda navigator interface/program

-go into environments

-create a new environment with python 3.7

-press the play button next to the created environment, open terminal

-pip install numpy==1.20.2

-pip install scipy==1.7.0

-pip install matplotlib==3.4.2

-pip instal tensorboard==2.5.0

-pip install open3d==0.9.0

-pip install opencv-pyhon==4.5.2.54

-pip install rtree==0.9.7

-pip install trimesh[easy]

-conda install pytorch==1.6.0 torchvision==0.7.0 cudatoolkit=10.1 -c pytorch

-pip install torch-scatter -f https://pytorch-geometric.com/whl/torch-2.0.6.html

-pip install torch-sparse -f https://pytorch-geometric.com/whl/torch-0.6.9.html

-pip install torch-spline-conv -f https://pytorch-geometric.com/whl/torch-1.2.1.html

-pip install torch-cluster -f https://pytorch-geometric.com/whl/torch-1.5.9.html

-pip install torch-geometric==1.7.2

-Download from https://www.lfd.uci.edu/~gohlke/pythonlibs/#rtree the file named "Rtree‑0.9.7‑cp37‑cp37‑win_amd64.whl" then run on the console  pip install Rtree‑0.9.7‑cp38‑cp38‑win_amd64.whl

-If any of the above ends up in an error it is possible to browse the created environment directly in anaconda navigator and install the above mentioned packages



2)scaricare codice da https://github.com/zhan-xu/RigNet ed estrailo in un path a piacere
--------
3)scaricare la cartella https://umass.box.com/s/l7dxfayrubf5qzxcyg7can715xnislwm e incollare la cartella all'interno di rignet main
--------
4)incollare quick_start1.py all'interno di rignet master
--------
5)avviare il terminal di anaconda e startare blender
--------
6)edit preferences install
--------
7)Press "N" to open the addon panel
