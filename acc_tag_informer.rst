==================================
informer
==================================

Осуществляет импорт информации об истории документов.

Информация о свойствах каждой записи содержится в атрибутах тега "item".

Атрибуты выделенные **жирным шрифтом** не могут иметь пустых значений

Используемые атрибуты:

* **"doc"** - Уникальный идентификатор документа в учетной системе заказчика.

* **"comment"** - Комментарий о статусе документа, максимальная длинна 255 символов

* "date" - Дата изменения статуса документа в формате %Y-%m-%d %H:%M:%S, при отсутствии значения будет подставлено время импорта записи

Пример::

 <informer>
   <item doc="a15092f2-4348-11dd-ac9f-0015e9b8c48d" comment="Принят в 1С" date="2020-06-29 08:15:27"/>
 </informer>