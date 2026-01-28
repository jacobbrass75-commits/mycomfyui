# Arkon ComfyUI Product Compositing

ComfyUI workflows and assets for Arkon product photography compositing.

## Workflows

- `workflows/archon_product_compositing_workflow.json` - Main SDXL-based workflow with Depth + Canny ControlNets
- `workflows/archon_iclight_enhanced_workflow.json` - IC-Light workflow for advanced lighting/shadow matching

## Product Images

Transparent PNG product images are in `products/transparent/`.

## Setup

1. Clone ComfyUI: `git clone https://github.com/Comfy-Org/ComfyUI.git`
2. Create Python 3.12 venv and install requirements
3. Install PyTorch with CUDA: `pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124`
4. Install custom nodes:
   - ComfyUI-Manager
   - comfyui_controlnet_aux
   - ComfyUI_essentials
   - ComfyUI-IC-Light
   - ComfyUI-Impact-Pack
   - was-node-suite-comfyui
   - stability-ComfyUI-nodes

5. Download models:
   - Checkpoints: Juggernaut XL v9, Realistic Vision v6 (VAE)
   - ControlNets: Depth SDXL, Canny SDXL
   - Upscaler: 4x-UltraSharp
   - IC-Light: iclight_sd15_fbc.safetensors

6. Copy workflows to ComfyUI and load in browser
