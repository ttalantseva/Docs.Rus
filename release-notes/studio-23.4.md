# Primo Studio 23.4

Примечания к выпуску Студии 23.4 описывают изменения для версии приложения, выпущенной в апреле 2023 года.

## Новые функции 
1. Добавлена востребованная возможность автоматизации процессов на виртуальных машинах под Citrix с использованием канала ICA, что существенно упрощает развертывание в закрытом контуре и позволяет повысить безопасность.
1. Значительно ускорено чтение больших Excel-файлов с драйвером Interop. Например, при чтении таблицы в 100 тыс. строк скорость выполнения повысилась в 3 раза.
1. В NuGet появилась библиотека для интеграции робота с Python - [**Primo.Python**](https://www.nuget.org/packages/Primo.Python). Ее также можно скачать через [Менеджер зависимостей](https://docs.primo-rpa.ru/primo-rpa/primo-studio/projects/manage-dependencies#menedzher-zavisimostei) Студии. Библиотека содержит набор элементов, которые позволяют взаимодействовать со сценарием, функциями и объектами на языке Python, а именно:
   * [**Python**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_extra/els_python/el_pythonscope) - устанавливает соединение с Python.exe. Требуется установленный Python 3.9 и Pywin32. 
   * [**Выполнить скрипт**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_extra/els_python/el_execscript) - выполняет сценарий Python.
   * [**Получить объект**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_extra/els_python/el_getobject) - позволяет получить объект Python и привести его к нужному типу.
   * [**Добавить функцию**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_extra/els_python/el_addfunction) - добавляет функцию Python, которую впоследствии можно вызвать.
3. В NuGet появилась библиотека для интеграции робота с Java - [**Primo.Java**](https://www.nuget.org/packages/Primo.Java). Она содержит набор элементов для работы с методами и объектами на языке Java, а именно:
   *  **Java** - устанавливает соединение с Java.exe. На машине должна быть установлена Java 8.
   *  **Загрузить Jar** - загружает файл \*.jar в контекст Java.
   *  **Создать объект Java** - создает объект Java с заданным типом.
   *  **Вызвать метод Java** - вызывает нужный метод в экземпляре Java.
   *  **Получить поле** - получает поле объекта Java.
   *  **Преобразовать объект Java** -  преобразовывает объект Java к нужному типу.
5. В NuGet добавлена библиотека [**Primo.Active Directory**](https://www.nuget.org/packages/Primo.ActiveDirectory). Пакет содержит набор элементов для взаимодействия с доменными службами Active Directory (AD DS), которые сгруппированы по их назначению:
   * **Группы** - набор элементов для управления группами в AD: создание, удаление, проверка того, что группа существует. 
   * **Компьютеры** - набор элементов для управления компьютерами: создание, удаление, добавление в группу, проверка того, что компьютер существует и др.
   * **Общие** - набор элементов для управления объектами: получение/изменение свойств объекта, переименование объекта, перемещение и др.
   * **Пользователи** - набор элементов для управления пользователями: создание, удаление, управление учетной записью и паролем, а также другие возможности.
6. В NuGet обновилась библиотека [**Primo.Networking**](https://www.nuget.org/packages/Primo.Networking). Теперь в нее входит элемент [**Запрос SOAP**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_extra/els_networking/el_soaprequest), который позволяет выполнять стандартные виды запросов к сервисам SOAP. 
7. [В разделе задач](https://docs.primo-rpa.ru/primo-rpa/primo-robot/robot-runner/tasks) Robot Runner внесены улучшения в интерфейс: 
   * добавлен признак, указывающий на выполнение задачи роботом. Теперь в общем списке задач можно легко отследить, какие задачи выполняются в данный момент; 
   * кнопка быстрого запуска задачи была уменьшена и перемещена в правую часть экрана.
8. В Robot Runner стал доступен запуск робота со второй версией ядра. Выбрать ядро можно в окне создания задачи на вкладке **Общие** в параметре **Ядро**. Использование второй версии позволяет ускорить загрузку процессов и повысить скорость выполнения проекта роботом.
9. [В панели **Вывод**](https://docs.primo-rpa.ru/primo-rpa/primo-studio/process/debug#panel-vyvod) появилась функция, позволяющая получить полное значение переменной для его просмотра. Функция может понадобиться в случае, если значение переменной вывода слишком большое и отображается в усеченном виде. Полная загрузка значения теперь доступна в окне просмотра по кнопке **Получить целиком**. 
10. При отладке стало возможным копировать текущие значения переменных в буфер обмена. Копирование доступно из панелей [**Переменные** и **Наблюдение**](https://docs.primo-rpa.ru/primo-rpa/primo-studio/process/debug#znacheniya-peremennykh) по команде контекстного меню либо комбинацией клавиш `Ctrl` + `C`. Значения переменных попадают в буфер обмена в виде текста. Структурированные данные сериализуются в JSON-формат и также становятся доступны в текстовом виде.
11. [В разделе импорта проектов](https://docs.primo-rpa.ru/primo-rpa/primo-studio/tools/import#zapusk-importa) появилась настройка **Импортировать переменную ForEach виртуально**. Включение параметра помогает избежать ситуации, когда при импорте проекта виртуальная переменная в цикле For Each замещается локальной.
12. В элементе [**Получить текст (SAP)**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/els_sap/el_sap_gettext) появилось свойство **Обрезка**, которое удаляет ненужные пробелы в начале и/или в конце текста, добавляемые к нему при чтении. Выбрать, какие пробелы нужно удалить, можно в значениях свойства.
13. В элементах [**Объект к XML**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/els_data/els_data_xml/el_data_xml_toxml) и [**Объект к JSON**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/els_data/els_data_json/el_data_json_tojson) добавлена функция форматирования строки с результатом. Отформатированные данные отображаются с отступами, что облегчает их восприятие. Функция опциональна.
14. Добавлен элемент [**Создать таблицу**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/prilozhenie-excel/el_excel_createtable) в разделе работы с Excel. Поскольку созданная таблица фактически будет представлять собой именованный диапазон данных, это расширяет сценарии взаимодействия с ними. Например, к такой таблице возможно обращаться в запросах ODBC SQL, совершать выборки, составлять отчеты из нескольких таблиц и т.п.
15. В элементе [**Запись диапазона** (Excel)](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/prilozhenie-excel/el_excel_writerange) добавилось свойство **Строгая типизация**, которое применяется по умолчанию. Настройка позволяет решить проблему неопределенности типа записанных данных. При строгой типизации изначальный тип данных будет сохранен при записи в таблицу. 
16. Элемент [**Сохранить документ**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/els_excel/el_excel_save) стал поддерживать сохранение Excel-файлов с раширением XLSB. 
17. В элементе [**Переместить в папку (Exchange)**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/els_mail/els_exchange/el_move) добавилось свойство **Общий ящик**, использование которого позволяет перемещать письма внутри общего почтового ящика. 
18. В окне [**Поиск** (Ctrl+F)](https://docs.primo-rpa.ru/primo-rpa/primo-studio/projects/search) стало возможным включать отображение столбцов **ID элемента** и **Номер** в таблице результатов. Отображение колонок настраивается в контекстном меню таблицы по команде **Показать выбор колонок**. По умолчанию эти столбцы не отображаются. 
19. Добавлена возможность [переименовывать аргумент](https://docs.primo-rpa.ru/primo-rpa/primo-studio/process/variables#redaktirovanie-argumenta) для всего процесса, где он используется. Для этого на панели **Аргументы** добавлена соответствующая кнопка.
20. В элементе [**Switch**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/els_logic/el_logic_switch) добавлено окно подтверждения при удалении случая. Это сделано для предотвращения потери данных при случайном нажатии.


## Исправленные ошибки
1. В шаблонах поиска исправлена некорректная обработка многострочного текста. Ранее переносы в таком тексте обрабатывались неправильно, из-за чего приходилось для каждой отдельной строки ставить символ `*` в шаблоне. Теперь поиск многострочного текста производится корректно, достаточно одного символа `*` для всех строк. 
1. При возникновении исключения в WorkflowController.Execute() робот, запущенный из Оркестратора, переставал реагировать. Ошибка была связана с неправильным сценарием использования проектов с аргументами, значение которых нужно было получить из Оркестратора. Поскольку аргументы привязываются к заданию, ручной запуск таких проектов (без задания) приводил к зависанию робота. Ошибка исправлена, ручной запуск таких проектов из Оркестратора стал запрещен.
1. В Robot Runner'е невозможно было запустить проект из Оркестратора, если выбран тенант не по умолчанию. Теперь проекты из других тенантов запускаются, и ошибки не возникает. При этом выбор проекта осуществляется только в рамках указанного тенанта, что является корректным поведением.
1. При указании в **Цикле ForEach** переменной с типом данных JToken/JObject проверка синтаксиса выводила предупреждение о том, что такого класса нет. Теперь при назначении типа данных отображается его полное имя, и ошибки не возникает.
1. В некоторых ситуациях при повторном редактировании шаблона поиска не сохранялись внесенные изменения. Ошибка исправлена.
1. Исправлена ошибка фильтрации элементов по слову *image* в интерфейсе на английском языке. Ранее фильтрация по искомому слову не производилась, отображался полный список элементов. С этой версии фильтрация осуществляется корректно, в том числе на уровне вывода всех дочерних элементов узла, содержащего искомую подстроку.
1. В процессе с типом **Только код** не работал элемент **Чтение теста (PDF)**: текстовые данные файла не считывались. Теперь элемент выполняется корректно.
1. В окне **Поиск** (Ctrl+F) не работал переход к найденному элементу в диаграммах. С этой версии переход к элементу в диаграммах возможен.
1. При выполнении элемента **Перетаскивание** (Работа с UI) возникала ошибка таймаута: неправильно обрабатывались координаты. Ошибка исправлена.
1. При использовании в процессе нескольких элементов **Клик изображения мышью** подряд возникала ошибка таймаута. Причина заключалась в потере значения у переменной System.Drawing.Bitmap. С этой версии элементы выполняются корректно.
1. Исправлена ошибка при работе с Git, которая возникала при попытке сделать pull из удаленного репозитория.
1. Исправлено ошибочное закрытие Студии, которое возникало при отмене выбора проекта в начале работы с приложением. 
1. В окне Студии пропадало меню быстрых действий (*Создать проект, Открыть...* и т.д.) при закрытия проекта. Теперь просмотр меню доступен.
1. Во время отладки не разворачивалось окно Студии при срабатывании точки останова в процессе. С этой версии оно разворачивается.
1. После установки дистрибутива Primo.Robot версии 23.2 в русской инсталляции у Robot Runner'a отображалось неправильное название ярлыка. Ошибка в наименовании исправлена.
1. При попытке создания библиотеки без открытого проекта появлялась ошибка. Теперь ошибки не возникает, пользователь возвращается в главное окно Студии.
1. Исправлена ошибка, возникавшая при отладке, которая приводила к повторному выполнению элемента с точкой останова.
1. В некоторых случаях при отправке ответа на письмо с помощью элемента **Отправить сообщение** (Exchange) возникала ошибка с сообщением, что письмо устарело. Также при ответе ошибочно удалялся текст предыдущего письма. Обе ошибки исправлены. 
1. Исправлена ошибка, возникавшая при сохранении Excel-файла как PDF: сохранялась только первая страница. Теперь сохраняются все страницы.