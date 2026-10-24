# Build Log

A dated record of what I did, what I expected, what happened, and what I learned. Failures belong here too.

## 2026-10-24: Project start

**Situation:** I temporarily have no access to my Raspberry Pi and have not bought the RTL-SDR dongle yet, so I am starting with the parts that need no hardware.

**Plan:**
1. Read the foundations (signal chain, modulation, antennas) before building.
2. Write a link budget to see whether a 137 MHz LEO pass is strong enough to receive.
3. Write a Python APT decoder that works on recorded audio.
4. Model, then build, a circularly polarized antenna (QFH or turnstile).
5. Set up the Pi and RTL-SDR when available.

**Understanding so far (to be corrected as I learn):**
- NOAA APT sends an image as a stream of lines. Pixel brightness is encoded as the amplitude of a 2400 Hz audio tone, which then frequency-modulates a carrier near 137 MHz.
- Decoding reverses that: FM demodulation, then AM demodulation, then arranging the values into lines.

**Open questions:**
- How does the receiver know where each line starts?
- Roughly how many lines does one pass produce, and what shape does that make the image?

**Next:** finish the foundations reading and answer the open questions above.
