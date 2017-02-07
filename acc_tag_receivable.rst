==================================
receivable
==================================

** В настоящее время неиспользуется**

Осуществляет импорт информации о задолженности контрагентов Заказчика в разрезе торговых точек и агентов.

Информация о свойствах каждой записи содержится в атрибутах тега "item".

Атрибуты выделенные **жирным шрифтом** не могут иметь пустых значений

Используемые атрибуты:

* **"customer"** - Уникальный идентификатор контрагента.

* "shop" - Уникальный идентификатор торговой точки.

* "agent" - Уникальный идентификатор агента.

* **"receivable"** - Сумма задолженности.

* "overdue" -  Сумма просроченной задолженности.

* "overduedays" - Количество дней просроченного долга.

Пример::

 <receivable>
   <item customer="a15092f2-4348-11dd-ac9f-0015e9b8c48d" shop="a15092f2-4348-11dd-ac9f-0015e9b8c48d" agent="" receivable="308250" overdue="1000" overduedays="3"/>
   <item customer="a15092f4-4348-11dd-ac9f-0015e9b8c48d" shop="a15092f4-4348-11dd-ac9f-0015e9b8c48d" agent="" receivable="40180" overdue="0" overduedays="0"/>
   <item customer="a15092f6-4348-11dd-ac9f-0015e9b8c48d" shop="a15092f6-4348-11dd-ac9f-0015e9b8c48d" agent="" receivable="21926" overdue="0" overduedays="0"/>
   <item customer="f8fa030b-4412-11dd-aca0-0015e9b8c48d" shop="f8fa030b-4412-11dd-aca0-0015e9b8c48d" agent="" receivable="360000" overdue="0" overduedays="0"/>
   <item customer="f8fa030d-4412-11dd-aca0-0015e9b8c48d" shop="f8fa030d-4412-11dd-aca0-0015e9b8c48d" agent="" receivable="353409.15" overdue="0" overduedays="0"/>
 </receivable>
