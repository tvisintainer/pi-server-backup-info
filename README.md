# Pi Server Backup — public information site

Public app-description and privacy pages only. No server configuration, backup logs, tokens or secrets belong in this repository.

## Publish through GitHub's website
1. Create a public repository named pi-server-backup-info. Initialize with a README so main exists.
2. Upload index.html, privacy.html and style.css to the repository root (not inside a folder). Commit the files to main.
3. Settings > Pages > Build and deployment: Deploy from a branch; main; / (root); Save.
4. Wait for GitHub to report the published URL and open both the homepage and privacy.html to verify them.

Expected URL pattern (replace YOUR-USERNAME, do not paste this placeholder into Google):
- https://YOUR-USERNAME.github.io/pi-server-backup-info/
- https://YOUR-USERNAME.github.io/pi-server-backup-info/privacy.html

In Google Auth Platform > Branding, enter the actual published home page and privacy policy URLs. Use YOUR-USERNAME.github.io as the authorized domain, without a scheme or path. If Google rejects that domain or requires ownership verification, follow its message and use a domain you control; do not substitute github.com or a local Pi address.

Save Branding, return to Audience and publish the OAuth application. Then reconnect the existing rclone remote using the same config file. Publishing the information site or OAuth app does not repair an expired token by itself.

Review the policy against the actual server configuration before publishing. It describes intended personal backup use and does not claim Google verification or certification.
