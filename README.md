# BAHA RP Launcher — исходники

Android Studio project для отдельного лаунчера BAHA RP.

## Сервер
- IP: `144.124.192.40`
- Port: `7777`

## Что делает
- Показывает адрес BAHA RP.
- Кнопка «ИГРАТЬ» запускает установленный клиент `com.blackhub.bronline`.
- Если клиент не установлен, открывается его страница Google Play.

## Важно
Этот проект **не встраивает и не изменяет** оригинальный APK Black Russia. Также в проекте намеренно не заявлен автоматический deep-link на `144.124.192.40:7777`: точный Intent/URI для подключения к серверу не был подтверждён по APK.

## Сборка
Открыть папку в Android Studio и выполнить Build → Build APK(s).

Для Gradle нужен Android SDK и доступ к Google/Maven репозиториям. В текущем окружении Android SDK/Gradle не установлен, поэтому готовый APK здесь не собирался.

## Сборка с телефона
В проект уже добавлен `.github/workflows/build-apk.yml`. Он собирает debug APK на GitHub Actions, поэтому Android Studio на телефоне не нужен. Подробные шаги — в `GITHUB_BUILD.md`.
