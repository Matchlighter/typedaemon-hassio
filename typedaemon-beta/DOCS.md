# TypeDaemon Add-on
## Installation

The installation of this add-on is pretty straightforward and not different in comparison to installing any other Home Assistant add-on.

1. Add the https://github.com/Matchlighter/typedaemon-hassio repository by:
    1. Navigating to Home Assistant Settings > Addons > Add-on Store
    2. Access the kebab menu in the upper right, and select "Repositories"
    3. Paste `https://github.com/Matchlighter/typedaemon-hassio` in the "Add" field, then click "ADD".
2. Reload the page
3. Find the TypeDaemon section and select the TypeDaemon addon
4. Install it

## Configuration

**Note**: _Remember to restart the add-on when the configuration is changed._

Example add-on configuration:

```json
{
  "tailcat": false
}
```

### Option: `tailcat`

Reach TypeDaemon's SSH server (used by `td` and remote development) through a [tailcat](https://github.com/tailscale/tailcat) tunnel, with no open port. Restart the add-on after changing. The tailcat address is written to `typedaemon/.typedaemon/connection_params`; anyone with it can reach SSH (the login key is still required), so keep it private.

### Option: SSH port

Port `7722` (SSH) is disabled by default. Set a host port in the add-on's Network section to reach it directly (then use `TD_SSH_HOST=host:port` with `td`).
