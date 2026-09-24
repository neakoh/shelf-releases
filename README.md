# Shelf builds

Unofficial builds of Shelf. Each release carries the installable zip, the update bundle and `latest.json`, which the app reads for updates. Not notarised.

## Install

```
curl -fsSL https://github.com/neakoh/shelf-releases/releases/latest/download/Shelf-macos-x64.zip -o /tmp/Shelf.zip && rm -rf /Applications/Shelf.app && ditto -x -k /tmp/Shelf.zip /Applications && xattr -dr com.apple.quarantine /Applications/Shelf.app; open /Applications/Shelf.app
```

If macOS still says it could not verify the app is free of malware, it is a quarantined copy: run `xattr -dr com.apple.quarantine /Applications/Shelf.app` and open it again.
