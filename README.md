# cgenius-flatpak

Commander Genius Flatpak support

# Building

```
flatpak-builder build-dir io.sourceforge.clonekeenplus.yml
```

# Installing it

```
flatpak-builder --user --install build-dir io.sourceforge.clonekeenplus.yml
```

# Running it

```
flatpak run io.sourceforge.clonekeenplus
```

# Linting

## Install linter

```
flatpak install flathub -y org.flatpak.Builder
```

## Test the linter command
```
flatpak run --command=flatpak-builder-lint org.flatpak.Builder --help
```

## Lint the Commander Genius build directory
```
flatpak run --command=flatpak-builder-lint org.flatpak.Builder builddir build-dir
```
