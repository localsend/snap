[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/localsend-uno)

Note: This is an unofficial repackaging and is not endorsed by the upstream project. The upstream Localsend project can be found [here](https://github.com/localsend/localsend).

## Want to build the snap yourself?

Before you begin
- Ensure you have snapd installed
- Ensure you have git installed

How to set up snapcraft
- Install snapcraft: run `sudo snap install snapcraft --classic`
- Install lxd: run `sudo snap install lxd`
- Add your user to the lxd group: run `sudo usermod -aG lxd $USER`
- Reboot your computer
- Configure lxd: run `lxd init --minimal`

How to build the snap
- Enter a nice working directory (e.g. ~/projects)
- Download repo: run `git clone --depth=1 https://github.com/thatLeaflet/localsend-snap.git && cd localsend-snap`
- Build the snap: run `SNAPCRAFT_ENABLE_EXPERIMENTAL_EXTENSIONS=1 snapcraft`
- Install the snap: run `sudo snap install ./<file-name> --dangerous`
