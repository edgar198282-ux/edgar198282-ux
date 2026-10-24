# ABAJ Monitor — установочные APK и автообновление

Версия **0.5.0**: автоматическая проверка обновлений в Admin и Client, без ручного ввода ссылок. Скачивание проверяет SHA-256, установку подтверждает Android.

- [ABAJ Monitor Admin](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/ABAJ-Monitor-Admin.apk?v=6)
- [ABAJ Monitor Client](https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/ABAJ-Monitor-Client.apk?v=6)

Стабильные манифесты (HTTPS):
- Admin: https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/admin-updates.json
- Client: https://raw.githubusercontent.com/edgar198282-ux/edgar198282-ux/abaj-monitor-downloads/client-updates.json

Светлая/тёмная темы и GPS сохранены. Камера/звук: администратор может отправить зашифрованный запрос, Client покажет уведомление и предоставит локальную проверку камеры/микрофона после подтверждения на самом телефоне. **Удалённой аудио- и видеотрансляции пока нет**. Передача GPS идёт через сторонний HTTPS relay ntfy.sh (не Railway, не Tailscale). Защитите ключ привязки.

Выпуски тестовые, подпись совместима с 0.4.1 и НЕ должна использоваться в production. Для полноценного релиза требуется безопасно хранимый сертификат, а для будущих версий — обновление файлов в этом канале.
