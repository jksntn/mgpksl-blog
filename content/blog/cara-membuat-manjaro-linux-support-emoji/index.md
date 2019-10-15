---
type:        post
title:       Cara Membuat Manjaro Linux Support Emoji
date:        2019-07-09
description: >-
    Cara supaya instalan manjaro Linux kamu support menampilkan emoji seperti ini 😅😁😎.
tags:
 - notes
 
---

Setelah menginstall [manjaro][1] di Laptop saya, ada beberapa pengaturan yang harus disesuaikan supaya bisa berjalan seperti yang diinginkan, salah satunya adalah fungsi support terhadap emoji seperti ini 😅😁😎.  

Masalahnya ketika selesai instalasi, emoji yang biasa saya gunakan di blog tidak muncul di web browser yang saya gunakan, baik itu Google Chrome atau Mozilla Firefox. 

Setelah beberapa lama googling, ternyata tidak hanya menginstall font emoji, namun juga harus ada yang disesuaikan supaya emojinya muncul di Manjaro. Caranya cukup mudah:

### Install noto-fonts-emoji

Buka terminal, dan ketikkan perintah ini:

```php
sudo pacman -S noto-fonts-emoji
```

### Buat file local.conf

Buka terminal, dan ketikkan perintah ini:

```php
sudo cat > /etc/fonts/local.conf
```

Kemudian Isi file local.conf dengan konten seperti di bawah ini:

```xml
<?xml version="1.0"?>
<!DOCTYPE fontconfig SYSTEM "fonts.dtd">
<fontconfig>

 <alias>
   <family>sans-serif</family>
   <prefer>
     <family>Noto Sans</family>
     <family>Noto Color Emoji</family>
     <family>Noto Emoji</family>
     <family>DejaVu Sans</family>
   </prefer> 
 </alias>

 <alias>
   <family>serif</family>
   <prefer>
     <family>Noto Serif</family>
     <family>Noto Color Emoji</family>
     <family>Noto Emoji</family>
     <family>DejaVu Serif</family>
   </prefer>
 </alias>

 <alias>
  <family>monospace</family>
  <prefer>
    <family>Noto Mono</family>
    <family>Noto Color Emoji</family>
    <family>Noto Emoji</family>
   </prefer>
 </alias>

</fontconfig>
```

Semoga bermanfaat 👌

[1]: https://manjaro.org