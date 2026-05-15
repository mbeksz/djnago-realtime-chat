# Django Gerçek Zamanlı Sohbet Uygulaması

<p align="center">
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=socketdotio&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
</p>

---

## Genel Bakış

Django ve Django Channels kullanılarak geliştirilmiş **gerçek zamanlı sohbet uygulaması**. WebSocket altyapısı sayesinde kullanıcılar mesajları anlık olarak alıp gönderebilir. Oda bazlı sohbet ve kullanıcı kimlik doğrulama sistemi içerir.

---

## Teknoloji Yığını

```
Backend    → Python · Django
WebSocket  → Django Channels
Önbellek   → Redis (channel layer)
Auth       → Django Authentication
```

---

## Mimari

```
a_core/          # Django proje ayarları
a_home/          # Ana sayfa ve oda listesi
a_rtchat/        # WebSocket consumer ve sohbet mantığı
a_users/         # Kullanıcı kayıt ve profil
templates/       # HTML şablonları
static/          # CSS, JS
```

---

## Kurulum

```bash
git clone https://github.com/mbeksz/djnago-realtime-chat
cd djnago-realtime-chat
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Tarayıcıdan `http://127.0.0.1:8000/` adresine giderek uygulamayı kullanabilirsiniz.

---

## Özellikler

- WebSocket ile anlık iki yönlü mesajlaşma
- Oda bazlı sohbet desteği
- Kullanıcı kayıt ve kimlik doğrulama
- Django Channels ile ASGI mimarisi
