# ABAJ Monitor v0.4.1 — APK для своих устройств

Прямое скачивание без входа GitHub:

- [Admin v0.4.1](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/ABAJ-Monitor-Admin.apk)
- [Client v0.4.1](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/ABAJ-Monitor-Client.apk)

Для автообновлений в настройках APK один раз установи соответствующий URL:

- Admin: https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/admin-updates.json
- Client: https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/client-updates.json

Admin v0.4.1 исправляет сохранение ключей через Android KeyStore (IV формирует Keystore, проверяется запись). Оба APK тестовые, подписаны тем же тестовым сертификатом, что и 0.4.0, и собирались из приватного проекта. Система не использует Railway и Tailscale. Для передачи GPS используется внешний HTTPS-ретранслятор, координаты зашифрованы. На клиенте включение GPS добровольное, Android показывает уведомление с кнопкой остановки. Камера и микрофон не реализованы.

SHA-256:
- Admin: fa0b21656bc0d997f49227c771af9160a9dd8153055c5a12fa1078b1f6f4956c
- Client: f81521c8d26e7fddc375fdcd14ae9083c5875ec2498bab8350658a21a53a026c

Установка/обновление APK требует подтверждения Android.
