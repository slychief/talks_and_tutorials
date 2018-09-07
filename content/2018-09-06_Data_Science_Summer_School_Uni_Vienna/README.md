# Deep Learning for Music Classification using Keras

(c) 2018 by

**Alexander Schindler**, AIT Austrian Institute of Technology<br>
Website: http://ifs.tuwien.ac.at/~schindler<br>
Twitter: https://twitter.com/Slychief

also visit: https://www.meetup.com/Vienna-Deep-Learning-Meetup

# Abstract

This is an introduction to Music Information Retrieval (MIR) and audio anlysis in general. The first part of the tutorial - an introduction to MIR - will be presented using the provided slide-deck. The second part introduces to basics of audio processing in Python. In Part 3 deep learning approaches to music classification tasks are presented.

# Tutorial Outline

**Part 1 - Music Information Retrieval (MIR)** ([Slides](Part1_Music_Information_Retrieval.pdf))

  * What is Music Information Retrieval?
  * Audio/Music Feature Extraction
  * Deep Learning for Audio
  * Research in Audio Analysis and MIR

**Part 2 - Audio Processing Basics** ([Jupyter Notebook](Part2_Audio_Basics.ipynb))

  * Audio Processing in Python
  * Processing audio
  * Extracting features

**Part 3 - Instrumental, Genre and Mood Analysis** ([Jupyter Notebook](Part3_Instrumental_Genre_Mood_detection.ipynb))

  * Instrumental vs. Vocal Detection
  * Genre Recognition
  * Mood Detection



# Tutorial Requirements

For the code tutorials, we use iPython / Jupyter notebook, which allows to program and execute Python code interactively in the browser.

### Viewing Only

If you do not want to install anything, you can simply view the tutorials' content in your browser, by clicking on the tutorial's filenames listed above in the GIT file listing.

The tutorials will open in your browser for viewing.

### Interactive Coding

If you want to follow the tutorials by actually executing the code on your computer, please [install first the pre-requisites](#installation-of-pre-requisites) as described below.

After that, to run the tutorials go into the `2018-09-06_Data_Science_Summer_School_Uni_Vienna` folder and start from the command line:

`jupyter notebook`


# Installation of Pre-requisites

## Install Python 3.x

Note: On most Mac and Linux systems Python is already pre-installed. Check with `python --version` on the command line whether you have Python 3.x installed.

Otherwise install Python 3.5 from https://www.python.org/downloads/release/python-350/

## Install Python libraries:

### Mac, Linux or Windows

(on Windows leave out `sudo`)

Important note: If you have Python 2.x and 3.x installed in parallel, replace `pip` by `pip3` in the following commands:

```
sudo pip install --upgrade jupyter
```

Try if you can open 
```
jupyter notebook
```
on the command line. 



Install the remaining Python libraries needed:

Either by:

```
sudo pip install Keras>=2.1.1 tensorflow scikit-learn>=0.18 pandas librosa spotipy matplotlib
```



### Optional for GPU computation

If you want to train your neural networks on your GPU (which is faster, but not necessarily needed for this tutorial),
you have to install the specific GPU version of Tensorflow:

```
sudo pip install tensorflow-gpu
```

and also install the following:

* [NVidia drivers](http://www.nvidia.com/Download/index.aspx?lang=en-us)
* [CUDA](https://developer.nvidia.com/cuda-downloads)
* [cuDNN](https://developer.nvidia.com/cudnn) (requires registration with Nvidia)


## Install Audio Decoder

In order to decode MP3 files (used in the MagnaTagAtune data set) you will need to install FFMpeg on your system.

* Linux: `sudo apt-get install ffmpeg`
* Mac: download FFMPeg for Mac: http://ffmpegmac.net and make sure ffmpeg is on PATH
* Windows: download https://github.com/tuwien-musicir/rp_extract/blob/master/bin/external/win/ffmpeg.exe and make sure it is on the PATH


## Download Prepared Datasets

Please download the following data sets for this tutorial:

**GTZAN Music Speech Classification**

https://owncloud.tuwien.ac.at/index.php/s/JiBXUPZK9LImTHB (145MB)

**MagnaTagAtune**

https://owncloud.tuwien.ac.at/index.php/s/hivOGXKoUQtacbo (332MB)

These are prepared versions from the original datasets described below.


# Credits

The data sets we use in the tutorials are from the following sources:

* GTZAN Music Speech: http://marsyasweb.appspot.com/download/data_sets/
* MagnaTagAtune: http://mirg.city.ac.uk/codeapps/the-magnatagatune-dataset

(don't download them from there but use the prepared datasets from the two owncloud links above)
