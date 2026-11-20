# Индекс контекстемы: открытые данные

Институт нейрокоммуникаций «Контекстема» изучает, как нейросети пересказывают людям мир: компании, людей, новости, историю и классику. Мы меряем это открытыми методиками, ведем индекс контекстемы и Словарь Контекстемы, выпускаем исследования и рейтинги отраслей и учим людей и компании говорить так, чтобы нейросеть передала их смысл точно. Методики и данные замеров выкладываем в открытый доступ, чтобы исследователь мог проверить и повторить результат.

В этом репозитории лежат данные замеров по рейтингам отраслей: мы задаем нейросетям вопросы покупателей и разбираем каждый ответ, где названа компания.

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
| `data/reyting-turoperatorov-2026-10.csv` | рейтинг туроператоров, октябрь 2026: 45 вопросов о туре на Новый год, 491 ответ, 3 190 упоминаний туроператоров, турагентств и сервисов продажи туров; место для 30 компаний рейтинга |
| `data/reyting-zastrojshchikov-2026-11.csv` | рейтинг застройщиков, ноябрь 2026: 45 вопросов человека, который выбирает квартиру в новостройке, 495 ответов, 4 247 упоминаний застройщиков жилья; место для 31 застройщика рейтинга |

Файлы в кодировке UTF-8, разделитель точка с запятой, десятичная запятая. Одна строка = одно упоминание компании в первом ответе нейросети; балл = роль × полка × верность фактам. Ответы, где компания не названа, строк не дают, но входят в расчет индекса с нулем. Колонка «тревожная оговорка» в таблицах туроператоров и застройщиков принимает три значения: «да» (отметили оба разметчика), «у одного разметчика» (в доле тревожных упоминаний считается за половину) и «нет»; в таблице банков «да» стоит, если оговорку отметил хотя бы один разметчик.

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

Kontekstema Institute of Neurocommunications studies how AI retells the world to people: companies, people, news, history and classics. We measure this with open methods, maintain the Kontekstema Index and the Kontekstema Dictionary, publish research and industry ratings, and teach people and companies to communicate so that AI conveys their meaning accurately. For the ratings we ask AI (Alice, GigaChat, ChatGPT, Claude, Gemini, Perplexity, DeepSeek, Qwen) buyers' questions and score every answer that names a company. Each statement about a company is scored on four questions: why the company was named, which competitors it is placed with, whether it is recommended, and whether the facts are correct. This repository holds open data from our industry ratings, licensed under CC BY 4.0. Methodology: DOI 10.5281/zenodo.23499257. Website: [kontekstema.ru](https://kontekstema.ru).

Контакты: hello@kontekstema.ru
