# folding-at-home
Repo that stores installation instructions

### Source
[Folding at Home](https://foldingathome.org/faqs/installation-guides/linux/manual-installation-optional-advanced/terminal-installation-for-debian-mint-ubuntu/?lng=en)

```
wget https://download.foldingathome.org/releases/public/release/fahclient/debian-testing-64bit/v7.4/fahclient_7.4.4_amd64.deb
wget https://download.foldingathome.org/releases/public/release/fahcontrol/debian-testing-64bit/v7.4/fahcontrol_7.4.4-1_all.deb
wget https://download.foldingathome.org/releases/public/release/fahviewer/debian-testing-64bit/v7.4/fahviewer_7.4.4_amd64.deb
```

```
sudo dpkg -i --force-depends fahclient_7.4.4_amd64.deb
```

```
sudo dpkg -i --force-depends fahcontrol_7.4.4-1_all.deb
```

```
sudo dpkg -i --force-depends fahviewer_7.4.4_amd64.deb
```

```
apt install python3-stdeb python3-gi python3-all python3-six debhelper dh-python gir1.2-gtk-3.0
```

```
git clone https://github.com/cdberkstresser/fah-control.git
cd fah-control
echo "version = '7.7.0'" > fah/Version.py
./FAHControl
```
