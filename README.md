# thiqa-shared

Small Python package for code shared between ThiqaScore backend services
(`thiqa-backend` and `thiqa-id-worker`), so it can't drift into two
independently-maintained copies.

## Usage

Add as a git dependency pinned to a tag, e.g.:

```
thiqa-shared @ git+https://github.com/abulotus/thiqa-shared.git@v0.1.0
```

When you change something here, bump the version in `pyproject.toml`, tag a
release (`git tag vX.Y.Z && git push --tags`), and bump the pinned tag in each
consumer repo.
