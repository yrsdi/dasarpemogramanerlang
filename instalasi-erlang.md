---
title: Instalasi Erlang
description: menjelaskan proses instalasi erlang di Linux, OSX dan Window
keywords: [erlang, belajar erlang, instalasi]
---

Instalasi Erlang sangat mudah, panduannya sudah tersedia lengkap untuk semua sistem operasi dan sudah tersedia di situs resmi erlang  https://www.erlang.org/downloads.

### Instalasi Erlang OSX & Linux

Di sini penulis mencoba membuat ringkas dengan memilih instalasi yang lebih simple, mudah dan cepat. Bagi anda yang menggunakan sistem operasi Linux atau OSX, [mise](https://mise.jdx.dev) bisa menjadi pilihan tepat. `mise` adalah global version manager yang digunakan untuk instalasi berbagai bahasa pemrograman dan sudah support banyak bahasa pemrograman termasuk erlang.

1. **Instalasi `mise`**
Target directory bisa disesuaikan, sesuaikan dengan sistem operasi anda : `~/bin`, `/usr/local/bin`, `~/.local/bin`

 **macos-arm64**
```bash
curl https://mise.jdx.dev/mise-latest-macos-arm64 > ~/.local/bin/mise
chmod +x ~/.local/bin/mise
```
**macos-x64**
```bash
curl https://mise.jdx.dev/mise-latest-macos-x64 > ~/.local/bin/mise
chmod +x ~/.local/bin/mise
```
**linux-x64**
```bash
curl https://mise.jdx.dev/mise-latest-linux-x64 > ~/.local/bin/mise
chmod +x ~/.local/bin/mise
```
**linux-arm64**
```bash
curl https://mise.jdx.dev/mise-latest-linux-arm64 > ~/.local/bin/mise
chmod +x ~/.local/bin/mise
```

2. **Activate `mise`**
 **.bashrc**
```bash
echo 'eval "$(~/.local/bin/mise activate bash)"' >> ~/.bashrc
```
  **.zshrc**
```bash
echo 'eval "$(~/.local/bin/mise activate zsh)"' >> ~/.zshrc
```
**fish**
```bash
echo '~/.local/bin/mise activate fish | source' >> ~/.config/fish/config.fish
```

3. **Install Erlang**
command berikut akan menginstall erlang versi 26 dan berlaku untuk global penggunaan.
```bash
mise use -g erlang@26
```
### Instalasi Erlang di Windows

1. Download telebih dahulu installer-nya di https://www.erlang.org/downloads.
2. Jalankan exe program dan ikuti instruksinya

Buka Command Prompt / CMD dan eksekusi perintah berikut untuk mengecek vesi erlang
```bash
erl --version

Erlang/OTP 26 [erts-14.2.5] [source] [64-bit] [smp:8:8] [ds:8:8:10] [async-  threads:1] [jit]

Eshell V14.2.5 (press Ctrl+G to abort, type help(). for help)
1>
```
