### Installation

1, clone this repository
```bash
git clone https://github.com/CIBRalgosw/cellpose.git -b add_tensorboard
```
2, installation
```bash
cd your_cloned_cellpose_dir_where_setup.py_in_it
python setup.py
```

### Usage

use tensorboard:
```bash
python -m cellpose --train --tensorboard True ...
```
or not:
```bash
python -m cellpose --train --tensorboard False ...
```
default: True

when you use human-in-the-loop training, you can not set this param's value, the default value is True, so it will save tensorboard's log automatically.

### Launch tensorboard session

use this command to launch tensorboard:
```bash
cd your_traindata_dir/log
tensorboard --logdir ./
```
then open your browser, open this url:
```
http://localhost:6006/
```