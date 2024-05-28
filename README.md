Провел анализ ключевых показателей игры "Баскетбол" в лиге NBA в динамике с 1947 года по 2023 год (данные взяты с kaggle).

С высоты птичьего полета можно сказать, что атакующие навыки до сих продолжают совершенствоваться и мы видим восходящую динамику ключевых показателей в атаке. Растет доля трехочковых бросков с дальней дистанции и уменьшается доля мячей забитых со средней дистанции, растет процент попаданий трехочковых бросков (3P%) и бросков с штрафной линии (FT%), увеличивается общая результативность матчей (FG). 
Видно, что в раннем периоде командами очень мало внимания уделялось защитным навыкам, поэтому в 1947-1990 гг. по показателям защиты наблюдался колоссальный рост. Навыки активно развивались - блокировки бросков (BLK), перехваты (SLT), подборы (DRB). Пик защитных показателей приходится на 1986-1992 гг. 
В связи с этим, нападающим становится все сложнее и сложнее забивать со средней и короткой дистанции, и они были вынуждены уйти за трехочковую линию. Мы видим как в 1986-1992 гг. начинает расти доля и точность бросков с дальней дистанции.

Резюме. Защитники прокачались по максимуму. Теперь прокачиваются нападающие, причем уже на атаку с дистанции. Защитники плавно начинают деградировать, потому что работы для них все меньше и меньше. 🙂 

Очень интересно каким будет следующий этап эволюции игры.

PS. Комментарий к одному странному месту на графике.

При анализе динамики доли 1-2-3 очковых бросков в общем результате матча, я увидел одно очень неприятное место на графике, вернее даже два, зеркальных друг к другу (выделено синими кружками).

Предыстория. После введения в 1980 году 3-очковых бросков, их доля неуклонно растет, а доля 2-очковых бросков снижается. Все логично и объяснимо.

Но, потом происходит что-то очень странное. 3 года - 1995-1996-1997 год - резкое увеличение доли трехочковых бросков. А потом, как ни в чем ни бывало, все возвращается обратно. Как будто бы кто-то разорвал наш бумажный график, а когда склеивал, делал это не очень аккуратно, и пару линий сместилось. Но мы же аналитики! Мы  прямо видим их место на кривой! Вон же оно!

Тем не менее, накидываем гипотезы: 
Почему все игроки резко стали забивать больше с трехочковой линии и меньше со средней дистанции?
Стали давать больше очков, может еще какие бонусы?
Уменьшили размер мяча?
Увеличили диаметр корзины?
Мячи с самонаведением?
Ввели какую-то непроходимую линию обороны и теперь к кольцу не пройдешь?
А что через 3 года? Вернули обратно? Отменили? Бред.
И тут любого аналитика данных посещает свежая мысль - Точно! Ошибка в данных! И, так как у нас целых 3 года, то на случайную ошибку не похоже, скорее систематическая, и как будто бы просто со смещением.

И в этом самом месте возникает желание найти ту самую “чертову ошибку” и соединить эти три точки плавной линией, ведь так оно и “должно быть”. И будет красиво!

Поехали. Сначала проверяем датасет на задвоенные значения, потом выборочно на корректность данных, сравнивая с двумя-тремя внешними источниками…совпадает ли количество игр, результаты конкретных игр и т.д. Потрачен час. Убедились, что данные корректны.
На всякий случай, решил посмотреть в свой же дашборд на другой график - график точности трехочковых бросков. И там тоже есть пик в 1995-1996-1997 гг. 
В эти годы резко увеличилась точность дальних бросков! 
То есть у нас не просто увеличилось количество попыток бросков с дальней дистанции и из-за этого увеличилась их доля, а резко выросла точность попаданий! 
“Ну точно самонаведение!”, - подумал я и ушел гуглить….

Ищу данные об изменении размера мяча, диаметра корзины в NBA, самонаводящиеся мячи. Ничего нет. Что только не искал…а помог мне простой запрос “как меняли правила в NBA трехочковые броски”. Он выдал мне статью про эволюцию трехочковых бросков.

Готовы?

В середине 90-х комиссар НБА Дэвид Стерн и руководство Лиги не на шутку забеспокоилось относительно уменьшения результативности матчей и, как следствие, были риски снижения популярности чемпионата. Перед началом сезона 1994-1995, с целью повышения привлекательности матчей и увеличения рейтингов ТВ-трансляций, приняло решение укоротить трехочковую линию на 38 см! Бинго!

Стоп! А через три года что? Отменили?

Да. Через 3 года просто отменили и вернули трехочковую линию на старое место. (Видимо, риски снижения популярности NBA исчезли.)
И показатели точности и доли тоже вернулись на “свои” места. 

А ведь соблазн исправить руками ошибку и “сделать красиво” был о-очень большой...