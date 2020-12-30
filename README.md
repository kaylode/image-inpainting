# Image Inpainting

## Pipeline:
- Data preparation:
  - Download CelebA dataset then crop the image but keeps while keeping ratio with [here](https://github.com/LynnHo/HD-CelebA-Cropper)
  - Create synthesis facemask segmentation dataset with [here](https://github.com/aqeelanwar/MaskTheFace)
 
- Edit configs on both ***segm.yaml*** and ***facemask.yaml***
- Train segmentation model
- Train impainting model

## Train segmentation

```
python train.py segm
```

## Train impainting

```
python train.py facemask
```

## References:
- Idea from https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9019697
- https://github.com/LynnHo/HD-CelebA-Cropper
- https://github.com/aqeelanwar/MaskTheFace
