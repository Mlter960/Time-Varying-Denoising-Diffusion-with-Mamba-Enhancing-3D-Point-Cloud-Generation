## Requirements:

Make sure the following environments are installed.
(Code tested with cuda11)

```
python
pytorch
torchvision
matplotlib
tqdm
open3d
trimesh
scipy
```

Install PyTorchEMD by
```
cd metrics/PyTorchEMD
python setup.py install
cp build/**/emd_cuda.cpython-36m-x86_64-linux-gnu.so .
```


## Training:

```bash
$ python train_generation.py --category car|chair|airplane
```

Please refer to the python file for optimal training parameters.

