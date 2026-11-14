# SHIPUCHKA CLIENT — Launcher App

Исходный проект Windows-лаунчера SHIPUCHKA CLIENT.

## Сборка установщика

1. Добавьте в корень репозитория файлы и папки исходного проекта: `src/`, `client/`, `build-exe.bat`, `build.bat`, и ресурсы (иконки), если они есть.
2. В GitHub откройте **Actions** → **Build SHIPUCHKA Windows installer** → **Run workflow**.
3. После успешной сборки скачайте artifact `SHIPUCHKA-Setup-Windows-x64`.

Для сборки требуется Java 21 и WiX Toolset 3. Установщик создаётся через `jpackage`; он устанавливает лаунчер с включённой Java-средой. Игровые файлы Minecraft/Fabric загружаются самим лаунчером при установке клиента.

## Важно

Не добавляйте GitHub Personal Access Tokens, пароли или другие секреты в репозиторий. Этот репозиторий предназначен для приложения-лаунчера, а не для метаданных обновлений.
