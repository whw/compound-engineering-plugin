# Fork Versioning Convention

For fork-specific changes, increment the fork number, not the patch version.

## Why

Fork changes should be tracked separately from upstream changes. The semver portion (`major.minor.patch`) tracks alignment with upstream, while `+fork.N` tracks fork-specific iterations.

## Wrong

```
2.24.0+fork.1 → 2.24.1+fork.1  # Incrementing patch for fork change
```

## Correct

```
2.24.0+fork.1 → 2.24.0+fork.2  # Incrementing fork number
```
