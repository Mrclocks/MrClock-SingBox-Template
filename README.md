<div align="center">
  
# 📌 تمپلیت Sing-Box مخصوص پنل مرزبان - MrClock

<p align="center">
  <a href="#معرفی">معرفی</a> •
  <a href="#ویژگی‌ها">ویژگی‌ها</a> •
  <a href="#نصب">نصب</a> •
  <a href="#به‌روزرسانی">به‌روزرسانی</a>
</p>

</div>

<a name="معرفی"></a>
## ✏️ معرفی

<p dir="rtl">
تمپلیت سینگ باکس جهت استفاده هر چه بهتر از این اپلیکیشن قدرتمند که می‌تواند برای شما تجربه‌ای متفاوت نسبت به سایر اپلیکیشن‌ها به ارمغان بیاورد.
</p>

<a name="ویژگی‌ها"></a>
## ✨ ویژگی‌های کلیدی

<div dir="rtl" align="center">

| ویژگی          | توضیحات                                                                 |
|----------------|-------------------------------------------------------------------------|
| **⚡ انتخاب اتوماتیک** | اتصال اتوماتیک به سریع‌ترین پروکسی                           |
| **🚫 حذف تبلیغات** | حذف تبلیغات درون برنامه‌ای               |
| **📩 واتس اپ** | استفاده از واتس اپ بدون VPN               |
| **🌐 دامنه‌های ایرانی**  | اتصال به دامنه‌ها و اپ‌های ایرانی بدون نیاز به قطع VPN                                     |

</div>

<a name="نصب"></a>
## 📥 نصب و راه‌اندازی

<div>

### 1️⃣ دانلود فایل تمپلیت

</div>

```bash
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/Mrclocks/MrClock-SingBox-Template/main/default.json
```

<div>

### 2️⃣ ثبت تنظیمات در محیط مرزبان

</div>

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"' | sudo tee -a /opt/marzban/.env
```

<div>

#### 📝 روش جایگزین: اضافه کردن مستقیم به فایل `.env`

مقادیر زیر را مستقیماً در فایل `.env` واقع در `/opt/marzban/` اضافه کنید:

</div>

```bash
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.json"
```

<div>

### 3️⃣ راه‌اندازی مجدد مرزبان

</div>

```bash
marzban restart
```

<a name="به‌روزرسانی"></a>
## 🔄 به‌روزرسانی تمپلیت

<div dir="rtl" align="right">
  <p>برای دریافت آخرین نسخه تمپلیت، کافیست مرحله اول (دانلود فایل تمپلیت) را دوباره اجرا کنید.</p>
</div>

---

<div align="center">
  <p dir="rtl">🌟 اگر از این پروژه خوشتان آمد، لطفاً به آن ستاره دهید 🌟</p>
  
  <p>
    <a href="https://github.com/Mrclocks/MrClock-SingBox-Template">
      <img src="https://img.shields.io/github/stars/Mrclocks/MrClock-SingBox-Template?style=social" alt="ستاره‌های گیت‌هاب">
  </p>
  
  <p dir="rtl">با ❤️ توسط MrClock</p>
</div>
