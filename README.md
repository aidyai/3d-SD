
### THE FINETUNED MODEL IS AVALIBLE ON HUGGINGFACE: <a href="https://huggingface.co/aidystark/3Dillustration-stable-diffusion" target="_top">HUGGINGFACE FINETUNED MODEL</a>
---
license: creativeml-openrail-m
tags:
- stable-diffusion
- text-to-image
---
### 3d illustration style: This is the fine-tuned Stable Diffusion model trained on images in my ```attribution.txt``` file.
Use the tokens **_3d illustration style_** in your prompts for the effect.

```python
from diffusers import StableDiffusionPipeline
import torch
model_id = "aidystark/3Dillustration-stable-diffusion "
pipe = StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16)
pipe = pipe.to("cuda")
prompt = "3d illustration style rendering of anthony joshua 3d illustration style"
image = pipe(prompt).images[0]
image.save("./img.png")
```


**Characters rendered with the model:**
<p align="center"><img alt="Output 1" src="/data/3d.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/cyxg.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/ycyxg.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/taylor.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/yxg.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/cugx.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/xtgug.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/xug.png" width="65%"/></p>
<p align="center"><img alt="Output 1" src="/data/cugxt.png" width="65%"/></p>

## License
This model is open access and available to all, with a CreativeML OpenRAIL-M license further specifying rights and usage.
The CreativeML OpenRAIL License specifies: 

1. You can't use the model to deliberately produce nor share illegal or harmful outputs or content 
2. The authors claims no rights on the outputs you generate, you are free to use them and are accountable for their use which must not go against the provisions set in the license
3. You may re-distribute the weights and use the model commercially and/or as a service. If you do, please be aware you have to include the same use restrictions as the ones in the license and share a copy of the CreativeML OpenRAIL-M to all your users (please read the license entirely and carefully)
[Please read the full license here](https://huggingface.co/spaces/CompVis/stable-diffusion-license)

