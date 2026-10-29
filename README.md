<p align="center">
  <img src="assets/icon.png" width="128" alt="Opal">
</p>

<h1 align="center">Opal</h1>

<p align="center">
  Офлайн-ежедневник и учёт рабочего времени в одном HTML-файле.<br>
  Offline diary and work-hours tracker in a single HTML file.
</p>

<p align="center">
  <a href="https://github.com/Finn013/Opal/releases/latest"><b>⬇️ Скачать / Download</b></a>
  &nbsp;·&nbsp;
  <a href="#русский">🇷🇺 Русский</a>
  &nbsp;·&nbsp;
  <a href="#english">🇬🇧 English</a>
</p>

---

<a id="русский"></a>
# 🇷🇺 Русский

## Что такое Opal

Opal — это личный ежедневник и табель рабочих часов, который целиком помещается в один файл `Opal.html`. Откройте его в любом браузере на компьютере или телефоне, и он сразу работает, даже без интернета. Без установки, без серверов, без регистрации: все записи хранятся локально в браузере, а при желании синхронизируются между устройствами через ваш собственный репозиторий GitHub.

## Для кого

Opal идеально подходит тем, кто работает каждый месяц и **сам считает свои рабочие часы**: записываете, сколько трудились каждый день, а в конце месяца точно знаете, сколько отработали, и можете сразу об этом сказать. Если в месяце остался **запас или недобор времени, он переносится на следующий месяц**, так что ни один час не теряется.

## Возможности

### 📅 Календарь и записи
- Просмотр по году, месяцу и дню, быстрый переход к «Сегодня».
- Записи на каждый день: открывайте день в отдельном окне и добавляйте строки.
- Карточки с итогами по месяцу.

### ⏱ Учёт рабочего времени
- Два режима ввода: «Часы / минуты» или диапазон «От → До» (кнопка «Сейчас» подставляет текущее время).
- Норма часов в месяц: общая по умолчанию или своя для конкретного месяца.
- Итоги по неделям и за месяц, отработанные дни.
- Перенос остатка (запаса или недобора времени) на следующий месяц — автоматически или вручную.
- Отметка «Оплачено».

### 🎨 Оформление
- Набор тёмных и светлых тем, плюс свои темы.
- Ручная настройка цветов.
- Фоновое изображение с регулируемой прозрачностью.
- Размер интерфейса: маленький, средний, большой.

### 🔒 Безопасность
- Защита входа PIN-кодом или паролем.
- Автоблокировка при сворачивании приложения.
- **Шифрование файла синхронизации** паролем (AES): в репозитории лежит только зашифрованный файл, который без пароля прочитать нельзя. Это заметно повышает безопасность ваших данных. Пароль восстановить нельзя — запомните его.

### 💾 Данные
- Экспорт и импорт в файл JSON.
- Копирование и вставка данных в виде JSON.

## ☁️ Синхронизация через GitHub

Opal хранит данные в JSON-файле в вашем репозитории GitHub и синхронизирует их между всеми устройствами. Записи объединяются построчно, поэтому правки, сделанные в один и тот же день на разных устройствах, не теряются. Если данные расходятся, Opal покажет конфликт и предложит, что оставить.

**Как настроить:**
1. Создайте на GitHub **приватный** репозиторий для данных.
2. Откройте GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** и создайте токен с доступом **только к этому репозиторию** и правом **Contents: Read and write**.
3. В Opal откройте **Настройки → Синхронизация GitHub**, включите синхронизацию и укажите:
   - токен доступа;
   - репозиторий (`owner/repo` или ссылку);
   - ветку (пусто — основная);
   - имя файла.
4. Нажмите **«Проверить»**, затем **«Синхронизировать»**.
5. Рекомендуем включить **шифрование** и задать пароль — тогда файл синхронизации будет защищён.

### 📚 Несколько ежедневников в одном репозитории
Можно вести сразу несколько ежедневников: просто укажите для каждого **своё имя файла синхронизации** (например, `work.json`, `personal.json`). Каждый файл — отдельная синхронизация со своей информацией, при этом все они хранятся в **одном и том же репозитории**.

## 📦 Установка

| Платформа | Как запустить | Статус |
|---|---|---|
| Любой браузер | Скачайте `Opal.html` из [Releases](https://github.com/Finn013/Opal/releases) и откройте | ✅ Доступно |
| Android 7+ | Скачайте `Opal.apk` из [Releases](https://github.com/Finn013/Opal/releases) и установите | ✅ Доступно |
| Windows | `Opal-Setup.exe` — установщик, `Opal-Portable.exe` — без установки, данные рядом с файлом | ✅ Доступно |

## 💬 Идеи и отзывы

Opal изначально написан для личных нужд — как удобный инструмент для себя. Поэтому мне особенно интересно мнение других: что неудобно, чего не хватает, что можно улучшить или добавить. Делитесь, даже если это небольшая мелочь!

- 💡 Предложить идею или обсудить: [Discussions](https://github.com/Finn013/Opal/discussions)
- ✨ Новая идея сразу: [создать обсуждение](https://github.com/Finn013/Opal/discussions/new/choose)
- 🐞 Сообщить об ошибке: [создать Issue](https://github.com/Finn013/Opal/issues/new)
- 📋 Все сообщения об ошибках: [Issues](https://github.com/Finn013/Opal/issues)

Каждое предложение читается, лучшие идеи попадут в следующие версии.

---

<a id="english"></a>
# 🇬🇧 English

## What is Opal

Opal is a personal diary and work-hours log that fits entirely into a single `Opal.html` file. Open it in any browser on your computer or phone and it just works, even offline. No installation, no servers, no sign-up: all entries are stored locally in your browser and can optionally sync between devices through your own GitHub repository.

## Who it's for

Opal is ideal for anyone who works every month and **tracks their own working hours**: log how long you worked each day, and at the end of the month you know exactly how many hours you put in and can report them right away. Any **surplus or shortfall of time carries over to the next month**, so no hour gets lost.

## Features

### 📅 Calendar and entries
- Year, month and day views, with a quick jump to "Today".
- Entries for every day: open a day in its own window and add lines.
- Cards with monthly totals.

### ⏱ Work-hours tracking
- Two input modes: "Hours / minutes" or a "From → To" range (the "Now" button fills in the current time).
- Monthly hours target: a default one or a custom one per month.
- Weekly and monthly totals, days worked.
- Carry-over of the remaining balance (surplus or shortfall) to the next month, automatically or manually.
- "Paid" mark.

### 🎨 Appearance
- Dark and light themes, plus your own themes.
- Manual color customization.
- Background image with adjustable transparency.
- Interface size: small, medium, large.

### 🔒 Security
- Sign-in protection with a PIN or password.
- Auto-lock when the app is minimized.
- **Encryption of the sync file** with a password (AES): the repository holds only an encrypted file that cannot be read without the password, which significantly improves the security of your data. The password cannot be recovered, so keep it safe.

### 💾 Data
- JSON export and import.
- Copy and paste your data as JSON.

## ☁️ GitHub sync

Opal stores your data in a JSON file in your GitHub repository and syncs it across all your devices. Entries are merged line by line, so edits made on the same day on different devices are never lost. If the data diverges, Opal shows the conflict and lets you choose what to keep.

**Setup:**
1. Create a **private** GitHub repository for your data.
2. Go to GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** and create a token with access **to this repository only** and the **Contents: Read and write** permission.
3. In Opal, open **Settings → GitHub sync**, enable sync and enter:
   - the access token;
   - the repository (`owner/repo` or a link);
   - the branch (empty = default);
   - the file name.
4. Tap **"Check"**, then **"Sync"**.
5. We recommend enabling **encryption** and setting a password to protect your sync file.

### 📚 Several diaries in one repository
You can keep several diaries at once: just give each one **its own sync file name** (for example, `work.json`, `personal.json`). Each file is a separate sync with its own data, while all of them live in **the same repository**.

## 📦 Installation

| Platform | How to run | Status |
|---|---|---|
| Any browser | Download `Opal.html` from [Releases](https://github.com/Finn013/Opal/releases) and open it | ✅ Available |
| Android 7+ | Download `Opal.apk` from [Releases](https://github.com/Finn013/Opal/releases) and install it | ✅ Available |
| Windows | `Opal-Setup.exe` — installer, `Opal-Portable.exe` — no install, data kept next to the file | ✅ Available |

> The app interface is currently in Russian.

## 💬 Ideas and feedback

Opal was originally written for personal use, as a handy tool for myself. That's exactly why other people's opinions matter so much: what's inconvenient, what's missing, what could be improved or added. Share your thoughts, even small ones!

- 💡 Suggest an idea or discuss: [Discussions](https://github.com/Finn013/Opal/discussions)
- ✨ New idea right away: [start a discussion](https://github.com/Finn013/Opal/discussions/new/choose)
- 🐞 Report a bug: [open an Issue](https://github.com/Finn013/Opal/issues/new)
- 📋 All bug reports: [Issues](https://github.com/Finn013/Opal/issues)

Every suggestion is read, and the best ideas will make it into future versions.
