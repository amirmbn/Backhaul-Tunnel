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
 - توقف و پاک‌سازی کامل تانل از روی سرور اوبونتو
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
