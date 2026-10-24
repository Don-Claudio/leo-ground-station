# LEO Ground Station

A mini receive-only ground station for low Earth orbit weather satellites (NOAA APT first, SatNOGS later), built from scratch as an introduction to satellite communication and RF.

**Author:** Claudio Kimani, mechatronic engineering student, Kenya

## Goal

Receive and decode a real satellite pass with hardware I built and software I understand, and document every step, including what went wrong.

The plan is to start with the parts that need no hardware (antenna design, a Python APT decoder working on recorded signals, a link budget), then add the Raspberry Pi and RTL-SDR once they are available, and finally register the station on the SatNOGS network.

## Status

| Part | Status |
|------|--------|
| Foundations reading | In progress |
| Link budget | Not started |
| APT decoder (Python, from recordings) | Not started |
| Antenna model | Not started |
| Antenna build | Not started |
| Station setup (Pi 4B + RTL-SDR) | Waiting on hardware |
| First live pass | Not started |
| SatNOGS registration | Not started |

## Repository layout

```
docs/       Build log, learning notes, link budget write-up, site survey
antenna/    Antenna models, build details, measurements
decoder/    Python APT decoder, tests, notebooks
analysis/   Scripts for calculations such as the link budget
setup/      Provisioning scripts and configs for the Pi / laptop
results/    Decoded images and captured passes
```

Each folder has its own README explaining what belongs there.

## Running things

Nothing to run yet. This section will be filled in as the decoder and scripts are added.

## License

MIT, see [LICENSE](LICENSE).
