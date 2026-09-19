# Tekken Tag Tournament Arcade — Web

هدف این مخزن اجرای نسخه Arcade بازی Tekken Tag Tournament با فایل ROM شخصی کاربر در مرورگر است.

## نکته مهم فنی

Tekken Tag Tournament Arcade برای **Namco System 12** است و در MAME با شناسه **tektagt** شناخته می‌شود. سورس رسمی MAME درایور Namco System 12 و نسخه‌های Tekken Tag را دارد.

نسخه‌های قبلی EmulatorJS که در پروژه تست شدند، هسته MAME مناسب برای این بازی را ارائه نمی‌کردند؛ بنابراین استفاده از `EJS_core="mame"` راه‌حل نهایی نیست.

هدف این پروژه استفاده از یک **MAME 0.139 / MAME 2010 WebAssembly** سازگار با `tektagt` است.

## ساختار هدف

```
/
├── index.html
├── tektagt.zip              # فایل ROM کاربر؛ داخل GitHub قرار نمی‌گیرد
├── emulatorjs/
│   └── data/
└── core/
    └── mame2010/            # هسته WebAssembly پروژه
```

## وضعیت

- [x] ریپوی GitHub ایجاد و متصل شد.
- [x] شناسه بازی `tektagt` تأیید شد.
- [x] Namco System 12 تأیید شد.
- [x] مشخص شد MAME 2010 / 0.139 یک گزینه مناسب برای این ROMset است.
- [ ] ساخت هسته WebAssembly مخصوص مرورگر.
- [ ] تست اجرای `tektagt.zip`.
- [ ] انتقال فایل‌های نهایی به هاست DirectAdmin.

**ROM بازی و فایل‌های دارای حق نشر در این مخزن قرار داده نمی‌شوند.**
