# Traffic Rider



**Traffic Rider** — это прототип бесконечного раннера на Unity, где игрок управляет транспортом, уворачиваясь от препятствий и соперников. Проект включает:

- Главное меню с четырьмя кнопками: **START**, **SETTINGS**, **CONTROLS**, **EXIT**.
- Режим игры с бесконечными секциями дороги, ИИ‑соперниками и подсчётом пройденного расстояния.
- Возможность перезапуска по нажатию **R**.

## Features

- **Main Menu**
  - **START**: запускает игровую сцену.
  - **SETTINGS**: регулировка громкости (Slider) и разрешения экрана (Dropdown).
  - **CONTROLS**: справка по управлению.
  - **EXIT**: выход из приложения.
- **Gameplay**
  - Бесконечный трек, генерируется из пула секций.
  - ИИ-машины (AICarSpawner) для динамики на дороге.
  - Подсчёт и отображение пройденного расстояния.
  - При столкновении — эффект взрыва и плавное замедление времени.

## Requirements

- Unity **2021.3 LTS** или выше
- Пакеты:
  - Universal Render Pipeline (URP)
  - TextMeshPro

## Installing

- [Перейти по ссылке на Google Drive](https://drive.google.com/drive/folders/1UkPMkOczgJ95-2VYfb8H2phSaDUP9dz6?usp=sharing)
- Скачать архив
- в папке builds запустить файл "TrafficRider_eschkereeee"
- Удачи!

## Открытие проекта

  Запустите Unity Hub и выберите загруженную папку.

  Убедитесь, что установлены все нужные пакеты (URP, TextMeshPro).

## Build Settings

File → Build Settings.

Добавьте MainMenu.unity (индекс 0) и игровую сцену.

Убедитесь, что MainMenu стоит первой.

## Использование

В редакторе нажмите ▶ Play, чтобы увидеть Main Menu.

В билде приложение сразу стартует с Main Menu.

Нажмите START для игры, EXIT для выхода.

В игре: дистанция отображается в левом верхнем углу.

При столкновении перезапустите игру на R.

## Детали реализации

- UI
    - UIHandler: обновляет дистанцию, рекорд, показывает Game Over.

    - MainMenuManager: управление кнопками меню.

    - SettingsManager: связывает Slider громкости и TMP_Dropdown разрешений.

    - ButtonHoverAnim: анимация кнопок.

- Gameplay Scripts
    - EndlessLevelHandler, TransportHandler, ExplodeHandler, AICarSpawner, AIHandler







