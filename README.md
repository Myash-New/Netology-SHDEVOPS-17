Домашнее задание к занятию 1. «Введение в виртуализацию»

Ответы на задачу 2.

Выбор типа платформы для решения задачи:
1) высоконагруженная база данных MySql, критичная к отказу
	Мне кажется оптимальным выбором паравиртуализация, т.к. это возможность получить сбалансированное отказоустойчивое решение при умеренных затратах. 
	Решения на физических серверах будет стоить значительно дороже.

2) различные web-приложения;
	Мне кажется оптимальным выбором будет виртуализация уровня ОС - это даст максимальную гибкость и масштабируемость при небольшой цене.

3) Windows-системы для использования бухгалтерским отделом;
	Мне кажется оптимальным выбором будет паравиртуализация Hyper-V от Microsoft, т.к. предполагается эко-система от Microsoft, встроенные механизмы отказоустойчивости и масштабируемости. Наличие специалистов знакомых с Windows Server и тп.

4) системы, выполняющие высокопроизводительные расчёты на GPU.
	Мне кажется оптимальным выбором будет физические серверы для максимальной производительности, ресурсы GPU напрямую доступны для вычислений без накладных расходов на виртуализацию. Полный контроль над оборудованием и драйверами.



Ответы на задачу 3.

Выберите подходящую систему управления виртуализацией для предложенного сценария. Опишите ваш выбор.

Сценарии:

1. 100 виртуальных машин на базе Linux и Windows, общие задачи, нет особых требований. Преимущественно Windows based-инфраструктура, требуется реализация программных балансировщиков нагрузки, репликации данных и автоматизированного механизма создания резервных копий.
	VMware vSphere — это наиболее подходящее решение:
  o	 отличная поддержке Windows-based инфраструктуры.
  o	 встроенные механизмы балансировки нагрузки, репликации и отказоустойчивости.
  o	 удобство управления и масштабируемости.
	
2. Требуется наиболее производительное бесплатное open source-решение для виртуализации небольшой (20-30 серверов) инфраструктуры на базе Linux и Windows виртуальных машин.
	XEN — это наиболее подходящее решение:
  o	 Простота интеграции с Linux
  o	 Удобство управления
  o	 Поддержка Windows

3. Необходимо бесплатное, максимально совместимое и производительное решение для виртуализации Windows-инфраструктуры.	
		Microsoft Hyper-V — это наиболее подходящее решение:
  o	 бесплатно (в составе Windows Server или как Hyper-V Server)
  o  максимальной совместимостимо с Windows-инфраструктурой
  o	 высокая производительность и интеграция с экосистемой Microsoft.

4. Необходимо рабочее окружение для тестирования программного продукта на нескольких дистрибутивах Linux.
	KVM — это наиболее подходящее решение:
   o	бесплатно + открытый исходной код
   o	высокая производительность и поддержка различных дистрибутивов Linux.

Ответ на задачу 4
Опишите возможные проблемы и недостатки гетерогенной среды виртуализации (использования нескольких систем управления виртуализацией одновременно) и что необходимо сделать для минимизации этих рисков и проблем. Если бы у вас был выбор, создавали бы вы гетерогенную среду или нет?
 Проблемы и недостатки гетерогенной среды виртуализации
1. Сложность управления: разные инструменты управления, интерфейсы и API.
2. Проблемы совместимости: сложность миграции VM между разными системами виртуализации
3. Высокие затраты на поддержку: лицензии + затраты на обучение персонала
4. Сложно эффективно использовать ресурсы(серверы, хранилища, сети)
5. Ограниченная автоматизация задач
6. Проблемы с мониторингом и аналитикой - разные инструменты мониторинга

Способы минимизации рисков и проблем
1. Стандартизация процессов и инструментов
2. Интеграция через API
3. Обучение персонала:
4. Использование инструментов для конвертации виртуальных машин между разными форматами
5. Внедрение единой системы мониторинга, поддерживающей разные платформы виртуализации 

Личный выбор
Если бы у меня был выбор, я бы не создавал гетерогенную среду, если в этом нет крайней необходимости.

