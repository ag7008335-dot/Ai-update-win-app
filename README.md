# Pylon Win App — Update Server

این ریپو فقط برای **آپدیت خودکار Pylon** روی ویندوز است.

## فایل‌ها

| فایل | کاربرد |
|------|--------|
| `version.json` | manifest که برنامه از Settings → System Update می‌خواند |

## انتشار نسخه جدید

1. `APP_VERSION` را در ریپوی [pylon](https://github.com/ag7008335-dot/pylon) آپدیت کن.
2. exe را با PyInstaller بساز (`Pylon.exe`).
3. در **GitHub Releases** این ریپو یک release بساز:
   - Tag: `v1.0.0` (مثال)
   - Asset: `Pylon.exe`
4. `version.json` را آپدیت کن:
   - `version` — نسخه جدید
   - `url` — لینک مستقیم دانلود exe همان release
   - `notes` — توضیحات تغییرات
5. commit و push به `main`.

## URL خوانده‌شده توسط برنامه

```
https://raw.githubusercontent.com/ag7008335-dot/Ai-update-win-app/refs/heads/main/version.json
```

## نسخه فعلی

- **1.0.0** — اولین نسخه پایدار Pylon Win App
