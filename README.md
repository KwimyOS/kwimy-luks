# kwimy-luks

Plymouth theme for encrypted (LUKS) boots in Kwimy

## Install path

- `/usr/share/plymouth/themes/kwimy-luks`

## Files

- `kwimy-luks.plymouth`: theme descriptor
- `kwimy-luks.script`: Plymouth script
- `entry.png`, `lock.png`, `bullet.png`, `logo-luks.png`: theme assets
- `throbber-*.png`: animation frames

## Package

Built from this directory via `PKGBUILD` and installed as the `kwimy-luks` package

## Notes

- Default theme selection is handled by the installer based on disk encryption
