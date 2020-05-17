# HereIsWally
Deep learning project that solves Where's Wally puzzles by finding the exact position of Wally in an image

![alt text](https://raw.githubusercontent.com/tadejmagajna/HereIsWally/master/docs/docs.png)

HereIsWally is a Tensorflow project that includes a model for solving Where's Wally puzzles.
It uses Faster RCNN Inception v2 model initially trained on COCO dataset and retrained for finding Wally using transfer learning with Tensorflow Object Detection API.

## Getting ready
1. Install Python 3.7
2. [Install Pipenv](https://github.com/pypa/pipenv#installation)
3. Run `pipenv install` to install the dependencies
4. Run `pipenv shell` to activate the Pipenv environment

## Usage
```
python find_wally_pretty.py images/1.jpg
```
or 
```
python find_wally.py images/1.jpg
```

A window displaying a Wally puzzle outlining Wally should show up.

## Retraining the model

For instructions about how to retrain the model follow the instructions [in this blog post](https://towardsdatascience.com/how-to-find-wally-neural-network-eddbb20b0b90).

## Sources
- [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection)
- [Training Images](https://github.com/vc1492a/Hey-Waldo)

## Related projects

- [Gathering and Analyzing Hardware Performance Data During Deep Network Training](https://github.com/amerus/BenchmarkingTensorflow/)

## Copyright

See [LICENSE](LICENSE) for details.