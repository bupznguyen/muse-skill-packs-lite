# Image Upscaler

## Purpose

Upscale AI-generated keyframes and posters (typically 576×1024 or 768×1024 from Seedream/Gemini) to high resolution for 9:16 vertical drama production. The bundled route runs on plain CPU — no GPU, no account, no API key.

## Tooling

A bundled script runs Real-ESRGAN x4plus (ONNX, via ONNX Runtime) with tiled CPU inference and seamless blending. The model weights (xinntao/Real-ESRGAN, BSD-3-Clause) are downloaded separately.

## Measured performance

On a small CPU host (2 vCPU, 7.7 GB RAM), a 576×1024 keyframe upscales to 2304×4096 in about 9 minutes. Run one upscale at a time.

## Workflow

Generate the keyframe, upscale it before editing or image-to-video, then crop or downscale to the delivery size (e.g. 1080×1920). Artifact repair is out of scope — hand results to an image-realism workflow instead.

## Operating Rules

CPU upscaling is slow, so large batches may be better on a cloud GPU; ncnn-vulkan binaries need a Vulkan GPU and fail on CPU-only hosts; no API key is ever required.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
