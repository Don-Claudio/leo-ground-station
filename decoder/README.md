# APT Decoder

A Python decoder that turns a recorded NOAA APT signal into an image, written step by step to understand each stage of the chain.

## Planned stages

1. Load recorded audio
2. Demodulate the 2400 Hz AM subcarrier
3. Detect sync pulses and align lines
4. Assemble the image and read the telemetry wedges
5. Compare against a reference decoder on the same recording

## Folders (created as needed)

- `apt_decoder/`: the Python package
- `tests/`: unit tests, including synthetic APT signals with known content
- `notebooks/`: exploration and plots
- `samples/`: a tiny sample recording only; link to public sources for anything large

## Status

Not started.
