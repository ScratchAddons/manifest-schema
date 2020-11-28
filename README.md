# manifest-schema

This repository hosts the schema for Scratch Addons' addon manifests.

[View the changelog](https://github.com/ScratchAddons/manifest-schema/wiki/Changelog).

## How-to

Add the pointed line to your manifest. Depending on your placement, you need to add a comma after the line. Reminder that this is optional.

```json5
{
    "$schema": "https://raw.githubusercontent.com/ScratchAddons/manifest-schema/master/1/1.4.json", // This one!
    "name": "...",
    ...
}
```

## Folder structure

```bash
.
└── 📂 1 # Folder with major version as the name
    └── 📜 1.0.json # Schema with both major and minor version as the name
```
