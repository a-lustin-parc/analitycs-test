Раздел "Биллинг"
Просмотр списка счетов
В списке отображаются счета по всем делам, которые доступны пользователю. 

В списке счета сгруппированы по клиенту. 

Счета без клиентов сгруппированы в группу "Неизвестный клиент"

Список отсортирован по имени участника, а затем по названию дела.

Список отсортирован по названию участника в порядке 0-9, A-Z, А-Я, а затем по названию дела в том же порядке.

В списке счетов отображаются следующие данные:

Название
Формат данных
Примечание
ID / ID	текст	ссылка на карточку счета 
Срок / Due In	 число дней	
Считается как значение поля Срок оплаты в счете минус текущая дата.

Если значение меньше 0, то отображается 0.

Если не указано значение поля Срок оплаты, то отображается " — "

Слово "дней" должно склоняться.

Дата создания / Issued On	дата	в формате чч Мес гггг
Статус / Status	текст	 
Оплачено / Paid Amount	число	
Если не указано, то отображаем 0.

Если число дробное, то отображается 2 знака после запятой.

Сумма счета / Bill Amount	число	Если число дробное, то отображается 2 знака после запятой.
Символ валюты счета	 	 
Просмотр задолженностей клиентов
В списке отображаются дела, в которых есть активности и затраты не учтенные в счете. 

Дела сгруппированы по заказчику. 

Список дел отсортирован по названию дела в порядке 0-9, A-Z, А-Я.

В списке отображается следующая информация:

Название
Формат данных
Примечание
Название дела	ссылка	 
Затраченное время	чч мм	 
Сумма к оплате	число	Сумма = активности + затраты
Счета
Основная информация
Основная информация счета содержит следующие данные:

Название
Формат данных
Обязательность
Примечание
Название клиента	
Для физ. лица:
Фамилия Имя

Для организации:
Название организации 

Да	
Если клиент был удален из системы, то счет открывается, поле Название клиента — пустое.

Если поле Заказчик в деле было очищено, то в ранее созданных счетах поле "Название клиента" не изменяется.

Если поле Заказчик в деле было изменено, то в ранее созданных счетах поле "Название клиента" не изменяется.

ID	 	Да	 
Статус	
Черновик (Draft)
На утверждении (Pending Approval)
Выставлен (Awaiting Payment)
Оплачен (Paid)
Да	
По умолчанию новый счет создается со статусом Draft.

 

Дата счета	 	Да	 
Срок оплаты	Дата в формате чч.мм.гггг	 	Срок оплаты = дата создания счета + 30 дней
Скидка	
Проценты / Percent
Число / Number
 	Положительное число. Может быть дробным. Округление в большую сторону до 2х знаков после запятой
Основной налог	число	 	Положительное число. Может быть дробным. Округление в большую сторону до 2х знаков после запятой
Второй налог	число	 	Положительное число. Может быть дробным. Округление в большую сторону до 2х знаков после запятой
Способ расчета второго налога	
С учетом основного налога / Apply to post-tax amount
Без учета основного налога / Apply to pre-tax amount
 	 
 

Включенные/Не включенные затраты

Помимо основной информации счет содержит данные о включенных в счет Логах и Расходах:

Название
Формат данных
Примечание
Дата	 ЧЧ МММ ГГГГ	 
Тип	Затраты
Лог 	 
Описание	
Для затрат:
Название затраты

Для Лога:
Тип активности 

Если затраты или активность были включены в счет, после этого удалены, то они счет не изменяется.

Если исключить из счета удаленные затраты, то они удаляются из счета.

Если активность или затрата не включена в счет, то при удалении, она удаляется из счета.

Активности и затраты включенные и не включенные в счет должны быть кликабельны.

По клику открывается попап затраты или сущности, по которой указано затраченное время.

Если в попапе сущности внесены изменения, то после сохранения, обновляется страница.

Пользователь	Пользователь добавивший лог или расход	 
Налог 1	Логическое значение	 
Налог 2	Логическое значение	 
Время	Формат Nч Mч	 
Тип ставки	
Фиксированная
Почасовая
По умолчанию устанавливается "Почасовая".
Ставка	Положительно целое число	
Ставка указывается в Настройках биллинга.

Если в счете изменена ставка активности/затраты (отличается от указанной в настройке биллинга) и эту активность/затрату исключают из счета, то значение ставки устанавливается в соответствии с настройками биллинга.

Если в настройках не указана ставка, то отображается ноль.

Тип скидки строки	
Процент
Сумма
 
Скидка строки	Положительно целое число	 
Просмотр списка включенных логов и затрат в счете:

Название
Формат данных
Примечание
Дата	ДД МММ ГГГГ	 
Описание 	
Для затрат:
Название затраты

Для Лога:
Тип активности 

 
Инициалы пользователя	 	 
Налог 1	Логическое значение	 
Налог 2	Логическое значение	 
Время	Формат Nч Mч
Если в строке затраты, то "—"	 
Ставка	
Фиксированная
Почасовая
 
Скидка строки	Положительно целое число	 
К оплате	 	 
Также в счете отображаются не включенные активности и затраты:

Название
Формат данных
Примечание
Дата	дд ммм гггг	 
Описание	
Для затрат:
Название затраты

Для Лога:
Тип активности 

 
Время	Формат Nч Mч
Если в строке затраты, то "—"	 
Ставка	число	 
К оплате	число	 
 

К оплате = СуммаСтроки - СкидкаСтроки + Налог 1 + Налог 2

Если ставка почасовая, то:
СуммаСтроки = ( Время * Ставка )

Если ставка фиксированная, то:
СуммаСтроки = (Ставка)

Налоги прибавляется только в случае, если напротив строки проставлена пометка Налог 1 или Налог 2

 

Расчет Налога 1:

Расчет ведется построчно. То есть все значения берутся построчно.

Налог 1 считается только для строк, в которых стоит пометка о расчете Налога 1

Сумма Налога 1 = (СуммаСтроки - СкидкаСтроки) * Налог 1 / 100

Расчет Налога 2:

Расчет ведется построчно. То есть все значения берутся построчно.

Налог 2 считается только для строк, в которых стоит пометка о расчете Налога 2.

Налог 2 имеет 2 варианта расчета, в зависимости от настроек, которые указаны были при создании счета, а именно:

Apply to post-tax amount
Apply to pre-tax amount
Дальнейшие изменения общих настроек биллинга не влияют на способ расчета в конкретном счете после его создания.

Если при создании счета стояла настройка "Apply to post-tax amount", то расчет следующий:

Сумма Налога 2 = ((СуммаСтроки - СкидкаСтроки) + Налог 1) * Налог 2 / 100

Если при создании счета стояла настройка "Apply to post-tax amount", то расчет следующий:

Сумма Налога 2 = (СуммаСтроки - СкидкаСтроки) * Налог 2 / 100


Расчет итогов
Название
Формат данных 
Примечание 
Сумма затрат 	(СуммаСтроки - СкидкаСтроки) всех строк	 
Скидка	Если скидка в %, то считаем то считаем:
Сумма затрат * Скидка / 100
Если скидка в числовом выражении, то просто отображаем размер скидки.	это размер скидки указанной в основных параметрах счета
Налог	Сумма Налог 1 и Налог 2 по каждой строке, в которой необходимо их рассчитать	 
К оплате	Сумма значений "К оплате" по каждой строке - общая скидка счета	Положительное число. Округление в большую сторону до 2х знаков после запятой
Создание, изменение счета

Создание карточки счета доступно из раздела "Счета" карточки дела и из раздела Просмотр списка задолженностей.

При создании счета в счет попадают все активности и затраты не включенные в другие счета. 

При создании счета отображается лоадер.

Счет открывается в новой вкладке.

Создание счета доступно только при правах Изменение на раздел Биллинг. 

Если не указан Заказчик в деле, то при попытке создать счет, отображается сообщение с желтой иконкой:

Обратите внимание
Для создания счета необходимо указать заказчика в деле

Pay your attention
To create a bill you must specify the client

Payer votre attention
Pour créer une facture, vous devez spécifier le client

Если в деле активности или затраты не включенные в счет, то при попытке создать счет отображается сообщение с желтой иконкой:

Обратите внимание
Для создания счета в деле должны быть активности или затраты не включенные в другие счета.

Pay your attention
To create invoice must be activities or expenses not included in other invoice.

Payer votre attention
Pour créer une facture doivent être des activités ou des frais non compris dans d'autres de la facture.

Редактирование счета доступно только при правах Изменение на раздел Биллинг. 

Для редактирования доступны следующие данные счета: 

Название
Примечание
ID	 
Статус	 
Дата счета	 
Срок оплаты	 
Дата оплаты	 
Скидка	
 

Основной налог	 
Второй налог	 
Способ расчета второго налога	 
Оплачено	 
Набор активностей и затрат, входящие в счет	 
Платежи
Просмотр списка
Также в счете отображается записи о платежах по этому счету.

В списке содержатся платежи, по данному счету.

Список отсортирован по дате платежа. Новые — сверху.

Если в списке нет платежей, то отображается заглушка "Платежей пока нет"

В списке отображаются следующие данные:

Название
Формат данных
Примечание
Дата платежа	
ЧЧ МММ ГГГГ

 
Источник платежа	Справочники Источник платежа	 
Банковский счет	Список счетов	 
Сумма	число	
Рассчитывается как Общая сумма счета - сумма платежей.

Не может быть отрицательной.

Валюта	Символ	
Unable to render JIRA issues macro, execution error.	Отображение валюты будет сделана в рамках этой задачи
Всего оплачено	число	сумма по всем платежам
Остаток	число	Разность между суммой в счете и суммой по всем платежам.
Создание, изменение платежа
Добавление нового платежа доступно из списка, с помощью "Добавить платеж".

Новая платеж добавляется сверху.

Для добавление платежа необходимо указать следующие поля:

Название
Формат
Обязательность
Примечание
Дата платежа	ЧЧ МММ ГГГГ	Да	По умолчанию подставляется текущая дата
Источник платежа	Справочник Источник платежа	Да	Если удаляется используемое значение в платеже, то платеж отображается с пустым полем. При следующем редактировании платежа должна срабатывать валидация, т.к. поле является обязательным.
Банковский счет	Список счетов	Да	 
Сумма	число	Да	
По умолчанию рассчитывается и подставляется.

Рассчитывается как Общая сумма счета - сумма платежей.

Для редактирования доступно любое поле в созданном платеже. 

Удаление платежа
Удаление платежа доступно из списка.

Для удаления необходимо подтверждение. 

В результате успешного удаления отображается нотификация об успешном удалении.

Добавление, изменение, удаление платежа доступны вне зависимости от статуса счета.

Права
Создание, изменение, удаление платежей доступно при правах редактирование, Администрирование на дело, и при правах Изменение на биллинг. 

С каждым счетом из списка доступны следующие действия:Действия со счетами
Скачать
Удалить
Изменить статус
Распечатать
Из карточки счета доступны действия со счетом:

удалить
Счета в статусе Ожидает оплаты и Оплачен невозможно удалить.

Предпросмотр счета
Превью счета доступно на отдельном табе в карточке счета.

По умолчанию установлен не удаляемый "Стандартный шаблон счета".

В превью можно выбрать ранее созданные шаблоны для отображения счета.

Во время формирования счета должен отображаться лоадер. 

В списке шаблонов отображаются только шаблоны для счета. 

Список шаблонов отсортирован по алфавиту в порядке 0-9, A-Z, А-Я.

Список отображается с паджинацией по 20 записей.

Для каждого счета сохраняется последний выбранный шаблон счета. 

Если в настройках аккаунта не указана валюта, то счет отображается без валюты.

Загрузка счета
Сохранение счета доступно из карточки счета.

Счет сохраняется в формате docx.

Имя файла по умолчанию - Счет №[номер счета] от [дата создания в формате чч.мм.гггг].

(Bill #[номер счета]_[дата создания в формате чч.мм.гггг - английский)

(Facture #[номер счета]_[дата создания в формате чч.мм.гггг - французский)

Файл сохраняется с учетом выбранного шаблона. 

Отправка по email
Функция позволяет отправлять счет по email.

Функция доступна в общем разделе Биллинг,в карточке счета и в карточке дела в разделе Счета. 

Счет можно отправить:

в любом статусе
без заказчика
При отправке счета отображается форма отправки email Send & Receive Email

При отправке к email прикладывается счет в формате pdf с учетом выбранного шаблона. 

Для отправки счета необходимо указать email получателя. 

В результате успешной отправки отображается нотификация

Счет отправлен.

Invoice sent

Функция доступна при правах любых правах на Биллинг.

При отправке счета по email событие в ленте не генерируется

Автонумерация счета
Номер счета состоит из шаблона и порядкового номера.

Шаблон это все, все окружает порядковый номер.

Примеры шаблона и порядкового номера:

2017/1 — [2017/] 1

ГОСТ34 — [ГОСТ] 34

ЕГЭ1ПРСТ — [ЕГЭ] 1 [ПРСТ]

Новый шаблон применяется после изменения номера последнего созданного счета.

Порядковый номер формируется инкрементом к максимальному порядковому номеру с последним актуальным шаблоном.

Порядковый номер определяется путем поиска комбинации последовательных цифр с конца номера счета.

Последний актуальный шаблон содержится в последнем созданном счете.

Если в номере счета нет порядкового номера, то при следующем создании алгоритм создаст в конце шаблона добавит порядковый номер 1.

Номер счета является уникальным значением. Если пользователь вводит номер, который уже существует, ему отображается сообщение:

Измените номер счета
Введенный номер счета уже присвоен одному из ранее созданных счетов. Пожалуйста, введите другой номер счета.

Change invoice id
Entered invoice number have been added to another invoice. Please, enter another invoice number

Если инкрементный номер счета превышает значение 2147483647, то отображается сообщение:

Ошибка при создании счета

Невозможно создать счет с номером превышающим значение 2147483647. Пожалуйста, введите другой номер счета или удалите предыдущий счет

Error creating invoice

Unable to create invoice with a number more than 2147483647. Please enter another invoice number or delete the previous invoice.

Печать счета
Функция позволяет распечатать счет.

Функция доступна из списка счетов и из карточки счета. 

В результате работы функции генерируется pdf файл, который открывается в новой вкладке с диалогом на сохранение.

Файл генерируется на основании используемого шаблона счета. 

Фукнция доступна при правах Только просмотр, Изменения на раздел Биллинг.

Групповые операции со счетом
Функция доступна из общего раздела Billing и раздела Invoice карточки дела.

Групповые операции со счетами:

удаление
изменение статусов
загрузка счетов
New Feature	
Групповая загрузка счетов
Функция позволяет загрузить архив с печатными версиями счетов в формате .docx

В результате работы функции пользователь загружается .zip архив с .docx версиями документов. 

Название архива — Invoice from CASE.ONE/CASE.PRO

Функция доступна пользователям с правами на просмотр и выше в разделе "Биллинг".

Групповое изменение статусов
Функция позволяет сменить статус нескольких счетов одновременно.

Функция доступна из раздела Billing и раздела Invoices в карточке дела.

Для работы функции необходимо выбрать 1 и более счетов, и затем выбрать один из статусов для замены. Для выбора доступны все имеющиеся статусы:

Draft
Awaiting Payments
Pending Approval
Paid
В результате работы функции изменяются статусы счетов на выбранный. 

Функция доступна пользователям с правами на редактирование/изменение в разделе "Биллинг"

Если на дело одного из выбранных счетов права Просмотр, Комментирование, то при попытке изменить статус отображается сообщение:

"Недостаточно прав для изменение статуса счетов: [номер счета1], [номер счета2]" 
"Not enough rights to change the status of bills: [номер счета1], [номер счета2]"  

CASEM-23053 - Change "bills, bill" in notification for Invoices Batch Status changing ( Open)	
В зависимости от количества счетов должно измениться "счетов, счета", "bills, bill".

Групповая печать счетов
Функция позволяет распечатать выбранные счета. 

Функция доступна при выборе хотя бы одного счета.

Функция доступна в:

разделе Счета в карточке 
в групповых операциях в списке счетов (кроме "Оплачиваемые клиенты"
в групповых операциях в каждой группе счетов.
В результате работы функции генерируется pdf файл, который открывается в новой вкладке с диалогом сохранения.

Название файла, в которых сохраняется сгенерированный pdf — Cases_[текущая дата] (с учетом настроек локализации)

В pdf файле каждый счет начинается с новой страницы. 

Печатная форма для каждого счета должна генерироваться с учетом выбранного шаблона.

Функция должна позволять одновременно печатать 150 счетов, суммарный размер pdf файла — 30 Мб.

Функция доступна при правах Только просмотр или Изменение на раздел Биллинг. 

Групповое удаление счетов
Функция позволяет удалять 1 и более счетов.

Для работы функции необходимо выбрать несколько счетов в списке

В результате операции группового удаления, отображается нотификация с результатом.

Удалить можно счет в любом статусе, кроме Ожидает оплаты и Оплачен.

При попытке удалить счета в статусе Ожидает оплаты или Оплачен отображается сообщение "You cannot delete invoice in the status of  Awaiting Payment or Paid".

Если операция выполнена успешно, то счета удаляются и более не отображаются в списке счетов.

Функция доступна пользователям с правами на редактирование/изменение в разделе "Биллинг".

Групповая отправка счетов
Функция позволяет отправлять по email более одного счета за раз. Доступна отправка как счетов одного блока, так и счетов из разных блоков. 

При отправке нескольких счетов одному клиенту каждый счет отправляется отдельным файлом.

При этом каждый счет в файле начинается с новой страницы. 

Функция доступна в карточке дела в разделе Счета и в общем разделе Биллинг. 

При отправке нескольких счетов, первой страницей добавляется страница с общей информацией по счетам.  

Название файла — Invoices_[текущая дата]. Текущая дата отображается с учетом НЛ.

Как должна выглядеть страница с общей информацией — Invoices summary page.docx

На странице выводятся общая информацию и данные по счетам.

Общая информация документа содержит следующие данные:

Название
Формат
Примечание
Дата отправки	дата	зависит от настройки даты
Название клиента	текст	
Для компании — название компании

Для физ лица — Фамилия Имя

Информация о счетах содержит следующие данные:

Название
Формат
Примечание
Дата создания счета	Дата	Отображается в соответствии с настройками локализации дат
Название дела	Текст	 
Номер счета	Текст	 
Сумма к оплате	
Дробное число

2 знака после запятой

Зависит от настроек локализации чисел 

Отображается с валютой

Сумма счета

Оплаченная сумма	
Дробное число

2 знака после запятой

Зависит от настроек локализации чисел 

Отображается с валютой

Сумма всех платежей по счету.

Неоплаченная сумма	
Дробное число

2 знака после запятой

Зависит от настроек локализации чисел 

Отображается с валютой

Разность между суммой счета и суммой всех платежей в счете.

Может быть отрицательной

Общая сумма	
Дробное число

2 знака после запятой

Зависит от настроек локализации чисел

Отображается с валютой

Сумма всех сумм счетов.

Общая оплаченная сумма	
Дробное число

2 знака после запятой

Зависит от настроек локализации чисел 

Отображается с валютой

Сумма всех платежей по всем счетам

Общая не оплаченная сумма	
Дробное число

2 знака после запятой

Зависит от настроек локализации чисел.

 Отображается с валютой.

Разность между "Общая оплаченная сумма" и "Общая не оплаченная сумма".

Может быть отрицательной.

Если список счетов занимает на странице с общей информацией по счетам занимает более одной страницы, то на каждой следующей отображается заголовок таблицы. 

Письма отправляются с почты, настроенной у данного пользователя, если пользователь не настроил ни одну из почт, то перед отправкой необходимо отобразить форму настройки почты.

В качестве адреса получателя используется email Участника, указанного в качестве Клиента в счете. 

Если хотя бы у одного участника не указан email, то перед отправкой писем, открывается форма для ввода email.

В форме указаны только уникальные участники, у которых не указан email. 

При вводе отсутствующих email осуществляется валидация email.

Если указанный email не валидный, то отображается сообщение "Некорректный email". 

После указания email каждому участнику, email добавляется в карточку участника. 

Указание email не обязательный шаг, который можно пропустить. 

Пользователь может:

Пропустить этот шаг по кнопке, тогда никакие данные не учитываются, отправляются счета, только участникам, у которых указан email.
Заполнить email всех участников, у которых не были указан email, в этом случае также счета отправляются всем участникам, указанные email добавляются в карточку участника в поле email. 
Заполнить email не всех участников, тогда отображается сообщение, и счета отправляются только пользователям, у которых указан email.
Cчета не будут отправлены
У нескольких клиентов не указан email, поэтому им не будут отправлены счета.  

Далее пользователю необходимо указать:

Название
Обязательность
Примечание
Subject	да	по умолчанию — пустое
Body	да	по умолчанию — пустое
По каждому Заказчику формируется отдельное письмо с указанными Subject и Body и приложенный счетом. 

Счет — в формате pdf, сформированный с учетом выбранного шаблона.  

После успешной отправки email отображается сообщение:

Счета отправлены

Если среди отправляемых счетов, есть счета, в которых не указан Заказчик, то все счета отправляются, кроме тех, у которых не указан Заказчик, отображается сообщение:

Some invoices not sent
Some invoices have not been sent. Please specify the Billable Client in these invoices and try again: [номер счета 1], [номер счета 2]

Если пользователь отправляет письма для заказчиков, ни у одного из которых не указана почта, и пользователь не указывает ни одну почту, то счета не отправляются, отображается сообщение "Invoices not sent"

Во время отправки отображается лоадер.

Если счета были отправлены, то необходимо для каждого счета записать следующие параметры:

дата и время отправки
id пользователя, отправившего счет
Если выбран один счет, то используется функциональность Invoice Emailing.

Права
Icon
Изменение было в рамках стори Unable to render JIRA issues macro, execution error. и бага Unable to render JIRA issues macro, execution error.

Добавился расчет прав на счета в деле в зависимости от прав на раздел Биллинг и прав на дело, также учитывая архивность дела.

Для одного счета
При выполнении хотя бы одного пункта:

права на дело Просмотр
права на дело Комментирование
дело в архиве
доступные функции для счетов во вкладке Счета в деле:

Отправить по электронной почте
Распечатать. 
Недоступные пункты меню:

Сменить статус (функции Отправить на утверждение, Отправить на оплату, Переоткрыть, Оплачено клиентом)
Удалить
Для групповых операций со счетами
Если хотя бы на один счет в группе счетов есть права на редактирование, то отображаются все пункты меню, но функция применяется только к тем счетам, на которые есть права на редактирование. 
