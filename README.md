## Requirements:

Make sure the following environments are installed.
(Code tested with cuda11.3)

```
pip install ninja

pip install matplotlib

pip install tqdm

pip install open3d

pip install trimesh

pip install scipy

pip install timm

pip install seaborn

pip install causal-conv1d==1.1.1

pip install mamba-ssm==1.1.1
```

Install PyTorchEMD by
```
cd metrics/PyTorchEMD
python setup.py install
cp build/**/emd_cuda.cpython-36m-x86_64-linux-gnu.so .
```

Datase
```
project_root/
├── data/
│   └── ShapeNetCore.v2.PC15k/
│       ├── airplane/
│       │   ├── 1234abcd.ply
│       │   └── ...
│       ├── chair/
│       │   ├── 5678efgh.ply
│       │   └── ...
│       └── ...
├── scripts/
├── models/
└── ...

```

## Training:

```bash
$ python train_generation.py --category car|chair|airplane
```

Please refer to the python file for optimal training parameters.

