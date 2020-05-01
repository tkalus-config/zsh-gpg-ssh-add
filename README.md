# zsh-gpg-ssh-add

zsh ssh-add wrapper that's compatible with gpg-agent backed by a SmartCard

## Dependencies

- Installed pinentry-tty or pinentry-curses (prefer former)
- Running gpg-agent
  - `gpg-agent` plugin on oh-my-zsh
  - `gpg` plugin on prezto

## Installation

Copy `pinentry-unattended` to `/usr/local/bin` or similar locale in PATH.

Copy gpg-agent.conf to `${HOME}/.gnupg/gpg-agent.conf`, modifying the `pinentry-program` line as appropriate.

## Usage

```
$ ssh-add
Please unlock the card

Number: 0054 01239876
Holder: Example User
PIN:
$
```
