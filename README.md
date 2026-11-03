# Key Holder

A client-side Fabric mod for Minecraft **26.3** (also available for 26.2) that lets you pick a key and holds it down for you, until you toggle it off.

[![GitHub Release](https://img.shields.io/github/v/release/vihaanvp/key-holder-mod)](https://github.com/vihaanvp/key-holder-mod/releases)
[![GitHub License](https://img.shields.io/github/license/vihaanvp/key-holder-mod)](LICENSE)
[![Minecraft Version](https://img.shields.io/badge/Minecraft-26.3-blue)](https://www.minecraft.net/)

## Download

| Minecraft Version | Download |
|-------------------|----------|
| **26.3** (Latest) | [key-holder-fabric-26.3-1.0.1.jar](https://github.com/vihaanvp/key-holder-mod/releases/download/v1.0.1/key-holder-fabric-26.3-1.0.1.jar) |
| 26.2 (Legacy) | [key-holder-fabric-26.2-1.0.1.jar](https://github.com/vihaanvp/key-holder-mod/releases/download/v1.0.1/key-holder-fabric-26.2-1.0.1.jar) |

## Usage

- `/keyholder set <key>` — pick the key to hold (e.g. `w`, `space`, `key.mouse.left`)
- `/keyholder on` / `off` / `toggle` / `status`
- Bind **Toggle Key Hold** in Controls for a one-press toggle (unbound by default)
- Or use the Mod Menu config screen to click-select the held key and flip it on/off

## Requirements

### For Minecraft 26.3 (Current)
- Minecraft 26.3
- [Fabric Loader](https://fabricmc.net/) `>=0.19.5`
- [Fabric API](https://modrinth.com/mod/fabric-api) `0.161.0+26.3`
- Optional: [Mod Menu](https://modrinth.com/mod/modmenu) `21.0.0` + [Cloth Config](https://modrinth.com/mod/cloth-config) `26.3.159` for the GUI screen

### For Minecraft 26.2 (Legacy)
- Minecraft 26.2
- [Fabric Loader](https://fabricmc.net/) `>=0.18.4`
- [Fabric API](https://modrinth.com/mod/fabric-api) `0.154.0+26.2`
- Optional: [Mod Menu](https://modrinth.com/mod/modmenu) `20.0.0-beta.4` + [Cloth Config](https://modrinth.com/mod/cloth-config) `26.2.155` for the GUI screen

## Building

Requires JDK 25:

```bash
# Linux/macOS
JAVA_HOME="<path to JDK 25>" ./gradlew build

# Windows
set JAVA_HOME=<path to JDK 25>
gradlew.bat build
```

The jars are output to:
- `fabric-26.2/build/libs/key-holder-fabric-26.2-1.0.1.jar`
- `fabric-26.3/build/libs/key-holder-fabric-26.3-1.0.1.jar`

## Configuration

Config file location: `config/keyholder.json`

```json
{
  "heldKey": "key.keyboard.w",
  "enabled": false
}
```

- `heldKey`: The translation key of the key to hold (e.g., `key.keyboard.w`, `key.mouse.left`)
- `enabled`: Whether the key hold is active

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for detailed version history.

## License

MIT License - see [LICENSE](LICENSE) for details.

## Author

**the-real-ltcg** - [GitHub](https://github.com/vihaanvp)
