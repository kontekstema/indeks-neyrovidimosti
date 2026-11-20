# Индекс контекстемы: открытые данные

Институт нейрокоммуникаций «Контекстема» проверяет, что нейросети говорят о компаниях, когда покупатель спрашивает у них совета. Мы задаем Алисе, GigaChat, ChatGPT и другим нейросетям вопросы покупателей и разбираем каждый ответ, где названа компания. Здесь лежат данные этих замеров и ссылки на методику.

## Что меряет индекс

Одно высказывание нейросети о компании мы называем контекстемой и проверяем по четырем вопросам:

| Вопрос | Что смотрим |
|---|---|
| За что назвали | на какой вопрос покупателя нейросеть ответила этой компанией |
| С кем рядом | в какой категории и рядом с какими конкурентами она стоит |
| Советуют ли | компанию рекомендуют, просто перечисляют или от нее предостерегают |
| Верно ли пересказали | совпадают ли факты в ответе с тем, что есть на самом деле |

Название в ответе отвечает только на первый вопрос. Остальные три показывают, что покупатель узнает о компании из ответа.

Полная методика: [doi.org/10.5281/zenodo.23499257](https://doi.org/10.5281/zenodo.23499257). Панель нейросетей и порядок сбора: [kontekstema.ru/metodika-paneli](https://kontekstema.ru/metodika-paneli).

## Данные

| Файл | Что внутри |
|---|---|
| `data/reyting-bankov-2026-10.csv` | рейтинг банков, октябрь 2026: 2 415 оценок высказываний о банках из 11 источников: 9 нейросетей, у Алисы и Google по два режима (Алиса в поиске и в чате, обзор от ИИ и режим ИИ в Google); по каждому ответу нейросеть, вопрос, банк, роль, полка, верность фактам, балл и место банка в рейтинге |

Файл в кодировке UTF-8, разделитель точка с запятой, десятичная запятая.

## Рейтинги на сайте

| Рейтинг | Страница |
|---|---|
| Банки | [kontekstema.ru/reyting-bankov](https://kontekstema.ru/reyting-bankov) |
| Аптеки | [kontekstema.ru/reyting-aptek](https://kontekstema.ru/reyting-aptek) |
| Туроператоры | [kontekstema.ru/reyting-turoperatorov](https://kontekstema.ru/reyting-turoperatorov) |
| Застройщики | [kontekstema.ru/reyting-zastrojshchikov](https://kontekstema.ru/reyting-zastrojshchikov) |

Место в рейтинге не продается.

## Лицензия

Данные открыты по лицензии CC BY 4.0: их можно брать в любых целях, в том числе коммерческих, со ссылкой на «Контекстему» как источник. Методика на Zenodo опубликована под своей лицензией CC BY-NC-ND 4.0. Подробно в файле `LICENSE`.

## Как сослаться

Данные: «Индекс контекстемы, Институт нейрокоммуникаций «Контекстема», kontekstema.ru». Методика: Руцинская Д., Макрушенко И. Методика индекса контекстемы. Zenodo, 2026. DOI 10.5281/zenodo.23499257. Готовая ссылка лежит в `CITATION.cff`.

## About (English)

Kontekstema Institute of Neurocommunications measures how AI assistants (Alice, GigaChat, ChatGPT, Claude, Gemini, Perplexity, DeepSeek, Qwen) describe companies when users ask for advice. Each statement about a company is scored on four questions: why the company was named, which competitors it is placed with, whether it is recommended, and whether the facts are correct. This repository holds open data from our industry ratings, licensed under CC BY 4.0. Methodology: DOI 10.5281/zenodo.23499257. Website: [kontekstema.ru](https://kontekstema.ru).

Контакты: hello@kontekstema.ru
