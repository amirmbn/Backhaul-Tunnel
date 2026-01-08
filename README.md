# Backhaul Installer
<br>

<div align="right">
 - تست و بررسی‌های پروژه انجام شده و قابل بهره‌برداری است.
</div>
<div align="left">

## Automatic Installation

</div>
<div align="right">
<br>
 - کد زیر را در سرور اوبونتو خود Past کنید
<br><br>
</div>
<div align="left">

```
sudo wget -4 https://raw.githubusercontent.com/amirmbn/Backhaul-Installer/main/backhaul_install.sh && sudo chmod +x backhaul_install.sh && sudo ./backhaul_install.sh
```
</div>
<div align="right">
<br>
 - برای بررسی وضعیت سرویس از کد زیر استفاده کنید
<br><br>
</div>
<div align="left">

```
sudo systemctl status backhaul.service
```
</div>
<div align="right">
<br>
 - برای بررسی آخرین لاگ های backhaul از کد زیر استفاده کنید
<br><br>
</div>
<div align="left">

```
journalctl -u backhaul.service -e -f
```
</div>
<div align="right">
<br>
 - ⛔ متوقف کردن سرویس
<br><br>
</div>
<div align="left">

```
sudo systemctl stop backhaul.service
sudo systemctl status backhaul.service
```
</div>
<div align="right">
<br>
  
### راه‌اندازی مجدد سرویس (Start / Restart)
<br><br>
شروع مجدد:
<br><br>
</div>
<div align="left">

```
sudo systemctl start backhaul.service
```
</div>
<div align="right">
<br>
 - ری‌استارت (بعد از تغییر تنظیمات حتماً از این استفاده کن):
<br><br>
</div>
<div align="left">

```
sudo systemctl restart backhaul.service
```
</div>
<div align="right">
<br>
 - توقف و حذف کامل تانل از روی سرور اوبونتو
<br><br>
</div>
<div align="left">

```
sudo systemctl stop backhaul
sudo systemctl disable backhaul
sudo rm -f /etc/systemd/system/backhaul.service
sudo systemctl daemon-reload
sudo rm -f /root/backhaul /root/config.toml /root/backhaul.json backhaul_install.sh
```
</div>

## 💰 Support This Project with Crypto
[![Donate BTC](https://img.shields.io/badge/Donate-BTC-orange)](https://www.blockchain.com/btc/address/bc1qul4v4rudyl7lacekfp8yda5sc5575mh2tzv9au)
[![Donate ETH](https://img.shields.io/badge/Donate-ETH-purple)](https://etherscan.io/address/0x79Bb867649277272C65ae047083A36ea91DFeE5B)
[![Donate TRX](https://img.shields.io/badge/Donate-TRX-red)](https://tronscan.org/#/address/TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6)
[![Donate USDT](https://img.shields.io/badge/Donate-USDT-green)](https://tronscan.org/#/address/TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6)

- Bitcoin `bc1qul4v4rudyl7lacekfp8yda5sc5575mh2tzv9au`

- Ethereum `0x79Bb867649277272C65ae047083A36ea91DFeE5B`

- Tron `TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6`

- Tether (TRC20) `TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6`

Thank you for your support!
