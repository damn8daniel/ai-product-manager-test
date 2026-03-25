# AI Product Manager — Тестовое задание

## Результат
- **ExcuseAI** (Генератор отмазок): [Live Demo](https://damn8daniel.github.io/ai-product-manager-test/index.html)
- **Портфолио** (3 проекта с AI-агентами): [Live Demo](https://damn8daniel.github.io/ai-product-manager-test/portfolio.html) | [PDF](https://damn8daniel.github.io/ai-product-manager-test/portfolio.pdf)

## Инструменты
| Инструмент | Роль |
|---|---|
| **Claude Code** (CLI) | Основной AI-агент — генерация кода, архитектура, отладка |
| **Xcode 26 + Simulator** | Сборка и запуск iOS-приложений (Brushely, Skin Cancer) |
| **Puppeteer** | Автоматические скриншоты и генерация PDF |
| **React / npm** | Запуск веб-фронтенда Skin Cancer Detector |
| **GitHub Pages** | Деплой результата |

## Как ставил задачи AI-агенту

### Часть 1: ExcuseAI (Генератор отмазок)
**Задача агенту**: Создать premium dark-theme веб-сервис генерации отмазок в одном HTML файле, zero dependencies.

**Итеративный процесс**:
1. Описал концепцию → получил базовый генератор
2. Попросил добавить neural canvas фон и анимации → агент реализовал particle system
3. Запросил комбинаторный движок вместо статичного списка → 1000+ компонентов
4. Добавил AI-анализ метрик отмазок → 4 метрики + вердикт
5. Финальная полировка: typewriter-эффект, звуки, liquid glass карточки

**Результат**: один HTML файл, миллиарды комбинаций отмазок, premium UI.

### Часть 2: Портфолио
**Задача агенту**: Собрать портфолио из 3 реальных проектов с запущенными скриншотами.

**Процесс**:
1. Передал репозитории всех 3 проектов (zip-бандл)
2. Агент автоматически:
   - Собрал **Brushely** (SwiftUI) в Xcode, пофиксил 2 ошибки компиляции, запустил в iPhone 17 Pro Simulator → скриншот
   - Собрал **Skin Cancer Detector** (React Native) — скопировал на локальный диск, переустановил CocoaPods, запустил в симуляторе → скриншот
   - Извлёк результаты **YOLO11-seg** из папки results/ → скриншот сегментации
3. Вставил скриншоты в HTML-портфолио (base64)
4. Сгенерировал PDF через Puppeteer
5. Задеплоил на GitHub Pages

## Время
| Этап | Время |
|---|---|
| ExcuseAI — от идеи до финала | ~1 час |
| Портфолио — сборка проектов + скриншоты | ~30 мин |
| Портфолио — расширенная версия с метриками | ~15 мин |
| Деплой на GitHub Pages | ~5 мин |
| **Итого** | **~2 часа** |

## Автор
**Борисов Даниил** — ML Engineer, РУДН, Магистратура AI
- GitHub: [damn8daniel](https://github.com/damn8daniel)
- Telegram: [@dabriety](https://t.me/dabriety)
