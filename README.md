# RedLightMC Wiki — Template

Готовый шаблон вики-сайта для Minecraft-сервера **RedLightMC** (Fabric 1.21.1) на базе [MkDocs](https://www.mkdocs.org/) + [Material](https://squidfunk.github.io/mkdocs-material/).

## Быстрый старт

1. Загрузите файлы в репозиторий на GitHub
2. Подключите репозиторий к [Cloudflare Pages](https://pages.cloudflare.com/)
3. Укажите:
   - **Build command:** `pip install -r requirements.txt && mkdocs build`
   - **Output directory:** `site`
4. Добавьте домен `wiki.redlightmc.fun` в настройках Pages
5. В панели управления доменом создайте CNAME `wiki` → `имя-проекта.pages.dev`

## Структура

```
.
├── mkdocs.yml              # Конфигурация сайта и навигации
├── requirements.txt        # Зависимости
└── docs/
    ├── index.md            # Главная страница
    ├── guides/
    │   ├── start.md        # Как начать играть
    │   └── mods.md         # Моды сервера
    ├── mechanics/
    │   ├── mechanic-1.md   # Механика 1
    │   ├── mechanic-2.md   # Механика 2
    │   └── mechanic-3.md   # Механика 3
    ├── global/
    │   ├── global-mod-1.md # Глобальное изменение 1
    │   ├── global-mod-2.md # Глобальное изменение 2
    │   └── global-mod-3.md # Глобальное изменение 3
    └── roadmap/
        ├── update-1.md     # Ближайшее обновление
        ├── update-2.md     # Следующее обновление
        └── update-3.md     # Долгосрочные планы
```

## Как редактировать

1. Откройте любой `.md` файл
2. Замените текст в квадратных скобках `[ВАШ ТЕКСТ]` на свой
3. Следуйте инструкциям в HTML-комментариях `<!-- -->`
4. Сохраните изменения — Cloudflare Pages автоматически пересоберёт сайт

## Как добавить новую страницу

1. Создайте `.md` файл в нужной папке (`docs/guides/`, `docs/mechanics/` и т.д.)
2. Добавьте путь в `mkdocs.yml` в разделе `nav:`
3. Закоммитьте изменения — сайт обновится автоматически
