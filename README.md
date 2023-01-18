---
description: Руководство пользователя
---

# Primo RPA

![](<.gitbook/assets/Заставка.png>)

Платформа Primo RPA - это российский комплекс программных продуктов, предназначенный для роботизации бизнес-процессов.

Pешение Primo RPA позволяет:
1. Сократить себестоимость процессов за счет передачи роботу рутинных, повторяемых операций.
2. Выполнять роботизируемые операции быстрее, обеспечивая рост прибыли и лояльности клиентов. 
3. Снижать число ошибок, вызванных «человеческим фактором».

## Функциональные возможности Primo RPA
В комплекс продуктов Primo RPA входит следующее программное обеспечение:
* Primo RPA Studio
* Primo RPA Robot
* Primo RPA Orchestrator 

### Primo RPA Studio

**Primo Studio** - это основной инструмент для разработки роботов. Именно здесь аналитики и разработчики собирают RPA-сценарий, используя как готовые компоненты, так и компоненты собственной разработки. 

Ключевые возможности:
1. **Создание сценария для Робота**. Разрабатывать сценарий можно в виде последовательности операций, диаграммы или в виде чистого кода, что позволяет роботизировать сценарии практически любой сложности. Набор сценариев составляет единый RPA-проект, в рамках которого доступна группировка сценариев по папкам. 
2. **Отладка сценария**. Позволяет протестировать сценарий через Студию и отследить результаты выполнения в Консоли. Помогает проанализировать и исправить ошибки в сценариях до публикации проекта.
4. **Использование зависимостей**. Возможно обращаться к дополнительным библиотекам при работе с RPA-проектом. Доступна возможность разрабатывать, опубликовывать и использовать собственные библиотеки в проекте.
5. **Шаблоны проекта**. Возможность сделать из готового проекта шаблон, который будет применяться при создании новых проектов. 
6. **Шаблоны поиска**. Используются для взаимодействия с пользовательским интерфейсом программ. Позволяют идентифицировать компонент приложения, чтобы получить к нему программный доступ.
7. **Расширение RDP**. Имеется возможность взаимодействовать с компонентами приложений удаленного рабочего стола.
8. **Запись трафика**. Помогает быстро и легко анализировать обмен с порталами, сайтами и веб-сервисами, а также формировать Web-запросы в сценариях на основе полученных данных.

### Primo RPA Robot

**Primo Robot** - робот, выполняющий заданные пользователем сценарии и поддерживающий работу как в среде Windows, так и в Linux, что особенно важно для компаний, активно использующих рабочие места на базе, например, отечественных операционных систем типа Astra Linux.

С приложением Primo Robot возможно работать как из командной строки, так и через графический интерфейс пользователя - при помощи ПО Primo Robot Runner (входит в комплект поставки).

Ключевые возможности Primo Robot:
1. Создание и запуск задач по выполнению RPA-проектов вручную. 
3. Интеграция с Оркестратором. Позволяет управлять Роботами автоматически через Оркестратор. 
4. Запись в журнал логов выполнения проекта.
5. Запись в журнал пользовательских событий.

Возможности Primo Robot Runner:
1. Автоматический запуск задач по выполнению RPA-проектов. 
2. Настройка расписаний. Расписания позволяют запускать задачи в соответствии с заданным графиком.
3. Работа со станциями.


### Primo RPA Orchestrator 
**Primo Orchestrator** -  предназначен для автоматизации запуска RPA-проектов на множестве развернутых в Организации роботов и для управления роботами. Оркестратор позволяет задавать расписание работы роботов, контролировать их работу. Для поддержки работы крупных компаний с несколькими независимыми группами пользователей Primo RPA Orchestrator предоставляет возможность «изолировать» группы роботов друг от друга. За счет поддержки мультитенантности пользователь каждой группы будет видеть и управлять только своими роботами, без возможности влияния на роботов других групп.

Ключевые возможности:
1.



## Системные требования

### Primo Studio

Для установки и эксплуатации ПО Primo Studio требуются:

| Параметры    |  OС | ПО |
| ------------ | ------------- | ----- |
| CPU 4 ядра, RAM 8 Гб, HDD 100 Гб | Microsoft Windows 7 (SP2) и выше | <p>Microsoft .NET Framework 4.6.1;</p><p>Microsoft Visual C++ Runtime 14;</p><p>Windows PowerShell.</p><br> Права локального администратора (в зависимости от используемых компонентов)</br> |

### Машина Робота

Для установки и эксплуатации ПО Robot\* необходимо, чтобы машина Робота соответствовала требованиям:

> \**Для роботов, работающих как с Оркестратором, так и без него.*

| Параметры     |  OС |
| ------------- | ------------- |
| CPU 8 ядер, RAM 8 Гб, HDD 250 Гб  | Windows 10 / Windows Server 2016 и выше |
| CPU 6 ядер, RAM 8 Гб, HDD 250 Гб  | Linux: CentOS 8+, Ubuntu 20+, Astra Linux 1.7+ |

### Оркестратор

Для установки и эксплуатации ПО Orchestrator требуются:

| Наименование   | Параметры     | ОС  |
| ------------- | ------------- | ----- |
| Сервер Оркестратора | CPU 8 ядер, RAM 16 Гб, HDD 200 Гб | Windows Server 2016 и выше. <p>Linux: CentOS 8+, Ubuntu 20+, Astra Linux 1.7+ </p> |
| Сервер БД | CPU 8 ядер, RAM 16 Гб, HDD 200 Гб  | см. выше |
| Сервер журнала | CPU 8 ядер, RAM 16 Гб, HDD 1000 Гб | см. выше |
