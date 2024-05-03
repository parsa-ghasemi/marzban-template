<p align="center">
  <a href="https://github.com/WhyMan1/marzban-template/tree/master/subscription" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/PreviewTemplate.png">
      <img width="372" height="408" src="https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/PreviewTemplate.png">
    </picture>
  </a>
</p>
<h1 align="center"/>قالب سابسکریپشن برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

## فهرست مطالب
- [ویژگی‌ ها](#ویژگی-ها)
- [مراحل نصب](#مراحل-نصب)

# مقدمه
یک قالب html ساده برای نمایش بهتر اطلاعات کاربر

# ویژگی ها
- افزودن سریع لینک سابسکریپشن به برنامه های v2rayNG، Streisand، NekoBox و sing-box
- لینک دانلود اپلیکیشن های مورد نیاز

# مراحل نصب
1. دانلود فایل template
```sh
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/index.html
```

2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت فقط کافیست مرحله 1 را تکرار کنید.

# شخصی سازی
برای شخصی سازی ایدی تلگرام, تصویر پس زمینه و لوگوی کاربر باید تغییراتی در فایل html لحاظ شود که با سرچ کردن برخی مقادیر امکان پذیره.
برای سرچ کردن با استفاده از nano ابتدا فایل را با nano با دستور زیر باز کنید:
```
nano /var/lib/marzban/templates/subscription/index.html
```
سپس با دکمه های ترکیبی Ctrl + W سرچ بار رو باز کنید و برای عوض کردن ایدی پشتیبانی تلگرام عبارت زیر رو سرچ کنید:
```
https://t.me/yourID
```
برای لوگوی کاربر این عبارتو سرچ کنید:
```
images/marzban.svg
```
برای تصویر پس زمینه این عبارتو سرچ کنید:
```
background: url('https://4kwallpapers.com
```
پس از اعمال تغییرات فایل رو سیو کنید و مرزبان رو ریستارت کنید.

## کپی رایت
این قالب توسط  https://github.com/x0sina/marzban-sub ساخته شده است.

# حمایت از من

<a href="https://nowpayments.io/donation?api_key=WE3KFT5-2VKMNSF-N1P4YQ6-24N82ZA&source=lk_donation&medium=referral" target="_blank">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>
