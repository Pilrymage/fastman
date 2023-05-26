# scoop

## Powershell 策略

```pwsh
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

## 输出

```pwsh
irm get.scoop.sh -outfile 'install.ps1'
.\install.ps1 -?
.\install.ps1 -ScoopDir 'D:\Windows\Scoop' -ScoopGlobalDir 'D:\GlobalScoopApps' -NoProxy
scoop install 7zip git ffmpeg sudo
scoop bucket add extras
scoop install vscode qbittorrent rufus nomacs
scoop bucket add chawyehsu_dorado https://github.com/chawyehsu/dorado
scoop install chawyehsu_dorado/clash-for-windows-np