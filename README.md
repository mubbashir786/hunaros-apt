# HunarOS APT repository

Signed packages for [HunarOS](https://tajsolution.com), served with GitHub Pages at
**https://mubbashir786.github.io/hunaros-apt**. HunarOS systems use it automatically (HunarOS Update).
This repository only holds built packages; it is written by HunarOS CI.

Add it by hand on Ubuntu 24.04 (noble):

```bash
sudo curl -fsSLo /usr/share/keyrings/hunaros-archive-keyring.gpg https://mubbashir786.github.io/hunaros-apt/hunaros-archive-keyring.gpg
printf 'Types: deb\nURIs: https://mubbashir786.github.io/hunaros-apt\nSuites: noble\nComponents: main\nSigned-By: /usr/share/keyrings/hunaros-archive-keyring.gpg\n' | sudo tee /etc/apt/sources.list.d/hunaros.sources
sudo apt update
```

Signing key fingerprint: `7515C0BF2A68C8E640CD2DD016774464D93C8ED8`

HunarOS is a product of TajSolution.com. Packages: GPL-3.0 (see each package's copyright file).
