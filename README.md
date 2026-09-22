# Sparse Audio Recovery Demo

Listening examples for white-box sparse recovery from VGGish internal
activations. The public listening page contains the original LJ Speech segment,
the Griffin--Lim reference ceiling, and Pool 1--3 reconstructions.

## Configuration

- Input: eight 96x64 VGGish log-mel patches
- Dictionary: orthonormal 8x8 block DCT
- Retained coefficients: 32 of 64 per block
- Optimizer: proximal Adam, 30,000 steps
- Learning rate: 0.03
- L1 weight: 0.001

| Recovery point | Log-mel SNR |
|---|---:|
| Pool 1 | 19.32 dB |
| Pool 2 | 11.83 dB |
| Pool 3 | 7.87 dB |

The WAV files are mono, 16 kHz PCM for browser compatibility.
