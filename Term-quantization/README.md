## Requirements

Pytorch 1.0.0 with CUDA

## Training
This repo includes the multi-reseolution training with term quantization for resnet-18 and resnet-50. 

To train the meta multi-resolution model(s) in the paper, run this command:

```train
python main.py -a model_name save_path
```

> 📋model_name can be one of the following three options: resnet-18, resnet-34, resnet-50.

> 📋save_path is the location of the result folder.

> 📋term-budgets can be modified in main.py.

## Code Explanation

> 📋The "model/resnet.py" contains the definitions of the multi-resolution resnet models.

> 📋The "model/quant_layer.py" contains the definitions of term quantization functions.

> 📋The "kernel" folder contains the definitions of the cuda kernels for term quantization.

> 📋The test accuracy will be saved in the 'accuracy' folder.
