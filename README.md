# ComfyUI_PBR_Maker
Use comfyUI make PBR materials..

Updated to output files to Comfyui outputs folder with material type and random prefix in name.
Also updated to find model in ComfyUI's models/diffusers/MatForger folder.
Still need to download models from https://modelscope.cn/models/smthem/MatForger/files .
I'm a beginner coder,and just wanted to make it work like I think it was intended to.
You can just copy my updated MatForger_node.py to your folder if you already have it installed.
----

1.Installation  (original install)
-----
  In the ./ComfyUI /custom_node directory, run the following:   
```

git clone https://github.com/smthemex/ComfyUI_PBR_Maker
```
2.checkpoints 
----
Use https://modelscope.cn/models/smthem/MatForger/files instead.

Old huggingface site no longer working:
download [gvecchio/MatForger](https://huggingface.co/gvecchio/MatForger) 

```
Best to put it in models/diffusers/MatForger now,instad of anypath/MatForger.
Keeps things a bit more organized.

├── anypath/MatForger
|     ├── prompt_encoder
|           ├── config.json
|           ├── diffusion_pytorch_model.safetensors
|           ├── encoder.py
|     ├── scheduler
|           ├── scheduler_config.json
|     ├──unet
|           ├── config.json
|           ├── diffusion_pytorch_model.safetensors
|     ├──vae
|           ├── config.json
|           ├── diffusion_pytorch_model.safetensors
|     ├──model_index.json
|     ├──pipeline.py
```

3.Example:
----
Right click and swap Save Image to Preview Image,so there's not 2 sets of textures in output folder.

![](https://github.com/smthemex/ComfyUI_PBR_Maker/blob/main/example.png)

4.Citation
--
using author another project ...
 ``` 
@article{vecchio2024stablematerials,
  title={StableMaterials: Enhancing Diversity in Material Generation via Semi-Supervised Learning},
  author={Vecchio, Giuseppe},
  journal={arXiv preprint arXiv:2406.09293},
  year={2024}
}

```
