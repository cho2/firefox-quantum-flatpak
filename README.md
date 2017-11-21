# Firefox Quantum Flatpak

## Build and install locally

* `flatpak-builder --repo=repo firefox org.mozilla.Firefox.json.in`
* `flatpak build-export repo firefox`
* `flatpak --user remote-add --no-gpg-verify --if-not-exists firefox-repo repo`
* `flatpak --user install firefox-repo org.mozilla.Firefox`
* `flatpak run org.mozilla.Firefox`

## Bundling

* `flatpak build-bundle repo firefox.flatpak org.mozilla.Firefox`
* `flatpak build-import-bundle repo firefox.flatpak`

## Issues
* Flash plugin not installed correctly
* Java plugin not installed correctly
* Error when install `firefox.flatpak`
```
error: GDBus.Error:org.gtk.GDBus.UnmappedGError.Quark._g_2dio_2derror_2dquark.Code0: Extra data missing in detached metadata
````