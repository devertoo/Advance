## Вывод

**Причины неэффективности привлечения пользователей следующие:**  
- Пользователи США перестали окупаться в тот момент, когда САС резко подскочил вверх. Эффекта реклама не произвела, а вот ROI из-за этого резко пошел вниз.  
- Мало внимания уделяется владельцам ПК - они удерживаются лучше других, и единственные из всех устройств окупаются к концу второй недели.  
- Удержание платящих пользователей из США оказалось хуже остальных.  
- Пользователи,пришедшие из каналов Типтоп и Фэйсбум не окупились по причине больших затрат на рекламу
- Пользователи из канала Фесбум и AdNoneSense удерживаются хуже других  

**Рекомендации для отдела маркетинга:**
- Владельцы ПК удерживаются лучше всего, и единственные из всех устройств окупаются к концу второй недели -стоит обратить на них внимание  
- Так же стоит обратить внимание на привлечение пользователей, использующих Андроид.
- Уменьшить затраты на маркетинг в СШАПривлекать больше пользователей с каналов Лямбда. 
- Уменьшить траты на рекламу в канале Фейсбум и AdNoneSense

## Задача

Необходимо выяснить, почему, несмотря на огромные вложения в рекламу, последние несколько месяцев компания терпит убытки, разобраться в причинах и помочь компании выйти в плюс.

## Ход исследования
### Обзор и предобработка данных

**Вывод:** 
Таблица cost имеет 1800 строк и содержит следующую информацию:  
- dt — дата проведения рекламной кампании,
- channel — идентификатор рекламного источника,
- costs — расходы на эту кампанию.  

Видим большой разброс по затратам на рекламные кампании. Средннее значение от медианы отличается на 46 долларов. Стандартное отклонение равно 107,7. Минимальная рекламная кампания обошлась в 0.8 долларов, а максимальная в 630. Болле 75% всех рекламных кампаний приходятся на суммму до 34 долларов.

### Исследовательский анализ данных (EDA)

**Вывод:**  
Из всех пользователей приложения, бОльшую часть составляют "Органические"- почти 37%. Также большая доля пользователей привлечены через каналы Фэйсбум и Типтоп- 19% и 13%. Оставшиеся 30% пользователей привлечены сумарно из 8 каналов привлечения, доля каждого из которых не превышает 5,7% от общего числа пользователей.
Что касается пользователей, имеющих статус "платящих", то тут безусловное лидерство занимают пользователи, привлечённые из канала Типтоп. Их доля составляет 40% от общего числа платящих пользователей. Второе место среди "платящих" занимают пользователи, перешедшие их канала Типтоп- 21%. Доля "органики" - 13%. Оставшиеся 8 каналов сумарно составляют 26%, доля каждого из которыз не превышает 5%.
Если смотреть процент перехода из "неплатящих" в "платящих" по каждому каналу, то тут картина заметно меняется: чаще всего готовы соверщать покупки пользователи из Фэйсбум, AdNonSense, lammbdaMediaAds, Типтоп, RocketSuper- процент совершенных покупок у них от 8 до 12%.

### Анализ затрат на маркетинг

**Вывод:**  
Вывод: Видим что дороже всего обходится привлечение пользователей из канала Типтоп, и это неудивительно, ведь около половины бюджета на рекламу приходится на этот канал. Пользователи из канала Фэйсбум и AdNoneSense обходятся в среднем в 1$.
Предварительно, могу сказать, что траты на маркетинг в канале Типтоп, необосновано высоки.


### Оценим окупаемость рекламы (LTV, CAC и ROI)

**Вывод:**
Судя по всему, ответ на наш вопрос: в чем причина убыточности приложения, кроется в этих графиках. Здесь отчетливо видно нехарактерное поведение красной линии, а именно пользователей из США. Несмотря на то, что пользователи США имеют бОльшую "пожизненную ценность", т.е. сумарно приносят больше прибыли, ROI пользователей этой страны ниже, чем у пользователей других стран. И на протяжении, практически, всего времени, "США" не окупаются. А всё потому, что САС у них стремительно растёт. Здесь так же можно заметить, что ROI пошёл в минус именно тогда, когда начали резко возрастать затраты на рекламу.
