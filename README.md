# Iptables Tester

Docker compose based iptables test setup.

## Requirements

* docker-compose
* tmux

## Usage

```no-highlight
./iptables-tester
```

This will open a tmux window with 4 panes:

* Pane 0: Output of docker compose
* Pane 1: Shell on Firewall
* Pane 2: Shell on Firewall
* Pane 3: Shell on 'external' box

This setup allows you to test rules by running a netcat listener on the
firewall, poking it from external and adjusted the rules to see the effects.
