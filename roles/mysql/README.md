
## Данная роль развертывает кластер баз данных galera.

### Проверим статус кластера galera когда все ВМ запущены:

- show status like 'wsrep_cluster_status';
- show status like 'wsrep_cluster_size';
- show status like 'wsrep_local_state_comment';

![image](screens/wsrep_db1.png)

### Проверим статус кластера galera после жесткого выключения одной ВМ:

- show status like 'wsrep_cluster_status';
- show status like 'wsrep_cluster_size';
- show status like 'wsrep_local_state_comment';

![image](screens/wsrep_db2_after_crash.png)

- visit http://demosite.local

![image](screens/demo_after_dbcrash.png)

- Как мы видим наш сайт доступен. 