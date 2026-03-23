# AnyTone D890UV Codeplug

A community-driven codeplug for the **AnyTone D890UV** radio, pre-configured with channels, zones, and settings for amateur radio use in Greece and beyond.

## What's Included

- **DMR Zones & Talk Groups** -- All(?) Greek DMR repeaters (Ymittos, Kitheronas, Vitsi, and more) with commonly used talk groups
- **Analog Simplex Channels** -- VHF and UHF simplex frequencies
- **Digital Simplex Channels** -- VHF and UHF DMR simplex
- **Marine Channels** -- Full marine band scan list
- **PMR Channels** -- European and US PMR/FRS/GMRS frequencies
- **LPD Channels** -- Low Power Device frequencies
- **APRS** -- Analog and digital APRS configuration
- **Airband Zones** -- Aviation monitoring (El. Venizelos, Makedonia, Iraklio)
- **ISS & SSTV** -- Frequencies for the International Space Station
- **Scan Lists** -- Pre-built scan lists for common use cases
- **Weather Channels** -- Weather monitoring for Athens

## Prerequisites

- **AnyTone D890UV** radio
- **AnyTone CPS** (Customer Programming Software) -- download from the official AnyTone website
- USB programming cable for the D890UV

## How to Use

1. **Download** the codeplug files from this repository (clone or download as ZIP).
2. **Open** the AnyTone CPS on your computer.
3. **Import** the codeplug by opening the `d890uv.LST` file in CPS. This file references all the CSV data files and loads the full configuration.
4. **Edit** the `RadioIDList.CSV` to set your own **DMR ID** and **callsign** before writing to the radio.
5. **Review** channels, zones, and talk groups -- adjust frequencies and repeater settings to match your local area if needed.
6. **Write** the codeplug to your radio using the USB cable.

### Downloading a Specific Version

Each codeplug release is tagged with a version number (e.g., `v1.03`, `v1.04`). The `main` branch always contains the latest version.

**From GitHub:** Go to the [Releases](../../releases) page and download the ZIP for the version you need.

**Using Git:**

```bash
# Clone the repository
git clone <repo-url>
cd <repo-folder>

# List all available versions
git tag

# Switch to a specific version
git checkout v1.03
```

> **Note:** Checking out a tag puts you in "detached HEAD" state -- this is normal for just reading/using the files. If you want to make changes based on an older version, create a branch from it:
> ```bash
> git checkout -b my-changes v1.03
> ```

> **Important:** You must update the Radio ID with your own DMR ID before transmitting on DMR. You can obtain a DMR ID at [radioid.net](https://radioid.net/).

## Contributing

Contributions are welcome! Whether you want to:

- Add new repeaters or talk groups
- Fix frequency data or tone settings
- Add channels for other regions
- Improve documentation
- Share your own zone configurations

Feel free to **open an issue** or **submit a pull request**. Any contribution, big or small, is appreciated.

## Credits

This codeplug was built using [alinakis/anytone-878uvii-plus](https://github.com/alinakis/anytone-878uvii-plus) as a starting point. Thanks to the original author for the groundwork and inspiration.

## License

This project is open source. Feel free to use, modify, and share.

## Disclaimer

Always ensure you are licensed and authorized to transmit on any frequency before doing so. This codeplug is provided as-is with no guarantees. Verify all frequencies and settings comply with your local regulations.

---

73 de SV2TSM
