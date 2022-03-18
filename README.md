# HereIsWally
Deep learning project that solves Where's Wally puzzles by finding the exact position of Wally in an image

![alt text](https://raw.githubusercontent.com/tadejmagajna/HereIsWally/master/docs/docs.png)

HereIsWally is a Tensorflow project that includes a model for solving Where's Wally puzzles.
It uses Faster RCNN Inception v2 model initially trained on COCO dataset and retrained for finding Wally using transfer learning with Tensorflow Object Detection API.

## What is needed to use this script
Python 3.7+ (python 3.8 is advised)

### Libraries
Mathplotlib 
```
pip3 install matplotlib
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


Pipenv (i think #TODO check if is needed)
```
pip3 install pipenv
```


The requirement.txt file is made on a UNIX system with M1 (ARM processor) so may have some incompatibility on windows system/not-ARM cpu
```
pip3 install -r requirements.txt
```


## Usage
```
python find_wally_pretty.py images/1.jpg. #this method is deprecated as tensorflow 2.x released please use the other method to execute the script
```
or 
```
python find_wally.py images/1.jpg
```

A window displaying a Wally puzzle outlining Wally should show up.

## Retraining the model

For instructions about how to retrain the model follow the instructions [in this blog post](https://towardsdatascience.com/how-to-find-wally-neural-network-eddbb20b0b90).

Some files are missing so i think is not instantly possible.

## Sources
- [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection)
- [Training Images](https://github.com/vc1492a/Hey-Waldo)

## Related projects

- [Gathering and Analyzing Hardware Performance Data During Deep Network Training](https://github.com/amerus/BenchmarkingTensorflow/)
- [HereIsWally by xtadejmagajna](https://github.com/tadejmagajna/HereIsWally/)
