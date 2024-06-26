# Product Photo-shoot Engine

## Problem Statement

> Use the reference photo and generate the product in the following backgrounds : sand, snow, forest and water
>> ![Reference Image](<images/reference image.png>)

## Method Used

- Inpaint background Extension
- Canny (ControlNet)
- Realism Engine and Realistic Vision Checkpoints

## Results

### For Sand

| Inputs | Sand 1 | Sand 2 |
| ------ | ------ | ------ |
|        |![Sand 1](<images/sand 1.png>)|![Sand 2](<images/sand 2.png>)|
|**Prompt** | professional product photoshoot of perfume bottle in sand with beach elements, studio lighting, warm weather | product shoot in sand with beach elements, warm weather, studio lighting |
|**Parameters**|Steps: 20, Sampler: Euler a, Schedule type: Automatic, CFG scale: 7, Seed: 3001968073, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.75, Mask blur: 2, Version: v1.9.4|Steps: 20, Sampler: DPM++ 2M, Schedule type: Karras, CFG scale: 8, Seed: 1659960289, Size: 985x1266, Model hash: b513c6287d, Model: realism_engine, Denoising strength: 0.91, Masked content: fill, Version: v1.9.4|
|**Negative Prompt**|incomplete figures|incomplete elements|

### For 