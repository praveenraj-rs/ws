# Linux Workspace Automation

This project contains a collection of Linux aliases and automation scripts to enhance productivity by streamlining common tasks in a development environment.

## Features

- Custom aliases for frequently used commands
- Automated environment setup for development
- Quick navigation shortcuts
- System monitoring and management utilities
- Git workflow optimizations

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/praveenraj-rs/ws.git
   cd ws
   ```
2. Run `init`
   ```sh
   ./init
   ```
3. Apply the changes:
   ```sh
   source ~/.bashrc
   ```

## Usage

Here are some useful aliases included:

```sh
# For python virtual env activation and deactivation
alias ws-venv="source ~/venv/bin/activate"
alias ws-denv="deactivate"

# Networking
alias ws-ipShow="hostname -I | awk '{print \$1}'"
alias ws-goLive='python3 -m http.server $1'
alias ws-portCheck='nmap localhost'
```

## Customization

You can modify or add new aliases by editing the `aliases.sh` file:

```sh
nano aliases.sh
```

Then re-source your shell configuration:

```sh
source ~/.bashrc  # or source ~/.zshrc
```

## Contributions

Feel free to fork this repository and submit pull requests with improvements!
