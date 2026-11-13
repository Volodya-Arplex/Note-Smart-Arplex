# Note Smart Arplex v3 — сборка APK через GitHub

## Что делать — 3 действия, без кода

1. Создай репозиторий на github.com, назови `note-smart-arplex`, Public, с README.
2. Нажми Add file -> Upload files -> перетащи СЮДА ВСЕ файлы из этого архива, ВКЛЮЧАЯ папку `.github` (важно: папка .github должна попасть в репозиторий, иначе сборка не запустится).
   - Если GitHub не показывает скрытую папку .github при перетаскивании — залей её отдельно: Add file -> Create new file -> в имени напиши `.github/workflows/build-apk.yml` и вставь содержимое этого файла из архива.
3. Зайди во вкладку Actions -> Build APK -> Run workflow -> жди зеленую галочку -> внизу скачай Artifacts -> Note-Smart-Arplex-v3 -> внутри app-debug.apk

## Что внутри
- index.html — всё приложение
- manifest.json — PWA
- package.json — зависимости Capacitor 6.2.2 (зафиксированные версии, без ошибок)
- capacitor.config.json — appId com.arplex.notesmart
- .github/workflows/build-apk.yml — автоматическая сборка
