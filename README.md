# JARVIS AI Desktop Assistant

A Python-powered desktop AI assistant with a PyQt6 interface, modular actions, and a floating mini-assistant mode.

## Features

- **PyQt6 desktop interface** for interacting with the assistant.
- **Floating mini mode** — switch to a compact, frameless, always-on-top companion window.
- **Quick return to the main window** using the **OPEN HUD** control.
- **Keyboard shortcut:** press `Ctrl+M` to toggle mini mode.
- **Modular actions and tools** organized into the `actions/`, `core/`, and `plugins/` folders.
- **Setup documentation** in `SETUP_GUIDE.md`.

## Requirements

- Windows desktop (the included `run.bat` is intended for Windows)
- Python 3.10 or a compatible version supported by the project's dependencies
- Internet access for features that use external services
- API credentials for any enabled AI or online integrations that require them

## Quick start

1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Create and activate a virtual environment:

   ```bat
   python -m venv .venv
   .venv\Scripts\activate
   ```

4. Install dependencies:

   ```bat
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```

5. Review `config/api_keys.json.example` and follow the setup guide to configure the services you want to use.
6. Start the application using the documented entry point or `run.bat`.

See [SETUP_GUIDE.md](SETUP_GUIDE.md) for more detailed setup and troubleshooting notes.

## Mini-assistant mode

- Click **MINI** in the main window header, or press `Ctrl+M`.
- The compact window stays above other windows and can be dragged around the desktop.
- Click **OPEN HUD** to return to the main assistant window.

## Project structure

- `actions/` — desktop, browser, file, system, and other assistant actions
- `core/` — core assistant logic and supporting services
- `config/` — configuration examples and project assets
- `plugins/` — plugin modules
- `README.md` — project overview and quick start
- `SETUP_GUIDE.md` — detailed setup notes
- `BRANDING.md` — current project branding
- `CHANGELOG_LOCAL.md` — summary of local changes

## Security

- **Never commit API keys, passwords, tokens, or private configuration files.**
- Use `config/api_keys.json.example` as a template and keep your real credentials local.
- Review permissions before enabling actions that control the browser, files, or desktop.
- Only use automation features on systems and accounts you are authorized to control.

## Status

This project is under active development. Some integrations may require additional configuration, compatible dependencies, or API access. Test changes in your own environment before relying on them.

## License

See [LICENSE](LICENSE) for license details.
