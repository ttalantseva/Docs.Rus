# Регистрация RDP-пользователей на машине Робота
RDP-пользователей, созданных в AD или локально на машине Робота, можно зарегистрировать в Оркестраторе. Регистрацию выполняет администратор или администратор тенанта.

Для этого требуется перейти в раздел **Настройки > Машины роботов**, выделить нужную машину и нажать кнопку **Все RDP-пользователи**. На открывшейся странице нажмите **Добавить RDP-пользователя**:

![](<../../.gitbook/assets/rdp-users-tab.png>)

См. также раздел [Привязка RDP-пользователя к Роботу](https://docs.primo-rpa.ru/primo-rpa/orchestrator/basics/assign-rdp).

Для Робота, привязанного к RDP-пользователю, RDP-сессия открывается автоматически при старте Робота. Чтобы сессия также автоматически закрылась после выполнения Роботом RDP-проекта, на форме создания/редактирования RPA-проекта нужно включить чекбокс **После выполнения проекта роботом закрыть RDP-сессию**.