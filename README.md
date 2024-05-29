<p align="center">
  <a href="https://github.com/oXIIIo/marzban-template/" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
    </picture>
  </a>
</p>
<h1 align="center"/>تمپلیت های مختلف برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

# نصب
برای نصب تمپلیت‌های موجود دستورات زیر را در ترمینال سرور خود اجرا کنید:
1. دانلود فایل‌های تمپلیت
```sh
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/parsa-ghasemi/marzban-template/master/subscription/index.html
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/parsa-ghasemi/marzban-template/master/home/index.html
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
echo 'V2RAY_SUBSCRIPTION_TEMPLATE="v2ray/default.json"' | sudo tee -a /opt/marzban/.env
```
3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت ها فقط کافیست مرحله 1 را تکرار کنید.
