<h1 align="center">
  <br>
  <a href="https://apiku.id/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://apiku.id/wp-content/uploads/2023/12/cropped-logo.png">
      <img alt="apiku logo" src="https://apiku.id/wp-content/uploads/2023/12/cropped-logo.png" height="100">
    </picture>
  </a>
  <br>
</h1>
Selamat datang, Penggunaan example-config.yml dapat lakukan copy paste file isi example-config.yml. jika ada issue atau ingin costume bisa open issue.

# Introduction
## Changelog
- 24/07/2024 First Update !

# Requirements
Basic Knowledge
- BIRD2
- pathvector
  
# pathvector.yml
configuration pathvector

BGP Debian bird2 & pathvector
[Debian 11]
download pathvector
```
curl https://repo.pathvector.io/pgp.asc > /usr/share/keyrings/pathvector.asc
echo "deb [signed-by=/usr/share/keyrings/pathvector.asc] https://repo.pathvector.io/apt/ stable main" > /etc/apt/sources.list.d/pathvector.list
apt update && apt install -y pathvector
```

config pathvector have update on 
```
nano /etc/pathvector.yml
```
copy and edit isi example-config.yml
save file
lanjutkan perintah di bawah ini :
```
sudo apt install bird2
```
```
sudo systemctl enable --now bird
```
( if need can skip)
```
sudo apt install bgpq4 
```
```
sudo pathvector generate
```

periksa apakah status berjalan dengan normal 
```
sudo pathvector status
```

fungsi next hope jika di perlukan
```
next-hop-self: true
listen4: ip-vps
listen6: ip-vps
```

# Sponsor Developer
- - - - - - - - - - - - - - - -
BCA : -

BCA Digital: -

Jago : -

Paypal: -
- - - - - - - - - - - - - - - -
Sponsor will honorer publish on link https://binsaryunus.my.id/sponsor-as215084/
