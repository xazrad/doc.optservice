==================================
receivabledocs
==================================

Осуществляет импорт информации о кредитных документах задолженности контрагентов Заказчика.

Информация о свойствах каждой записи содержится в атрибутах тега "item".

Атрибуты выделенные **жирным шрифтом** не могут иметь пустых значений

Используемые атрибуты:

* **"id"** - Уникальный идентификатор документа

* **"firm"** - Уникальный идентификатор организации

* **"customer"** - Уникальный идентификатор контрагента.

* "shop" - Уникальный идентификатор торговой точки.

* "contract" - Уникальный идентификатор договор контрагента.

* "agent" - Уникальный идентификатор агента.

* **"docname"** - Наименование кредитного документа.

* **"docdate"** -  Дата кредитного документа в формате YYYY-MM-DD.

* **"doctotal"** - Сумма кредитного документа.

* **"docdebt"** - Остаток суммы взаиморасчетов по документу.

* **"doctype"** - Тип документа: 1 - Отгрузка, 2 - Возврат, 3 - Оплата, 4 - Иной.

* "docdatepayment" - Предполагаемая дата оплаты документа в формате YYYY-MM-DD.

Поля "id", "agent", "contract" обеспичивают уникальность записи

Пример::

 <receivabledocs>
   <item firm="f63c2ffe-e382-11e1-a5b1-0015175ffdb8" contract="0ddd1304-dafc-11e1-b7e9-0015175ffdb8" shop="" customer="1a909a1b-dafb-11e1-b7e9-0015175ffdb8" agent="2c7025cf-e2d7-11e1-a5b1-0015175ffdb8" docname="Реализация товаров и услуг ОМ000005475 от 21.02.2013 16:28:46" docdate="2013-02-21 16:28:46" doctype="1" DocSumm="50.1" docdebt="50.1" docdatepayment=""/>
   <item firm="e4702366-daf6-11e1-b7e9-0015175ffdb8" contract="2ce6a4b0-021d-11e2-ae27-0015175ffdb8" shop="" customer="1a909b52-dafb-11e1-b7e9-0015175ffdb8" agent="2c7025d8-e2d7-11e1-a5b1-0015175ffdb8" docname="Реализация товаров и услуг ОМ000008423 от 25.03.2013 16:27:16" docdate="2013-03-25 16:27:16" doctype="1" DocSumm="9923.44" docdebt="9471.16" docdatepayment=""/>
   <item firm="e4702365-daf6-11e1-b7e9-0015175ffdb8" contract="0ddd136e-dafc-11e1-b7e9-0015175ffdb8" shop="" customer="1a909a30-dafb-11e1-b7e9-0015175ffdb8" agent="44a4fab9-e2e6-11e1-a5b1-0015175ffdb8" docname="Ввод начальных остатков по взаиморасчетам 00000008182 от 31.08.2012 0:00:00" docdate="2012-08-31 00:00:00" doctype="4" DocSumm="" docdebt="-0.24" docdatepayment=""/>
   <item firm="f63c2ffe-e382-11e1-a5b1-0015175ffdb8" contract="07b9e5ed-dafc-11e1-b7e9-0015175ffdb8" shop="" customer="13cdafbd-dafb-11e1-b7e9-0015175ffdb8" agent="2c7025e3-e2d7-11e1-a5b1-0015175ffdb8" docname="Реализация товаров и услуг ОМ00048783 от 07.12.2012 16:48:17" docdate="2012-12-07 16:48:17" doctype="1" DocSumm="1746.31" docdebt="768.18" docdatepayment=""/>
   <item firm="e4702366-daf6-11e1-b7e9-0015175ffdb8" contract="07b9e5db-dafc-11e1-b7e9-0015175ffdb8" shop="" customer="213baf2d-dafb-11e1-b7e9-0015175ffdb8" agent="2c7025d9-e2d7-11e1-a5b1-0015175ffdb8" docname="Реализация товаров и услуг ОМ000000248 от 08.01.2013 16:09:49" docdate="2013-01-08 16:09:49" doctype="1" DocSumm="319.6" docdebt="319.6" docdatepayment=""/>
   <item firm="e4702366-daf6-11e1-b7e9-0015175ffdb8" contract="07b9e5db-dafc-11e1-b7e9-0015175ffdb8" shop="" customer="213baf2d-dafb-11e1-b7e9-0015175ffdb8" agent="2c7025d9-e2d7-11e1-a5b1-0015175ffdb8" docname="Реализация товаров и услуг ОМ000000252 от 08.01.2013 16:11:40" docdate="2013-01-08 16:11:40" doctype="1" DocSumm="3030.66" docdebt="3030.66" docdatepayment=""/>
 </receivabledocs>