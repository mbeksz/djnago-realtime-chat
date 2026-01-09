Django Realtime Chat

Bu proje, Django ve Django Channels kullanılarak geliştirilmiş basit bir gerçek zamanlı sohbet uygulamasıdır. WebSocket altyapısı sayesinde kullanıcılar mesajları anlık olarak alıp gönderebilir.

Özellikler

Gerçek zamanlı mesajlaşma

WebSocket desteği (Django Channels)

Basit ve anlaşılır arayüz

Django tabanlı yapı

Gereksinimler

Python 3.8+

Django

Django Channels

Kurulum
git clone https://github.com/mbeksz/djnago-realtime-chat.git
cd djnago-realtime-chat
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt

Çalıştırma
python manage.py migrate
python manage.py runserver


Tarayıcıdan http://127.0.0.1:8000/ adresine giderek uygulamayı kullanabilirsiniz.

Proje Amacı

Django ile WebSocket mantığını ve gerçek zamanlı iletişimi öğrenmek için örnek bir projedir.
