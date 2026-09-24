# Shelf builds

Unofficial builds of Shelf. Each release carries the installable zip, the update bundle and `latest.json`, which the app reads for updates. Not notarised.

## Install

```
curl -fsSL https://github.com/neakoh/shelf-releases/releases/latest/download/Shelf-macos-x64.zip -o /tmp/Shelf.zip && ditto -x -k /tmp/Shelf.zip /Applications && open /Applications/Shelf.app
```

Downloaded with a browser instead, the zip is quarantined and macOS refuses the app once: `xattr -dr com.apple.quarantine ~/Downloads/Shelf.app`, then move it to Applications.
