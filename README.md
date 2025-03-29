<h1 align="center" dir="rtl">📌 تمپلیت Sing-Box مخصوص پنل مرزبان - MrClock</h1>



---

## ✏️ معرفی

<p dir="rtl">
تمپلیت سینگ باکس جهت استفاده هر چه بهتر از این اپلیکیشن قدرتمند که می تواند برای شما تجربه ای متفاوت نسبت به سایر اپلیکیشن ها به ارمغان بیاورد .
</p>

---

## ✨ ویژگی‌های کلیدی

<div align="center" dir="rtl">

| ویژگی          | توضیحات                                                                 |
|----------------|-------------------------------------------------------------------------|
| **⚡ انتخاب اتوماتیک** | اتصال اتوماتیک به سریع ترین پروکسی                           |
| **🚫 حذف تبلیغات** | حذف تبلیغات درون برنامه ای               |
| **🌐 دامنه های ایرانی**  | اتصال به دامنه ها و اپ های ایرانی بدون نیاز قطع VPN                                     |

</div>

---


## 📥 نصب اولیه

<p dir="rtl">

### 1- دانلود فایل تمپلیت:
</p>

   ```bash
   sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/Mrclocks/MrClock-SingBox-Template/main/default.json
   ```

<p dir="rtl">

### 2- ثبت تنظیمات در محیط مرزبان:
</p>

   ```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"' | sudo tee -a /opt/marzban/.env
   ```

<p dir="rtl">

#### یا مقادیر زیر را مستقیماً در فایل `.env` واقع در `/opt/marzban/` اضافه کنید:
 </p>

   ```bash
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"
   ```

<p dir="rtl">

### 3- راه‌اندازی مجدد مرزبان:
</p>

   ```bash
   marzban restart
   ```

---

## 🔄 به‌روزرسانی تمپلیت

##### برای دریافت آخرین نسخه تمپلیت، کافیست مرحله اول (دانلود فایل تمپلیت) را دوباره اجرا کنید.









