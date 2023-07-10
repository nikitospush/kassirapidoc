### Оригинальная документация для Kassir.kartina.tv ###

Для работы вам понадобится UID. Его нужно запросить по почте
[ib@kartina.tv](ib@kartina.tv)

### Примеры на Postman

https://go.postman.co/workspace/My-Workspace~95024bc4-a36e-4d54-8cbe-3bc72cdc3ad5/collection/1253875-a66a4408-2a77-5816-2a92-cbde8d896752


#### эти два запроса надо перед созданием заказа прогнать
https://kassir.kartina.tv/SavePaymentOptions.cmd
https://kassir.kartina.tv/SaveDeliveryOptions.cmd

paymentType = BANK_PAY

deliveryType= ETICKET

#### разъяснение что значит client, login password

в запросе на создание заказа /ConfirmOrderCommand.cmd есть следующие переменные
```
__auth   = это токен полученный после авторизации **пользователя** партнера через который делаются API колы;
login    = логин от **пользователя** партнера через который делаются API колы;
password = пароль от **пользователя** партнера через который делаются API колы; 
order    = номер заказа
status   = 1 - подтвержденный заказ. 
email    = Email клиента
client   = ID клиента 
format   = json
```

UID пользователя, login, password можно получить от сотрудников biletkartina.tv 