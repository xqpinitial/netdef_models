# netdef_models
Repository for different network models related to flow/disparity from the following papers: 

**NOTE: We only provide deployment code for these networks. We do not publish any training code and also do not off support about questions for training networks.**

* **Occlusions, Motion and Depth Boundaries with a Generic Network for Disparity, Optical Flow or Scene Flow**  
(E. Ilg and T. Saikia and M. Keuper and T. Brox published at ECCV 2018)  [[paper]](http://lmb.informatik.uni-freiburg.de/Publications/2018/ISKB18) [[video]](https://www.youtube.com/watch?v=SwOdSaBRysI)


## Setup
* Install [tensorflow (1.4)](https://www.tensorflow.org/install/) (pip3 install tensorflow-gpu==1.4)
* Compile and install [lmbspecialops](https://github.com/lmb-freiburg/lmbspecialops/tree/eccv18). Please use the branch `eccv18` instead of `master`
* Install [netdef_slim](https://github.com/lmb-freiburg/netdef_slim)
* Clone this repository

## Running networks

* Change your directory to the network directory (Eg: FlowNet3)
* Run download_snapshots.sh. This takes a while to download all snapshots
* Now you should be ready to run the networks. Change your directory to a network type (Eg: css).
  Use the following command to test the network on an image pair:
  `python3 controller.py image0_path image1_path out_dir`

## License

netdef_models is under the [GNU General Public License v3.0](LICENSE.txt)
