1. Install pytorch
CUDA version 11.7
`pip install torch==2.0.1+cu117 torchvision==0.15.2+cu117 --extra-index-url https://download.pytorch.org/whl/cu117`
CUDA version 11.8
`pip install torch==2.0.1+cu118 torchvision==0.15.2+cu118 --extra-index-url https://download.pytorch.org/whl/cu118`

2. Install requirements
`pip install -r requirements`

3. Install our forked viser
```
mkdir extern && cd extern
git clone https://github.com/heheyas/viser 
cd viser
pip install -e viser
cd ..
```

4. Build Gaussian Splatting Renderer and submodules
```
pip install -e gaussiansplatting/submodules/diff-gaussian-rasterization
pip install -e gaussiansplatting/submodules/simple-knn
```