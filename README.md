### Alice
#### Конкурс «Alice» - идентификация пользователя в Интернете по последовательности переходов по сайтам.
#### Описание
В этом конкурсе нужно определить конкретного пользователя сети Интернет по сессии посещения веб-сайтов. В каждой сессии может быть от 1 до 10 сайтов – количество сайтов ограничено длиной сессии. Почему конкурс называется «Alice»?

Во-первых, так назвали конкурс его создатели. Да, конкурс уже достаточно давно используется в курсе mlcourse.ai его создателем Юрой Кашницким @Yorko. Он любезно предоставил данные для перезапуска конкурса на платформе ODS, чтобы курсы, такие как «Линейные модели» и «Открытый курс машинного обучения», могли переиспользовать конкурс. 

Во-вторых, Alice – это «обычное имя», например, в криптографии говорят Alice вместо «Пользователь А» и Bob вместо «Пользователь Б». Все равно как мы назовем пользователя, которого мы ищем, или «target = 1», поэтому давайте именно его, вернее, её назовём Alice. Будем искать Alice!

Данные для конкурса собраны с прокси-серверов Университета Блеза Паскаля и взяты из статьи, которая описывает методы поиска Alice. Если хочется посмотреть на все научные подходы к решению, есть книга. Современные материалы ищите в сети по словам "Traversal Pattern Mining" и "Sequential Pattern Mining".

А мы будем решать задачу методами машинного обучения как задачу классификации.

#### Постановка задачи 
Для каждой сессии нужно предсказать, принадлежит ли сессия Alice (метка «1»), или нет (метка «0»).

#### Метрика оценки решений
Целевая метрика – ROC AUC.
