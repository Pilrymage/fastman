# WSL

```pwsh
wsl --import Gentoo D:\Windows\AppData\Local\WSL\Gentoo\ .\stage3-amd64-openrc-20211121T170545Z.tar --version 2
wsl -d Gentoo
wsl -u root -d Gentoo
```

```sh
useradd -m -G wheel pilrymage
passwd pilrymage
cat > /etc/wsl.conf << "EOF"
[user]
default=larry
EOF
```

```pwsh
wsl --terminate Gentoo
