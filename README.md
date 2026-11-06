# 🎨 NeuroHub

**Генерация изображений на своём компьютере — без подписок, облака и очередей.**
Написал промпт, нажал кнопку — картинка готова. Движок [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
работает локально на твоей видеокарте, промпты никуда не отправляются.

**ПРОМТ НУЖНО ПИСАТЬ НА АНГЛИЙСКОМ!!!**
**ПРОМТ НУЖНО ПИСАТЬ НА АНГЛИЙСКОМ!!!**
**ПРОМТ НУЖНО ПИСАТЬ НА АНГЛИЙСКОМ!!!**

[![Скачать для Windows](https://img.shields.io/badge/⬇️_Скачать-для_Windows-2ea44f?style=for-the-badge)](https://github.com/Zerphen/neurohub/releases/latest)
[![Telegram](https://img.shields.io/badge/✈️_Telegram-@NeuroHubProBot-229ED9?style=for-the-badge)](https://t.me/NeuroHubProBot)

---

## 📥 Скачать

**[Последний релиз →](https://github.com/Zerphen/neurohub/releases/latest)**

На странице релиза открой **Assets** и скачай `NeuroHub_<версия>_x64-setup.exe` (~24 МБ).
Файлы `Source code` и `latest.json` скачивать не нужно.

> Windows может показать «Неизвестный издатель» — это нормально для программы без
> платного сертификата. Нажми **«Подробнее» → «Выполнить в любом случае»**.

## ⚙️ Системные требования

| | |
|---|---|
| **Видеокарта** | NVIDIA, 8+ ГБ видеопамяти (VRAM) |
| **Оперативная память** | от 16 ГБ |
| **Диск** | от 25 ГБ свободно (лучше SSD) |
| **ОС** | Windows 10 / 11, 64 бита |

AMD и Intel Arc пока не поддерживаются: движок рассчитан на CUDA.

## ✨ Что умеет

- **Текст → картинка**: промпт, негатив, шаги, CFG, сид, сэмплер, планировщик
- **Пресеты под модель**: RealVisXL, Pony, Juggernaut, SDXL, SD 1.5 — шаги и CFG подставляются сами
- **Ручной размер** с блокировкой пропорций: от 256 до 2048 px по стороне
- **Очередь**: пакет картинок на промпт, статусы, прогресс, отмена отдельных задач
- **LoRA**: до 4 слотов с силой 0–2
- **Модели**: библиотека скачанного, каталог Hugging Face, докачка с паузой, удаление, «своя ссылка»
- **Редактирование**: img2img и inpaint с маской кистью прямо по картинке
- **Увеличить**: апскейл ×2–×4 (RealESRGAN), опционально «добавить деталей» вторым проходом
- **История**: превью, повторный сид, скачивание
- **Выгрузка модели из VRAM** и авто-выгрузка по простою
- **Автоустановка движка** из приложения: ComfyUI и базовая модель SDXL в один клик
- **Обновление по кнопке** в шапке приложения

## 🆓 Free и Pro

**Free** — бесплатно, без ограничения по времени: генерация, пресеты до Full HD,
история, автоустановка движка, выгрузка модели.

**Pro — 769 ₽, один платёж, навсегда.** Ключ привязывается к одному компьютеру
и после активации работает офлайн.

| Возможность | Free | Pro |
|---|:---:|:---:|
| Текст → картинка, негатив, шаги, CFG, сид, сэмплеры | ✓ | ✓ |
| Размер до 1920×1080 (2,07 МП) | ✓ | ✓ |
| Размер до 2048×2048 | — | ✓ |
| Пакет за запуск | 1 | до 8 |
| Очередь | до 10 задач | без лимита |
| Модели: каталог Hugging Face, докачка, удаление | — | ✓ |
| Редактирование: img2img, inpaint, маска | — | ✓ |
| Апскейл ×2–×4 и «добавить деталей» | — | ✓ |
| LoRA до 4 слотов | — | ✓ |
| Свои воркфлоу ComfyUI | — | ✓ |

Купить ключ или задать вопрос: **[@NeuroHubProBot](https://t.me/NeuroHubProBot)**

## 💾 Установка

1. Скачай установщик со [страницы релиза](https://github.com/Zerphen/neurohub/releases/latest).
2. Запусти его и открой **NeuroHub** с ярлыка на рабочем столе.
3. В левом нижнем углу нажми **«Установить движок»**. Приложение само скачает
   ComfyUI (~2 ГБ) и модель SDXL (~6,9 ГБ) в `%APPDATA%\NeuroHub`.
   Загрузку можно поставить на паузу или отменить.
4. Когда появится «Готово», напиши промпт и нажми **«Сгенерировать»**.

Python, Node.js и Stability Matrix не нужны — всё уже внутри.

## 🔑 Активация Pro

1. Открой приложение и нажми **Free** в правом верхнем углу.
2. Вставь ключ `NHUB-XXXX-XXXX-XXXX-XXXX` и нажми **«Активировать»**.

Если приложение пишет «нет связи с сервером» (обычная ситуация из РФ), активируй кодом:

1. Скопируй **HWID** в окне Pro.
2. Отправь боту: `/activate КЛЮЧ HWID`.
3. Бот пришлёт код `NH1.…` — вставь его в то же поле.

Подпись и HWID проверяются локально, поэтому после активации интернет не нужен.
Ключ действует на одном ПК; для переноса напиши боту.

## ❓ Частые вопросы

<details>
<summary><b>Нужен ли VPN?</b></summary>

Для работы приложения — нет. Интернет нужен только для скачивания движка, моделей
и первой активации. Генерация и лицензия работают офлайн.
</details>

<details>
<summary><b>Можно ли на AMD или Intel?</b></summary>

Нет. Нужна NVIDIA с CUDA и 8+ ГБ VRAM. На 8 ГБ комфортно идёт SDXL 1024×1024.
</details>

<details>
<summary><b>Сколько занимает установка?</b></summary>

Около 9 ГБ загрузок и ~25 ГБ на диске вместе с моделями. Время зависит от скорости интернета.
</details>

<details>
<summary><b>Куда сохраняются картинки и модели?</b></summary>

Картинки — `%LOCALAPPDATA%\NeuroHub\Images`, модели — `%LOCALAPPDATA%\NeuroHub\models`.
Обе папки открываются кнопками в приложении и не удаляются при обновлении.
</details>

<details>
<summary><b>Как обновляться?</b></summary>

Когда выходит новая версия, в шапке появляется кнопка **«⬆ Обновить»**.
Приложение скачает установщик, проверит SHA-256, тихо установит и перезапустится.
</details>

<details>
<summary><b>Это безопасно?</b></summary>

Приложение работает локально и слушает только `127.0.0.1`. Промпты, модели и картинки
не уходят в сеть. Единственные внешние запросы — проверка обновлений и активация ключа.
</details>

---

## 🌍 English

<details>
<summary><b>English version (click to expand)</b></summary>

### 🎨 NeuroHub

Local image generation hub powered by ComfyUI. Runs on your own NVIDIA GPU —
like LM Studio, but for images. No subscription, no cloud, no queues.

**⬇️ [Download for Windows](https://github.com/Zerphen/neurohub/releases/latest)**

### Requirements

- NVIDIA GPU with 8+ GB VRAM
- 16 GB RAM
- 25 GB free disk space (SSD recommended)
- Windows 10 / 11, 64-bit

### Features

Text-to-image with presets, batch generation and queue, LoRA (up to 4 slots),
Hugging Face model catalog with resumable downloads, img2img and inpainting,
2×–4× upscaling, generation history, one-click engine setup and app updates.

### Free vs Pro

Free includes generation up to 1920×1080, 1 image per run and a 10-job queue.
**Pro — 769 ₽ once, lifetime** — unlocks up to 2048×2048, batches of 8, unlimited
queue, Models / Edit / Upscale tabs, LoRA and custom workflows.

### Pro license

Get a lifetime key from the official Telegram bot: **[@NeuroHubProBot](https://t.me/NeuroHubProBot)**

### Install

1. Download `NeuroHub_<version>_x64-setup.exe` from [Releases](https://github.com/Zerphen/neurohub/releases/latest).
2. Run the installer. If SmartScreen appears, click **More info → Run anyway**.
3. Open NeuroHub and click **Install Engine** in the bottom-left corner (one-time setup).
4. Wait for ComfyUI and SDXL to download, then generate your first image.

### Activation

Open the app, click **Free**, paste your key and press **Activate**. If the license
server is unreachable, copy the HWID and send `/activate KEY HWID` to the bot —
it will reply with an offline activation code.

</details>
