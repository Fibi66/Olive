# CLIP VIT Optimization with PTQ on Qualcomm NPU using QNN EP
This workflow performs CLIP VIT quantization on Qualcomm NPU with ONNX Runtime PTQ. It performs the pipeline:
- *PyTorch Model -> Onnx Model -> Quantized Onnx Model*

It requires x86 python environment on a Windows ARM machine with `onnxruntime-qnn` installed.

**NOTE:** The model quantization part of the workflow can also be done on a Linux/Windows machine with a different onnxruntime package installed. Remove the `"evaluators"` and `"evaluator"` sections from the configuration file to skip the evaluation step.
