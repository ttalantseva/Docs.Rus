# Ввод текста

![](<../../../.gitbook/assets/image (937).png>)

Компонент, производящий ввод текста в выбранный элемент управления.

| Свойство             | Тип                                  | Описание                                            |
| -------------------- | ------------------------------------ | --------------------------------------------------- |
| Шаблон поиска        | String                               | Шаблон поиска элемента управления                   |
| Элемент              | LTools.UIInteraction.Model.UIControl | Ссылка на элемент управления                        |
| Текст\*              | String                               | Вводимый текст                                      |
| Область              | System.Drawing.Rectangle             | Область поиска компонента                           |
| Текущий пользователь |                                      | Искать только среди процессов текущего пользователя |
| Таймаут\*            | Int32                                | Предельное время ожидания завершения процесса (мс)  |
