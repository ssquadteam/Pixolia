
<div align="center">
  <img src="https://github.com/pixeledge-verify/Pixolia/blob/main/logo.png?" width="32%" height="32%"/>
  <h1>Pixolia</h1>
  <h3>PaperMC Fork Designed for Maximum Performance</h3>

  [![License](https://img.shields.io/github/license/kugge/Kaiiju?style=for-the-badge&logo=github)](LICENSE)
  [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kugge/Kaiiju/build.yml?style=for-the-badge)](https://github.com/pixeledge-verify/Pixolia/actions)
  [![Discord](https://img.shields.io/discord/675813643673141313?color=5865F2&label=discord&style=for-the-badge)](https://discord.gg/8FQBnGSSEq)

</div>

## Features

### Main Changes
- **Toggleable Linear World Format**: Saves about 50% of disk space in OW/Nether and 95% in The End.

### Mentionable Changes
- **Optimize Hopper**: Enable/Disable Paper "Optimize Hopper" patch that break a lot of redstone farms.
- **Fix void trading**: Enable/Disable void trading.

### Configuration

```yaml
verbose: false
region-format:
  debug: false
network:
  send-null-entity-packets: true
  alternate-keepalive: false
gameplay:
  server-mod-name: Pixolia
  shared-random-for-players: true
world-settings:
  default:
    region-format:
      format: ANVIL
      linear:
        compression-level: 1
        crash-on-broken-symlink: true
    gameplay:
      shulker-box-drop-contents-when-destroyed: true
      fix-void-trading: true
      optimize-hoppers: true
      tick-when-empty: true
      break-redstone-on-top-of-trap-doors-early: true
config-version: 1
```

## Building

```bash
./gradlew applyPatches # Apply Pixolia patches
./gradlew createReobfPaperclipJar # Generate Paperclip executable jar
```

## License
Original patches are licensed under GPL-3.0.
