---

# funos-updates

**funos-updates** is the official update repository for **FunOS**.
It provides a simple, lightweight, and transparent way to deliver FunOS-specific updates outside of the standard APT system.

This repository works together with the `funos-update` command-line tool.

---

## What Is This Repository For?

FunOS aims to stay **light, minimal, and stable**.
Not all improvements or fixes belong in traditional system packages.
Some updates are better delivered as small, targeted changes.

This repository is used to distribute:

* New wallpapers and artwork
* JWM themes and visual enhancements
* Configuration improvements
* Bug fixes and maintenance scripts
* Optional package installation or adjustments

All updates are **modular**, **version-independent**, and **applied only with user consent**.

---

## How Updates Work

1. A FunOS user runs:

   ```bash
   funos-update
   ```

2. The tool fetches update metadata from this repository.

3. Available updates are listed with clear descriptions.

4. The user chooses whether to apply each update.

5. Applied updates are recorded locally to prevent reinstallation.

Nothing is installed automatically, and nothing is hidden from the user.

---

## Design Principles

This update system is intentionally simple:

* ✅ No automatic updates
* ✅ No forced upgrades
* ✅ No interference with APT
* ✅ Fully auditable and transparent
* ✅ User consent is always required

The goal is to improve FunOS without sacrificing control or simplicity.

---

## Repository Structure (Overview)

```text
funos-updates/
├── updates.json        # Update metadata
├── wallpapers/         # New wallpapers and artwork
├── jwm-themes/         # JWM themes
├── scripts/            # Fixes and maintenance scripts
```

Each update is defined in `updates.json` and handled individually by `funos-update`.

---

## Target Audience

This repository is intended for:

* FunOS users who want safe and optional updates
* FunOS maintainers and contributors
* Developers who prefer transparent, script-based maintenance

---

## License

This repository follows the same licensing principles as FunOS.
Please check individual files or directories for specific license information.

---
