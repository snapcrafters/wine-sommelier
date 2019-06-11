# Sommelier Template

WINE-Sommelier is a wrapper and Snapcraft build script that will take your Windows application and wrap it into a Snap-based WINE environment for use on many Linux-based operating systems.

## Compatibility

Unfortunately, due to the nature of the WINE system, your Windows application might not work in this wrapper. Please be aware of this and be prepared for failure to launch.

## Steps to customise

Use GitHub's template repository feature to create a copy of this repository in your account.

You will need to:

- Change the `name` and `version` fields in `snapcraft.yaml`.
- Set the URL to a publicly available installer for your application in `snapcraft.yaml` in the `environment` block's `INSTALL_URL` line.
- Set the URL to your support channel in the `environment` block in `snapcraft.yaml` in the `SNAP_SUPPORT_URL` line.
- Edit `desktop-file.desktop` to add your application's snap name in the `Exec=` line, the human-readable name in the `Name=` line, and a Comment/description in the `comment=` line.