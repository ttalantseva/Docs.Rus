# Аппаратные требования

## Оркестратор

Аппаратные требования к Оркестратору\*  для управления до 250\** Роботов одновременно приведены в таблице ниже:

| Параметр | Требование | 
| -------- | ---------- | 
| CPU      | 16 ядер    |    
| RAM	     | 16 Гб (рекомендуемая 32 Гб) | 
| HDD      | 1000 Гб (OS + Data) | 

> *\* Обобщенные требования ко всем компонентам бэкэнда Системы.*\
> \** *Обобщенное требование. В зависимости от выполняемого проекта/настроек логирования Робот может создавать разную нагрузку на Оркестратор.*

У БД с логами ожидается быстрый рост объема. Ежедневный прирост – индивидуальная величина для разных пользователей (зависит от количества логов, которые создают работающие роботы) – может быть оценен по результатам эксплуатации. И на его основе может быть оценен более точно объем HDD и определена периодичность ротации/очистки логов. Величина 1000 Гб взята как усредненная оценка для комфортной работы.

**Оценка объема HDD может быть произведена следующим образом:**

Пусть 10 роботов параллельно работают 24 часа в сутки. Каждый обращается в Оркестратор 10 раз в секунду. Суммарно – 100 запросов в секунду. Пусть за один запрос Роботом отдается 0,1 Кб. Ежесуточный прирост = 100 \* (24 \* 60 \* 60) \* 0,1 = 864000 Кб = ~1 Гб.

Если используется поддержка RDP-сессий, надо исходить из оценки: один сервис поддержки RDP на 20 сессий. Это должна быть отдельная машина с CPU 4 ядра и RAM 16 Гб. Или эти ресурсы должны быть включены в сервер Оркестратора.

## Машина Робота

Аппаратные требования к машине Робота (рабочей станции):

| Параметр | Windows    | Linux  |
| -------- | ---------- | ------ |
| CPU      | 8 ядер     | 6 ядер |
| RAM      | 8 Гб       | 8 Гб   |
| HDD      | 250 Гб (OS + Data) | 250 Гб (OS + Data) |
 
Обязательно требуется установить последние обновления ОС.
