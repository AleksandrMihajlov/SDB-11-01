Базы данных, их типы - Aleksandr Mihajlov SYS34  
  
**Задание 1. СУБД**  
  
Кейс  
  
Крупная строительная компания, которая также занимается проектированием и девелопментом, решила создать правильную архитектуру для работы с данными.   
Ниже представлены задачи, которые необходимо решить для каждой предметной области.

Какие типы СУБД, на ваш взгляд, лучше всего подойдут для решения этих задач и почему?  
  
1.1. Бюджетирование проектов с дальнейшим формированием финансовых аналитических отчётов и прогнозирования рисков.   
СУБД должна гарантировать целостность и чёткую структуру данных.   
*- Реляционные СУБД: MySQL, PostgreSQL, MariaDB*  
  
1.2. Под каждый девелоперский проект создаётся отдельный лендинг, и все данные по лидам стекаются в CRM к маркетологам и менеджерам по продажам.   
Какой тип СУБД лучше использовать для лендингов и для CRM? СУБД должны быть гибкими и быстрыми.   
*- Графовые СУБД: Neo4j, Amazon Neptune, Apache Giraph, JanusGraph и ArangoDB*  
  
1.3. Отдел контроля качества решил создать базу по корпоративным нормам и правилам, обучающему материалу и так далее, сформированную согласно структуре компании. СУБД должна иметь простую и понятную структуру.  
 *- Документная СУБД: CouchDB, MongoDB, Amazon DocumentDB*  
  
1.4. Департамент логистики нуждается в решении задач по быстрому формированию маршрутов доставки материалов по объектам и распределению курьеров по маршрутам с доставкой документов. СУБД должна уметь быстро работать со связями.   
*- Возможно это графовые СУБД*  
  
**Задание 2. Транзакции**  
  
2.1. Пользователь пополняет баланс счёта телефона, распишите пошагово, какие действия должны произойти для того, чтобы транзакция завершилась успешно.  
Ориентируйтесь на шесть действий.  
  
*- Отправка запроса от пользователя*  
*- Информация о сумме пополнения*  
*- Проверка текущего баланса*  
*- Суммирование баланса*  
*- Подтверждение операции*  
*- Конец операции*  
  
**Задание 3. SQL vs NoSQL**  
  
3.1. Напишите пять преимуществ SQL-систем по отношению к NoSQL.  
  
*- Использование языка SQL запросов*  
*- Использование ACID*  
*- Безопасность*  
*- Поддержка и сообщества*  
*- Управление структурированными данными*  
  
**Задание 4. Кластеры**  
  
Необходимо производить большое количество вычислений при работе с огромным количеством данных, под эту задачу выделено 1000 машин.

На основе какого критерия будете выбирать тип СУБД и какая модель распределённых вычислений здесь справится лучше всего и почему?

Приведите ответ в свободной форме.  
  
*Главные критерии:*  
*-Сложность модели данных*  
*-Согласованность и доступность*  
*-Масштабируемость*  
*-Затраты*

*Воможно стоит рассмотреть модель MapReduce*
