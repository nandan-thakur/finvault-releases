# FinVault

A private, local-first vault for your cards, logins, IDs, documents and secure notes - on Android. No account or sign-up is needed.

## What it holds

- **Cards** - credit & debit cards, with network detection and expiry warnings
- **Logins** - usernames & passwords, with autofill in apps and browsers
- **IDs** - identity documents, with photos
- **Docs** - encrypted files you can share or save out when you choose
- **Notes** - secure notes

## How it protects your data

- The vault database is encrypted (SQLCipher), with keys protected by the Android Keystore.
- Lock: fingerprint-first, with a PIN fallback.
- No account, and no analytics or advertising SDKs. Internet access is used only for features you choose: encrypted backup to your own Google Drive, and delivery of the on-device text-recognition component used for card scanning (via Google Play services).
- Backups (file export or Google Drive) are encrypted with a passphrase you choose (Argon2id).

## Install

Requires Android 10 or later.

1. Open the latest release on this page and download the APK under Assets.
2. Open the downloaded file. Android will ask you to allow installs from your browser or file manager - allow it once.
3. Open FinVault and set up your lock.

If you used an earlier test build: the release here is signed differently and cannot install over it. Keep the test build until your release download is ready; then export a backup from the test build, check the backup restores, and only then uninstall the test build and install the release. Uninstalling deletes the vault.

## Updating

Later releases of this same signed app are intended to install over the top: download the newest APK and install it without uninstalling. Uninstalling deletes the vault, so keep a current backup before any update.

## Backup & restore

In Settings, open the backup section. Backups are written only when you ask. Restoring replaces the current vault contents with the backup's contents. Backups are encrypted with your passphrase; if you forget it, that backup cannot be recovered - keep it somewhere safe. Android's automatic cloud backup is off for this app, so if the phone is lost or the app is uninstalled without your own backup, the vault cannot be recovered.

## Notes

- This is a personal project shared as-is.
- The source code is private; this page only distributes the app.
