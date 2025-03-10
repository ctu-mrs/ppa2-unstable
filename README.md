# PPA2 Unstable

Personal Package Archive (PPA) for unstable ROS2 MRS deb packages.

## Adding the PPA

```bash
curl https://ctu-mrs.github.io/ppa2-unstable/add_ppa.sh | bash
```

## Uninstalling packages from this PPA

```bash
sudo apt-get -y install aptitude
sudo apt remove $(aptitude search -F '%p' '~S ~i ?origin("ctu-mrs") ?label("unstable")')
```

## Removing the PPA

```bash
curl https://ctu-mrs.github.io/ppa2-unstable/remove_ppa.sh | bash
```
