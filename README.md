# <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Linux-Dark.svg" width="38" height="38" valign="middle"/> BrabusOS Desktop (Pasito Linux Edition)

<p align="left">
  <img src="https://img.shields.io/badge/Ubuntu-24.04_LTS-E95420?logo=ubuntu&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/Kernel-Linux_6.x-FCC624?logo=linux&logoColor=black&style=flat-square" />
  <img src="https://img.shields.io/badge/Browser-Chromium-4285F4?logo=google-chrome&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/Build-GitHub_Actions-2088FF?logo=github-actions&logoColor=white&style=flat-square" />
  <img src="https://img.shields.io/badge/Hardware-Smoant_Pasito_3-300A24?style=flat-square" />
</p>
---

## <img src="https://api.iconify.design/octicon:info-16.svg?color=%23E95420" width="20" height="20" valign="middle"/> Описание проекта

**BrabusOS Desktop (Pasito Linux Edition)** — специализированный легковесный дистрибутив Linux формата LiveCD, построенный на пакетной базе Ubuntu 24.04 LTS (Noble Numbat). Система разработана как готовая программная среда, сочетающая полноценный стек классической операционной системы и тематический интерфейс управления электроникой в стиле линейки устройств Smoant Pasito.

Образ функционирует в оперативной памяти без необходимости установки на накопитель, предоставляя доступ к графическому окружению, веб-браузеру Chromium и системным утилитам прямо из коробки.

---

## <img src="https://api.iconify.design/octicon:checklist-16.svg?color=%23E95420" width="20" height="20" valign="middle"/> Назначение и концепция

* <img src="https://api.iconify.design/octicon:zap-16.svg?color=%23E95420" width="16" height="16" valign="middle"/> **Автономная работа:** загрузка в режиме LiveCD без перезаписи локальных дисков компьютера или виртуальной машины.
* <img src="https://api.iconify.design/octicon:cpu-16.svg?color=%23E95420" width="16" height="16" valign="middle"/> **Полноценный системный стек:** система опирается на официальное ядро Linux 6.x и стандартную библиотеку GNU C, обеспечивая совместимость с x86-64 оборудованием.
* <img src="https://api.iconify.design/octicon:globe-16.svg?color=%23E95420" width="16" height="16" valign="middle"/> **Предустановленный софт:** встроенный Chromium для веб-серфинга, терминал для администрирования через Bash и панель управления параметрами Ant-Chip.
* <img src="https://api.iconify.design/octicon:paintbrush-16.svg?color=%23E95420" width="16" height="16" valign="middle"/> **Кастомный стиль:** графическое окружение Openbox и панель Tint2 стилизованы под баклажаново-оранжевую палитру Ubuntu Yaru и бренд Brabus.

---

## <img src="https://api.iconify.design/octicon:tools-16.svg?color=%23E95420" width="20" height="20" valign="middle"/> Ключевые компоненты

| Иконка | Компонент | Назначение |
| :---: | :--- | :--- |
| <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Ubuntu-Dark.svg" width="24" height="24"/> | **Ubuntu 24.04 RootFS** | Минимальная базовая файловая система, собранная через утилиту `debootstrap` |
| <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Linux-Dark.svg" width="24" height="24"/> | **Linux Image Generic** | Официальное модульное ядро с поддержкой файловых систем, USB и сетевых интерфейсов |
| <img src="https://api.iconify.design/octicon:screen-full-16.svg?color=%23E95420" width="24" height="24"/> | **X.Org + Openbox** | Оконная система и оконный менеджер с низким потреблением оперативной памяти |
| <img src="https://api.iconify.design/logos:chrome.svg" width="24" height="24"/> | **Chromium Browser** | Настольный веб-браузер с поддержкой JavaScript, аппаратного рендеринга и сети |
| <img src="https://api.iconify.design/octicon:rss-16.svg?color=%23E95420" width="24" height="24"/> | **NetworkManager** | Служба автоматической настройки проводных и беспроводных сетевых подключений |
| <img src="https://api.iconify.design/octicon:terminal-16.svg?color=%23E95420" width="24" height="24"/> | **Systemd Live-Init** | Управление службами и автоматический беспарольный вход в графическую сессию |

---

## <img src="https://api.iconify.design/octicon:file-directory-16.svg?color=%23E95420" width="20" height="20" valign="middle"/> Структура репозитория

```text
.
├── README.md
└── .github/
    └── workflows/
        └── build-distro.yml
