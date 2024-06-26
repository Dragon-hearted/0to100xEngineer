# Product Photo-shoot Engine

## Problem Statement

> Use the reference photo and generate the product in the following backgrounds : sand, snow, forest and water

<div class="center">
  <div class="img-sizer" style="width: 100px">

![Reference Image](<images/reference image.png>)

  </div>
</div>


## Method Used

- Inpaint background Extension
- Canny (ControlNet)
- Realism Engine and Realistic Vision Checkpoints

## Results

### For Sand

| Inputs | Sand 1 | Sand 2 |
| ------ | ------ | ------ |
|**Images**|![Sand 1](<images/sand 1.png>)|![Sand 2](<images/sand 2.png>)|
|**Prompt**| professional product photoshoot of perfume bottle in sand with beach elements, studio lighting, warm weather | product shoot in sand with beach elements, warm weather, studio lighting |
|**Parameters**|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 3001968073, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 2, Version: v1.9.4|Steps: 20, Sampler: DPM++ 2M, Schedule type: Karras, CFG scale: 8, Seed: 1659960289, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.91, Masked content: fill, Version: v1.9.4|
|**Negative Prompt**|incomplete figures|incomplete elements|

### For Snow

| Inputs | Snow 1 | Snow 2 | Snow 3 |
| ------ | ------ | ------ | ------ |
|**Images**|![Snow 1](<images/snow 1.png>)|![Snow 2](<images/snow 2.png>)|![Snow 3](<images/snow 3.png>)|
|**Prompt**|professional product photo of perfume bottle in snow, gifting box, studio lighting|professional product photo of perfume bottle in snow, gifting box, studio lighting|professional product poster in snow, gifting box,studio lighting|
|**Parameters**|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 1122959677, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 4, Masked content: fill, Version: v1.9.4|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 1122959680, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 4, Masked content: fill, Version: v1.9.4|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 1014064563, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 4, Masked content: fill, Version: v1.9.4|

### For Water

| Inputs | Water 1 | Water 2 |
| ------ | ------ | ------ |
|**Images**|![water 1](<images/water 1.png>)|![water 2](<images/water 2.png>)|
|**Prompt**|professional product photo of perfume bottle water background and water splashes, gifting box, studio lighting |professional product photo of perfume bottle in water, gifting box, studio lighting |
|**Parameters**|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 2515039110, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 4, Masked content: fill, Version: v1.9.4|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 1452799803, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 4, Masked content: fill, Version: v1.9.4|

### For Forest

<div class="center">
  <div class="img-sizer" style="width: 100px">

![Forest](<images/forest 1.png>)

  </div>
</div>

> Prompt:
>> professional product photoshoot in forest background with wild elements and gift box
>
> Parameters:
>> Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 8, Seed: 1042954205, Size: 985x1266, Model hash: f47e942ad4, Model: realistic_vision_V6.0, Denoising strength: 0.9, Mask blur: 4, Masked content: latent noise, Version: v1.9.4
>
> Negative Prompt:
>> incomplete elements, incomplete blending, no human, different lighting effect

### Miscellaneous

<div class="center">
  <div class="img-sizer" style="width: 100px">

![Miscellaneous](<images/miscellaneous.png>)

  </div>
</div>

> Prompt:
>> professional product photo of perfume bottle in water, gifting box, studio lighting
>
> Parameters:
>> Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 1452799801, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 4, Masked content: fill, Version: v1.9.4
