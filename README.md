# ABAJ Monitor — публичная раздача APK

Прямая загрузка (без авторизации GitHub):

- [Admin APK](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/ABAJ-Monitor-Admin.apk)
- [Client APK](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/ABAJ-Monitor-Client.apk)

JSON для настройки обновлений в соответствующем приложении:

- [admin-updates.json](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/admin-updates.json)
- [client-updates.json](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/client-updates.json)

Исходный Android-проект хранится в приватной ветке `edgar198282-ux/Test-test:traffic-ai-armenia-v0.9`. Взаимодействие клиентов происходит только с явным разрешением на геолокацию, через сторонний HTTPS-ретранслятор; без Railway и Tailscale. Камера и микрофон не реализованы.

APK 0.4.0 подписаны тестовым ключом, прежде чем обновлять, необходимо проверить подпись и предусмотреть постоянную безопасную подпись релизов.
