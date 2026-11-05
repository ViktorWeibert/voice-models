# voice-models

Speech recognition models for the Android app *Voice Pilot*. The models are not stored in git, only as release assets.

| Release | Asset | Content |
|---|---|---|
| `parakeet-v3-int8pc-1` | `voice-parakeet-tdt-0.6b-v3-int8pc.tar.bz2` (+ `.sha256`) | NVIDIA Parakeet TDT 0.6B v3 for sherpa-onnx, encoder re-quantized (int8 per channel, MatMul only) |

The archive holds one folder with `encoder.int8.onnx`, `decoder.int8.onnx`, `joiner.int8.onnx`, `tokens.txt`, a `LICENSE`
and a `README.md` (origin, quantization, measurements, SHA-256 of every file).

## Licence and credit

The model is *parakeet-tdt-0.6b-v3* by NVIDIA, licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3).
ONNX conversion, decoder, joiner and tokens: [k2-fsa/sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx).
The encoder was re-quantized by Viktor Weibert (2026), which is a change to the original. The packages are licensed under
CC BY 4.0 as well. NVIDIA does not endorse them.
