# Este repositório contém minhas configurações pessoais para o BlendOS.
## 💻 Notebook ASUS Zenbook Duo 14 UX482EAR

### 📋 Especificões:
- Intel® Core™ i7-1165G7 (2.8 GHz, cache de 12 MB, até 4.7 GHz, 4 núcleos)
- Intel® Iris Xe Graphics
- 16 GB LPDDR4X integrada
- 1 TB M.2 NVMe™ PCIe® 3.0 SSD
- Wi-Fi 6E (802.11ax) (banda dupla) 2x2 + Bluetooth® 5.3
- Trusted Platform Module (TPM)
- Proteção de senha de inicialização da BIOS
- Trusted Platform Module (Firmware TPM)
- Webcam IR

## ⚙ [System.yaml](https://raw.githubusercontent.com/Gabriel-Freitas-S/track-personal/main/local/system.yaml)
```yaml
repo: 'https://pkg-repo.blendos.co' 

arch-repo: 'https://geo.mirror.pkgbuild.com' 

impl: 'https://github.com/Gabriel-Freitas-S/track-personal/raw/main' 

package-repos:
  - name: 'liquorix'
    repo-url: 'https://liquorix.net/archlinux/$repo/$arch'
  - name: 'chaotic-aur'
    repo-url: 'https://cdn-mirror.chaotic.cx/$repo/$arch'
  - name: 'arch-mact2'
    repo-url: 'https://mirror.funami.tech/$repo/os/$arch/'

commands:
  - 'sudo pacman-key --keyserver hkps://keyserver.ubuntu.com --recv-keys 9AE4078033F8024D'
  - 'sudo pacman-key --lsign-key 9AE4078033F8024D'
  - 'sudo pacman-key --recv-key FBA220DFC880C036 --keyserver keyserver.ubuntu.com'
  - 'sudo pacman-key --lsign-key FBA220DFC880C036'
  - 'sudo pacman -U ''https://cdn-mirror.chaotic.cx/chaotic-aur/chaotic-keyring.pkg.tar.zst'''
  - 'sudo pacman -U ''https://cdn-mirror.chaotic.cx/chaotic-aur/chaotic-mirrorlist.pkg.tar.zst'''
```
Este repositório está licenciado sob **The Unlicense**, que é uma licença de software livre que tem como objetivo colocar trabalhos que são de domínio público o mais livre possível. Isso significa que você pode copiar, modificar, distribuir e executar o trabalho, mesmo para fins comerciais, tudo sem precisar de permissão.

A licença The Unlicense afirma:

> This is free and unencumbered software released into the public domain.
>
> Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.

Portanto, o código-fonte e a documentação contidos neste repositório podem ser utilizados livremente, sem restrições de direitos autorais ou outras obrigações legais.

