# Git Training Project

Учебный репозиторий для тренировки командной работы через GitHub.

Цель: отработать процесс, который потом будет использоваться в реальном
проекте:

```text
Issue -> feature branch -> Pull Request -> Review -> merge to develop
```

## Ветки

- `main` - стабильная ветка.
- `develop` - рабочая интеграционная ветка.
- `feature/*` - ветки задач.

## Как работать над задачей

```bash
git checkout develop
git pull origin develop
git checkout -b feature/1-change-title
```

После изменений:

```bash
git add .
git commit -m "Update homepage title"
git push -u origin feature/1-change-title
```

Затем открыть Pull Request:

```text
base: develop
compare: feature/1-change-title
```

## Локальный запуск

Откройте `index.html` в браузере.
