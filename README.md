# Nerd Nova | Field Notes

Responsive technical field journal, hosted on GitHub Pages. Includes search, categories, sanitized example commands, in-browser editing, and direct GitHub saves.

## Publish

Repository Settings → Pages → Build and deployment → Deploy from a branch → `main` → `/(root)` → Save.

## Editing from mobile or desktop

Open the app and choose **⚙ Sync**. Create a GitHub fine-grained personal access token restricted to this repository, with **Contents: Read and write** permission. Use the token in the Sync screen. The token stays in this browser tab's session storage and is not committed to the repository. Use **Disconnect** when finished. You may need to reconnect on a new device/tab.

The app saves note and category changes to `data.json` using GitHub's Contents API, creating a commit on `main`. Public read access works without a token. GitHub Pages deploys the new notes after each commit. Manual editing of `data.json` concurrently with the app can cause conflicts; verify recent changes before large edits.

## Security

This repository and published notes are public. Never enter real operational IPs, internal paths, hostnames, credentials, logs, controlled information, or otherwise restricted details. Git history retains prior versions even after deleting a note. Only enter pre-sanitized generic examples. Avoid storing tokens outside the sync field.
