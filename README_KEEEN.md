# requirement
pip install kornia==0.7.2 asyncio wget insightface onnxruntime==1.17.3 onnxruntime-gpu==1.17.1 numba rembg -i https://pypi.tuna.tsinghua.edu.cn/simple


blend-modes
segment-anything
trimesh

diffusers==0.27.2
facexlib
ninja
pillow_avif_plugin
ultralytics==8.2.53
yacs
rtree

typer
loguru
typer_config
pydantic==2.8.2


# FLUX

yacs
rtree

mss
spandrel
diffusers==0.30.2

# !!! Exception during processing !!! No operator found for `memory_efficient_attention_forward` with inputs:
pip uninstall xformers

# joycaptiom
peft
Jinja2==3.1.0
bitsandbytes==0.44.1
transformers==4.45.2
accelerate==0.26.0

# LayerStyle
# yolo
supervision
inference-cli>=0.13.0
inference-gpu[yolo-world]>=0.13.0
# evf-sam
hydra-core
torchscale


### Cannot import name 'guidedFilter' from 'cv2.ximgproc'
先卸载所有已安装的opencv，然后按顺序重装如下：
pip uninstall -y opencv-python opencv-python-headless
pip install opencv-python opencv-python-headless opencv-contrib-python-headless -i https://pypi.tuna.tsinghua.edu.cn/simple
pip install opencv-contrib-python -i https://pypi.tuna.tsinghua.edu.cn/simple
apt-get install -y libgl1-mesa-glx

# https://github.com/comfyanonymous/ComfyUI/issues/4434
# flux: module 'torch' has no attribute 'float8_e4m3fn' #4434
pip uninstall torch torchvision torchaudio
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118


# 启动
python main.py --listen '0.0.0.0'


downloading https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth to /project/models/sams/sam_vit_h_4b8939.pth
downloading https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/GroundingDINO_SwinT_OGC.cfg.py to /project/models/grounding-dino/GroundingDINO_SwinT_OGC.cfg.py
downloading https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/groundingdino_swint_ogc.pth to /project/models/grounding-dino/groundingdino_swint_ogc.pth

downloading https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/GroundingDINO_SwinB.cfg.py to /project/models/grounding-dino/GroundingDINO_SwinB.cfg.py
downloading https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/groundingdino_swinb_cogcoor.pth to /project/models/grounding-dino/groundingdino_swinb_cogcoor.pth


# PULID 人脸
Downloading: "https://github.com/xinntao/facexlib/releases/download/v0.1.0/detection_Resnet50_Final.pth" to /opt/conda/lib/python3.10/site-packages/facexlib/weights/detection_Resnet50_Final.pth
Downloading: "https://github.com/xinntao/facexlib/releases/download/v0.2.2/parsing_parsenet.pth" to /opt/conda/lib/python3.10/site-packages/facexlib/weights/parsing_parsenet.pth
Downloading: "https://github.com/xinntao/facexlib/releases/download/v0.2.0/parsing_bisenet.pth" to /opt/conda/lib/python3.10/site-packages/facexlib/weights/parsing_bisenet.pth


# Pulid flux安装
EVA02_CLIP_L_336_psz14_s6B.pt: /root/.cache/huggingface/hub/models--QuanSun--EVA-CLIP/snapshots/11afd202f2ae80869d6cef18b1ec775e79bd8d12/EVA02_CLIP_L_336_psz14_s6B.pt
Downloading: "https://github.com/xinntao/facexlib/releases/download/v0.1.0/detection_Resnet50_Final.pth" to /opt/conda/lib/python3.10/site-packages/facexlib/weights/detection_Resnet50_Final.pth
Downloading: "https://github.com/xinntao/facexlib/releases/download/v0.2.2/parsing_parsenet.pth" to /opt/conda/lib/python3.10/site-packages/facexlib/weights/parsing_parsenet.pth
Downloading: "https://github.com/xinntao/facexlib/releases/download/v0.2.0/parsing_bisenet.pth" to /opt/conda/lib/python3.10/site-packages/facexlib/weights/parsing_bisenet.pth

# ImportError: libGL.so.1: cannot open shared object file: No such file or directory
1. apt-get install libgl1-mesa-glx
2. pip uninstall opencv-python-headless
3. pip install opencv-python-headless