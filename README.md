# Ansible Role: socat

Setup a `systemd` Service with your custom `socat` command.

It's perfect to bridge traffic from `ipv4` to `ipv6` or do some other crazy network stuff.

## Configuration Variables

You can use several Variables to configure this role.

### required variables

- `socat_service_name` - the name for the `systemd` Service (appended to `socat-`)
- `socat_command` - the parameter line for the `socat` command. (e.g.: `TCP6-LISTEN:443,fork TCP4:10.10.10.10:443`)