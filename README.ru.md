<div align="center">

<img src="logo.svg" alt="Omarchy" width="320">

# Omarchy

[English](README.md) · **Русский**

### Linux с управлением с клавиатуры.

Arch Linux · Hyprland · Инструменты оболочки

![Arch Linux](https://img.shields.io/badge/platform-Arch_Linux-7aa2f7?style=flat-square)
![Bash](https://img.shields.io/badge/tooling-Bash-9ece6a?style=flat-square)
![QML](https://img.shields.io/badge/desktop-QML-bb9af7?style=flat-square)
[![MIT](https://img.shields.io/badge/license-MIT-e0af68?style=flat-square)](LICENSE)

[Исходный проект](https://github.com/omacom/omarchy) · [Официальный сайт](https://omarchy.org) · [Руководство](#руководство-omarchy) · [Структура](#структура)

</div>

Omarchy — современный Linux-дистрибутив с собственным взглядом на рабочее окружение, созданный **David Heinemeier Hansson и участниками проекта**. Он объединяет тайловый рабочий стол, терминальные инструменты, темы и команды настройки системы.

**Это копия исходного проекта в репозитории Igor Kramar.** Она не является официальным каналом релизов и не гарантирует совпадение возможностей и выпусков с upstream. Установку и текущие требования к оборудованию смотрите на [omarchy.org](https://omarchy.org) и в [официальном репозитории](https://github.com/omacom/omarchy).

## Структура

| Каталог | Назначение |
|:---|:---|
| [`bin/`](bin/) | Команды рабочего стола и CLI |
| [`config/`](config/) · [`default/`](default/) | Конфигурация и ресурсы по умолчанию |
| [`shell/`](shell/) | Компоненты рабочего стола на QML |
| [`themes/`](themes/) | Цветовые темы |
| [`install/`](install/) · [`migrations/`](migrations/) | Установка системы и обновления |
| [`manual/`](manual/) | Пользовательское руководство |
| [`docs/`](docs/) | Устройство системы и справочные материалы |
| [`test/`](test/) | Автоматические проверки |

## Разработка

Перед изменениями прочитайте [правила работы](AGENTS.md) и [описание проверок](docs/testing.md). Существующие команды точечных проверок:

```sh
./test/cli
./test/shell
```

`./test/all` объединяет эти наборы, но не запускает графическую приёмку. Её проводят в одноразовой виртуальной машине. Установщики и миграции меняют систему: это не универсальная команда подготовки проекта к разработке.

## Руководство Omarchy

Исходник руководства находится в [`manual/`](manual/). Зеркало со скриншотами — [learn.omacom.io](https://learn.omacom.io/2/the-omarchy-manual). Названия ниже переведены для навигации; сами главы остаются на английском.


### Знакомство

- [Добро пожаловать в Omarchy!](manual/01-welcome-to-omarchy.md)

### Основы

- [Первые шаги](manual/02-getting-started.md)
- [Переход с macOS или Windows](manual/03-coming-from-mac-or-windows.md)
- [Навигация](manual/04-navigation.md)
- [Верхняя панель](manual/05-the-top-bar.md)
- [Темы](manual/06-themes.md)
- [Горячие клавиши](manual/07-hotkeys.md)
- [Общий буфер обмена и история](manual/08-unified-clipboard-history.md)
- [Напоминания](manual/09-reminders.md)
- [Уведомления](manual/10-notices.md)
- [Распознавание текста и диктовка](manual/11-text-extraction-dictation.md)
- [Снимки и запись экрана](manual/12-screenshots-recording.md)
- [Переключатели, бездействие и заставка](manual/13-toggles-idle-screensaver.md)
- [Командная строка Omarchy](manual/14-omarchy-cli.md)

### Приложения

- [Терминал](manual/15-terminal.md)
- [Neovim](manual/16-neovim.md)
- [Инструменты ИИ](manual/17-ai.md)
- [Средства разработки](manual/18-development-tools.md)
- [Инструменты оболочки](manual/19-shell-tools.md)
- [Функции оболочки](manual/20-shell-functions.md)
- [Терминальные интерфейсы](manual/21-tuis.md)
- [Графические приложения](manual/22-guis.md)
- [Браузеры](manual/23-browsers.md)
- [Коммерческие приложения и сервисы](manual/24-commercial-apps-services.md)
- [Веб-приложения](manual/25-web-apps.md)
- [Игры](manual/26-gaming.md)
- [Заполнение PDF](manual/27-filling-out-pdfs.md)
- [Виртуальная машина Windows](manual/28-windows-vm.md)
- [Другие пакеты](manual/29-other-packages.md)

### Настройка

- [Обновления](manual/30-updates.md)
- [Конфигурационные файлы](manual/31-dotfiles.md)
- [Плагины оболочки](manual/32-shell-plugins.md)
- [Мониторы](manual/33-monitors.md)
- [Клавиатура, мышь и трекпад](manual/34-keyboard-mouse-trackpad.md)
- [Сеть](manual/35-networking.md)
- [Сон системы](manual/36-system-sleep.md)
- [Аппаратная аутентификация](manual/37-hardware-authentication.md)
- [Шрифты](manual/38-fonts.md)
- [Фоны](manual/39-backgrounds.md)
- [Приглашение оболочки](manual/40-prompt.md)
- [Оформление](manual/41-branding.md)
- [Частые настройки](manual/42-common-tweaks.md)
- [Создание темы](manual/43-making-your-own-theme.md)

### Дополнительно

- [Поддержка Mac](manual/44-mac-support.md)
- [Решение проблем](manual/45-troubleshooting.md)
- [Частые вопросы](manual/46-faq.md)
- [Снимки системы](manual/47-system-snapshots.md)
- [Безопасность](manual/48-security.md)
- [Omarchy на разных устройствах](manual/49-omarchy-on.md)
- [Установка с двойной загрузкой](manual/50-dual-boot-install.md)
- [Автоматическая установка](manual/51-unattended-installs.md)

## Лицензия и авторство

[MIT](LICENSE) с сохранённым исходным уведомлением об авторских правах David Heinemeier Hansson. Авторство upstream и уведомления для сторонних ресурсов сохраняются. Локальную витрину репозитория поддерживает Igor Kramar.
