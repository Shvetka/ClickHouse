Установлен Clickhouse  
[Скрин работающего ClickHouse](scsh1.png)  
Добавлен конфигурационный файл для тестирования настроек(пробую сделать хуже чем было)  
/etc/clickhouse-server/config.d/memory.xml  
  
<?xml version="1.0"?>  
<clickhouse>  
  <listen_host>::</listen_host>  
  <max_memory_usage_for_all_queries>200</max_memory_usage_for_all_queries>  
</clickhouse>  

С таким параметром запрос выполняется 0.46, без него 0.008   
[Скрин с настройкой](scsh2.png)  
[Скрин без настройки](scsh3.png)  
