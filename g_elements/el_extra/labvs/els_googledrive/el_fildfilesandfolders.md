# Поиск файлов и папок

![](<../../../../.gitbook/assets/image (471) (1) (2) (1).png>)

Элемент, осуществляющий поиск файлов и папок

| Свойство    | Тип                                   | Описание                                                                                                |
| ----------- | ------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| Запрос      | String                                | Поисковый запрос (name = 'testfile') - 'https://developers.google.com/drive/api/v3/reference/query-ref' |
| Кол-во      | Int32                                 | Максимальное кол-во результатов                                                                         |
| Общий диск  |                                       | Поддержка общих дисков                                                                                  |
| Файлы       | List\<Google.Apis.Drive.v3.Data.File> | Массив найденных файлов                                                                                 |
| Первый файл | Google.Apis.Drive.v3.Data.File        | Первый найденный файл                                                                                   |
