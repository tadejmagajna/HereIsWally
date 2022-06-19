# HereIsWally
Deep learning project that solves Where's Wally puzzles by finding the exact position of Wally in an image

![alt text](https://raw.githubusercontent.com/tadejmagajna/HereIsWally/master/docs/docs.png)

HereIsWally is a Tensorflow project that includes a model for solving Where's Wally puzzles.
It uses Faster RCNN Inception v2 model initially trained on COCO dataset and retrained for finding Wally using transfer learning with Tensorflow Object Detection API.

## What is needed to use this script
Python 3.8+ (python 3.8 is advised)

### Libraries

Use this command to install the libraries: (tensorflow is not present cause in Apple ARM chips is not yet available
```
pip3 install -r requirements.txt
```


TensorFlow for Chip Intel/AMD #TODO to check if is ok
```
pip3 install tensorflow
```
if it doesn't work use this instead:
```
pip3 install tf-nightly
```


TensorFlow for Chip Apple Silicon M1
I advise to use this package to install solely to make the environment as smooth as possible to use
```
https://drive.google.com/drive/folders/1oSipZLnoeQB0Awz8U68KYeCPsULy_dQ7

```
```
pip3 install ~/Downloads/tensorflow-2.4.1-py3-none-any.whl <or the path where the package downloaded is located>
```


## Usage
```
python find_wally.py images/1.jpg
```

A window displaying a Wally puzzle outlining Wally should show up.

## Retraining the model

For instructions about how to retrain the model follow the instructions [in this blog post](https://towardsdatascience.com/how-to-find-wally-neural-network-eddbb20b0b90).

Some files are missing in this repo so is not instantly possible to retrain the model.

## Sources
- [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection)
- [Training Images](https://github.com/vc1492a/Hey-Waldo)

## Related projects

- [Gathering and Analyzing Hardware Performance Data During Deep Network Training](https://github.com/amerus/BenchmarkingTensorflow/)
- [HereIsWally by xtadejmagajna](https://github.com/tadejmagajna/HereIsWally/)
