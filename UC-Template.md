# Отображение превью в ссылке

**Акторы:** 

- пользователь
- мессенджер (система)

**Цель:** как пользователь, я хочу видеть содержимое (заголовок, описание, главное изображение, адрес) ссылки, чтобы экономить время, не открывая ее в браузере

**Предусловия:** 
1. Пользователь должен быть подключен к интернету 
2. На устройстве пользователя в настройках включен режим предпросмотра

**Сценарий:**

Пользователь видит превью в ссылке, введя URL в поле ввода сообщения 
Бэкенд возвращает содержимое ссылки (заголовок, описание, главное изображение, адрес) ссылки до ее откытия

**Результат:**

отображение сообщения с ссылкой с превью 
- Список значимых результатов сценария.
- В базу данных добавлен новый чат.

**Исключения:**

Если нет подключения к интернету, показывается ошибка 
Если на устройстве пользователя не включен режим предпросмотра, превью не будет показано

**Альтернативный сценарий:** 

Пользователь удаляет превью после ввода URL, нажав на × (крестик). 



# Отправка отложенных сообщений

**Акторы:** 
- пользователь
- мессенджер (система)

**Цель:** как пользователь, я хочу отправлять отложенные сообщения, чтобы сообщение отправлялось в указанное время

**Предусловия:** 
Созданный чат

**Сценарий:**
1. Пользователь зажимает кнопку «Отправить»
2. Выбирает «Отложенное сообщение»
3. Выставляет таймер, чтобы сообщение отправилось в указанное время 
Бэкенд возвращает уведомление об отправке сообщения в указанное время

**Результат:**
В базу данных добавлено отложенное сообщение 

**Исключения:**


**Альтернативный сценарий:** 

Если пользователь в указанное в таймере время не подключен к сети, то сообщение отправится при подключении к сети
