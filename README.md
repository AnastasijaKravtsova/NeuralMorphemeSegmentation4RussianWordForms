![Python 3.6](https://img.shields.io/badge/python-3.6-green.svg)
# Morpheme segmentation for Russian word forms via convolutional neural networks

#### Create and activate a virtual environment for python 3
```bash
python3 -m venv venv
. venv/bin/activate
```

#### Install requirements in your virtual environment
```bash
pip install -r requirements.txt
```

#### Train a model
```bash
python neural_morph_segm.py config/train_config.json
```

#### Test a trained model on a test set
```bash
python neural_morph_segm.py config/test_config.json
```

#### Repository structure

* [сonfig](config): configuration files
* [data](data): train and test sets (morpheme segmentations for word forms of Tikhonov's morphological dictionary).
* [models](models): trained models
* [neural_morph_segm.py](neural_morph_segm.py): main file with model code
* [read.py](read.py): input data reader
