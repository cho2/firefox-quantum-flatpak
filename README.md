# Firefox Quantum Flatpak

## Build and install locally

* `flatpak-builder --repo=repo firefox org.mozilla.Firefox.json.in`
* `flatpak build-export repo firefox`
* `flatpak --user remote-add --no-gpg-verify --if-not-exists firefox-repo repo`
* `flatpak --user install firefox-repo org.mozilla.Firefox`
* `flatpak run org.mozilla.Firefox`

## Bundling

* `flatpak build-bundle repo firefox.flatpak org.mozilla.Firefox`

## Issues
* Flash plugin not installed correctly
* Java plugin not installed correctly