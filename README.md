## Hospitality Overview

*Представьте, что вы **менеджер продукта** в отеле Karpov.Inn. Ваш партнер по заданию будет задавать вам вопросы, а вы должны отвечать ему, исходя из информации, описанной ниже. Не показывайте и не передавайте этот документ вашему коллеге! Он должен получить эти знания, проведя интервью с вами. Если во время интервью появится вопрос, в котором будет что-то, что не было описано ниже, можете придумать решение, исходя из здравого смысла (только не увлекайтесь).*

Ваше подразделение занимается работой с отелями, которые вы предоставляете, поиском инвестиций в них и улучшениями вариантов их бронирования. Вы отвечаете за открытие/закрытие новых отелей, анализ заполняемости текущих, а также за оптимизацию их бронирования.

За некоторыми метриками вы регулярно следите, к ним относятся: 

- выручка от бронирований,
- количество бронирований,
- средняя стоимость номеров,
- среднее время пребывания.

За этими метриками вы следите каждую неделю и отмечаете отклонения неделя к неделе, которые составляют +-10% WoW (неделя к неделе). В самом дашборде также возможность детализации до месяца (помимо недель), там аналогичный KPI – отклонение в +-10% MoM (месяц к месяцу).

На основании **количества бронирований и выручки по отелям** вы принимаете решение о дополнительных инвестициях в них или о поиске отелей похожего типа. На основании **анализа каналов бронирования** вы ищите способы расширения каналов или закрытия существующих, в зависимости от выручки и заявок, которые они генерируют. Поэтому важно иметь возможность сравнения основных метрик по отелям и каналам бронирования.

Вам хотелось бы иметь общие фильтры на весь дашборд по дате (date), отелю (property) и типу комнаты (room_type) и каналу бронирования .

Отдельно вы анализируете самые прибыльные бронирования отдельно по каждому отелю. Вам важно иметь возможность проанализировать детали резервации и посмотреть детальную информацию о тех бронированиях, которые принесли наибольшую выручку. Это вы делаете в CRM системе по номеру резервации из таблицы. 

Вам нужен общий дашборд, который показывал бы общее состояние метрик по отелям и каналам бронирования, а также список прибыльных бронирований. В настоящее время нам приходится еженедельно вручную извлекать данные из базы данных и компилировать их для наших еженедельных собраний. 

Дашборд будет использоваться всеми членами вашей команды: руководителем, менеджерами ответственными за каналы бронирования и менеджерами каждого из отелей.

После просмотра дашборда вы принимаете решение о состоянии каждого отеля и необходимости плотной работы с ним: рекламные кампании, анализ удовлетворенности посетителей в них для более детального анализа. При анализе каналов вы делаете выводы о необходимости подключений большего количества тревел-агентств или собственных расширении колл-центров. 

Дашборд вы смотрите каждую неделю по понедельникам для отслеживания основных метрик как «health check», а также раз в месяц для стратегического планирования

### Данные

*Когда вас спросят про данные, дайте коллеге [ссылку на данные](https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Hospitality.csv).*

- avg_room_rate: средняя стоимость номера в $ (числовое значение);
- reservation_id: идентификатор бронирования (уникальный идентификатор);
- date: дата записи (дата);
- check_in_date: дата заезда (дата и время);
- property: отель (текстовое значение);
- booking_channel: канал бронирования (текстовое значение);
- stay_duration: длительность пребывания (числовое значение, например, количество дней);
- adults: количество взрослых гостей (целое число);
- children: количество детей (целое число);
- room_type: тип комнаты (текстовое значение);
- special_requests_flag: флаг особых запросов (логическое значение, например, true/false);
- booking_channel: канал бронирования (текстовое значение);
- reservation_status: статус бронирования (текстовое значение);
- advanced_booking: количество дней между бронированием и датой заезда (числовое значение);
- rate_type: тип тарифа (текстовое значение).
