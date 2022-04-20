# Tinkoff Invest Robot Contest
## Соревнуемся в создании торговых роботов

Мы проводим конкурс по разработке торгового робота для Тинькофф Инвестиций. Задача участников — написать пример торговой системы, которая реализует любую торговую стратегию на бирже. Работать она должна на новом [API Тинькофф Инвестиций](https://github.com/Tinkoff/investAPI). 

В конкурсе семь номинаций, указанных ниже. Победитель в каждой номинации получит 200 тысяч рублей. 

Мы ждем разработчиков старше 18 лет уровня junior+ и выше, интересующихся алгоритмическим трейдингом. Ограничений по языкам программирования нет, но предпочтительнее писать на Java, Go, Python и Java Script. Чтобы зарегистрироваться, оставьте заявку на [странице конкурса](https://meetup.tinkoff.ru/event/tinkoff-invest-robot-contest/) до 23 мая включительно и следуйте инструкциям. 

# Номинации 

- Лучший пример торгового робота на языке python 

- Лучший пример торгового робота на языке go 

- Лучший пример торгового робота на языке js 

- Лучший пример торгового робота на языке java

- Лучший торговый робот для мобильных устройств 

- Лучший интерфейс (визуализация) торговой стратегии

- Самое оригинальное использование API Тинькофф Инвестиций

## С чего начать 

1. Вы должны быть клиентом Тинькофф Инвестиций. В разделе [настройки](https://www.tinkoff.ru/invest/settings/) сгенерируйте новый токен для доступа к API.
2. Ознакомьтесь с [описанием API](https://tinkoff.github.io/investAPI/), если вы никогда не сталкивались с протоколом [gRPC](https://grpc.io/docs/), прочтите [документацию](https://tinkoff.github.io/investAPI/grpc/)
3. Посмотрите [примеры коннектров на разных языках программирования](https://tinkoff.github.io/investAPI/) или можете сгенерировать коннекторы на любом языке программирования самостоятельно на основе [proto-контрактов](https://github.com/Tinkoff/investAPI/tree/main/src/docs/contracts)
4. Ознакомьтесь с нашим [глоссарием](https://tinkoff.github.io/investAPI/glossary/) и помощью [Тинькофф Инвестиций](https://help.tinkoff.ru/investments/?)
5. Для начала загрузите [список торгуемых ценных бумаг](https://tinkoff.github.io/investAPI/head-instruments/) и [историю котировок ценных бумаг](https://tinkoff.github.io/investAPI/head-marketdata/) - локально будет проще тестировать торговые гипотезы.
6. Выберете (или придумайте) торговые гипотезы, которые хотите проверить. Потестируйте их на истории котировок.
7. Попробуйте реализовать работу торговой гипотезы на "[песочнице](https://tinkoff.github.io/investAPI/head-sandbox/)" - специальном сервисе-эмуляторе брокера, при котором ваши торговые поручения не выводятся на биржу и вы не несете рисков потери средств.
8. Если алгоритм показывает хорошие результаты на песочнице, то реализуйте выставление ордеров на [реальную биржу](https://tinkoff.github.io/investAPI/head-orders/) 
9. Добавьте отображение статистики работы торгового алгоритма, чтобы вам было проще отслеживать эффективность робота
10. По завершению подготовьте описание работы алгоритма в свободной форме - и присылайте нам в одну из [номинаций](https://github.com/Tinkoff/invest-robot-contest/issues?q=is%3Aissue+is%3Aopen+label%3A%D0%9D%D0%BE%D0%BC%D0%B8%D0%BD%D0%B0%D1%86%D0%B8%D1%8F) 

Желаем успеха!  

## Примеры торговых стратегий
Так как цель конкурса - в разработке примеров кода роботов, работающих через Tinkoff Invest, то стратегии могут быть любые по выбору участника. 
Выбранный тип стратегии не влияет на итоговую оценку работы. 
Примеры текстовых описаний стратегий можно посмотреть [здесь](https://github.com/Tinkoff/invest-robot-contest/blob/main/examples.md)

## Каким должно быть решение

### Требования к работам участников (кроме номинаций №6 и №7)
* описание торгового алгоритма в свободной форме; 
* реализация исполнения поручений (заявок на продажу/покупку ценных бумаг) как в "песочнице" (специальном сервисе, предназначенным для тестирования стратегией без вывода ордеров на реальную биржу) так и в "боевом" режиме.
* ведение статистики работы алгоритма
* предварительная загрузка системой истории рыночных котировок и проведение бэктеста(тестирования стратегии на исторических данных) на уже загруженных данных;

### Загруженный на GitHub код

* Свободно скачивается, и компилируется на операционных системах Mac, Windows и Linux-подобных
* Не требует установленных дополнительных решений, кроме компилятора конкретного языка
* Все используемые компоненты и библиотеки должны распространяться под лицензией apache 2 или аналогичных
* Важно маркировать все выставляемые ордера с [appname](https://tinkoff.github.io/investAPI/grpc/#appname), соответствующему нику участника на Github.com или названию решения
* К коду нужно приложить инструкцию по установке и запуску решения

## Этапы конкурса 

Зарегистрируйтесь: оставьте заявку [странице конкурса](https://meetup.tinkoff.ru/event/tinkoff-invest-robot-contest/) до 23 мая включительно. На почту придет письмо с подтверждением регистрации.

- Создайте пример торгового робота и разместите его в своем репозитории на Github на условиях открытой лицензии Apache 2.0. Сделать это нужно 23 мая до 23:59
- Отметьтесь в треде соответствующей номинации, оставив ссылку на репозиторий.
- Дождитесь оценок жюри. Жюри проверит решения участников до 27 мая и выберет победителей. Подробнее о критериях оценки работ читайте [здесь](https://github.com/Tinkoff/invest-robot-contest/blob/main/score.md). 
- Если победили - получите приз! 

## Коммуникации

Если у вас есть любые вопросы по конкурсу - задавайте их:
* либо в Телеграмм чате https://t.me/tinkoff_invest_robot_contest
* либо в [Issue Github](https://github.com/Tinkoff/invest-robot-contest/issues) 






