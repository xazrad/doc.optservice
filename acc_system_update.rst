====================
Импорт справочников 
====================

Пример: http://api.opt-service.com/acc_system_update/

Импорт подразумевает выгрузку справочников из Учетной Системы на Сервер.

Импорт осуществляется в формате XML.

Файл XML имеет корневой узел **<root>**.

Каждый элемент справочника "обрамлен" тегом **<item>**.

Поток данных может представлять собой ZIP архив, для этого в заголовке необходимо указать параметр compressed = “1”. 
Из архива для обработки берется только первый файл. Если размер первого файла после распаковки будет превышать 50 megabits (52428800 bytes) - система отсылает ошибку - “limit file size”

**ВАЖНО!**:

Все наименования тегов, а также имена  атрибутов указываются в **нижнем** регистре

Пример::
    
    ﻿<?xml version="1.0" encoding="UTF-8"?>
    <root>
	  <stores>
		<item id="bd72d91f-55bc-11d9-848a-00112f43529a" name="Главный склад"/>
		<item id="1de4815f-fd36-11db-a40e-00055d80a2d1" name="Торговый зал (офис)"/>
	  </stores>
	  <customers>
		<item id="cbcf491c-55bc-11d9-848a-00112f43529a" name="АОЗТ Лабан"/>
		<item id="cbcf494b-55bc-11d9-848a-00112f43529a" name="Белявский Олег Константинович"/>
		<item id="dee6e17e-55bc-11d9-848a-00112f43529a" name="ТОО ЭКИП"/>
	  </customers>	
    </root>
   


Список используемых узлов-тегов:

.. toctree::

   acc_tag_customers.rst
   acc_tag_shops.rst
   acc_tag_goods.rst
   acc_tag_agents.rst
   acc_tag_routes.rst
   acc_tag_stores.rst
   acc_tag_pricelists.rst
   acc_tag_firms.rst
   acc_tag_contracts.rst
   acc_tag_units.rst
   acc_tag_prices.rst
   acc_tag_stocks.rst
   acc_tag_receivabledocs.rst
   acc_tag_saleshistory.rst
   acc_tag_docs.rst

   
   






   
   

    


