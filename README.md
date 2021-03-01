# manifest-schema

This repository hosts the schema for Scratch Addons' addon manifests.

[View the changelog](https://github.com/ScratchAddons/manifest-schema/wiki/Changelog).

## How-to

Add the pointed line to your manifest. Depending on your placement, you need to add a comma after the line. Reminder that this is optional.

```json5
{
    "$schema": "https://raw.githubusercontent.com/ScratchAddons/manifest-schema/dist/schema.json", // This one!
    "name": "...",
    ...
}
```

## Versioning

The versioning consist of the major version and the minor version. The major version is rarely bumped, because it is reserved for very, very, large changes.

In most times, you bump the minor once there is a new feature, but for Scratch Addons, there are some special cases that you need to know.

1. Bump the minor version only if the new minor version of Scratch Addons requires changes on the schema.
This means if there are no changes needed on the schema on a certain minor version of SA, there's no need to bump. This also means that the schema's versioning is seperate from SA's versioning. (e.q. SA 1.6.x doesn't need changes on the schema, so bumping is skipped and SA 1.7.x gets the previous schema version)
2. Mind the grammar on the description.
Most of the times it is a noun phrase, but sometimes it is a proper sentence. Either way, you need to use proper grammar on the description.

## Folder structure

```bash
.
└── 📂 1 # Folder with major version as the name
    └── 📜 1.0.json # Schema with both major and minor versions as the name
```
