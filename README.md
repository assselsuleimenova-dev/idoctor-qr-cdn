# idoctor-qr-cdn

CDN-папка для QR-картинок тейблтентов клиник. PNG'и в `qr/<slug>.png`, сервятся через `https://raw.githubusercontent.com/assselsuleimenova-dev/idoctor-qr-cdn/main/qr/<slug>.png`.

Зачем: Canva MCP `upload-asset-from-url` двойным-percent-encode-ит query-string при fetch, поэтому `api.qrserver.com?data=...` ломается. Локальный QR + raw GitHub URL без query — clean fetch.

Регенерируется автоматически из `table-tents-bot` pipeline.
