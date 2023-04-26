# Создать таблицу

![](<../../../.gitbook/assets/image (100) (1) (1) (1) (1) (1) (1) (10) (177).png>)

![](<../../../.gitbook/assets/excel-create-table.png>)

Компонент создает таблицу на заданном листе Excel. Не забудьте сохранить готовую таблицу с помощью элемента [**Сохранить документ**](https://docs.primo-rpa.ru/primo-rpa/g_elements/el_basic/prilozhenie-excel/el_excel_save) (Excel).

## Свойства

Все свойства элемента разделены на группы - они выделены в таблице жирным курсивом.

| Свойство                | Тип                                  | Описание           | 
| ----------------------- | ------------------------------------ | ------------------ |
| ***Общие***  | | Описание общих свойств см. в разделе [Свойства элемента](https://docs.primo-rpa.ru/primo-rpa/primo-studio/process/elements#svoistva-elementa) | 
| ***Excel***  | | | 
| Диапазон                | String                               | Диапазон таблицы. Пример: `"A1:D12"` |
| Наименование            | String                               | Наименование будущей таблицы |
| Страница                | String                               | Наименование страницы        |
| Индекс страницы         | Int32                                | Индекс страницы, отсчет с 0  |