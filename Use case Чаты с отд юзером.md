@startuml
left to right direction
skinparam usecase {
 BackgroundColor Lightgreen
 FontColor Black
}
:авторизованный user: as u
rectangle Чаты {
(Поиск по чатам и каналам)
(Создавать групповые чаты)
(Создавать каналы)
(Архивировать чаты)

rectangle Чат_с_отдельным_пользователем {
(Отправлять/Получать сообщения)
(Удалять отправленные сообщения)
(Редактировать отправленные сообщения)
(Отправлять медиа-файлы)
(Закрепить/открепить сообщение)
(Открыть информацию о пользователе)
(Посмотреть вложенные файлы)
(Добавить пользователя в черный список)
(Поиск по чату)
(Позвонить пользователю)
(Скопировать данные о пользователе) 

(Отправлять/Получать сообщения)..>(Отправлять медиа-файлы):расширяет
(Отправлять/Получать сообщения)..>(Редактировать отправленные сообщения):расширяет
(Отправлять/Получать сообщения)..>(Удалять отправленные сообщения):расширяет
(Отправлять/Получать сообщения)..>(Закрепить/открепить сообщение):расширяет
(Отправлять/Получать сообщения)..>(Поиск по чату):расширяет
(Открыть информацию о пользователе)..>(Посмотреть вложенные файлы) :расширяет
(Открыть информацию о пользователе)..>(Скопировать данные о пользователе) :расширяет
(Открыть информацию о пользователе)..>(Позвонить пользователю) :расширяет
(Открыть информацию о пользователе)..>(Добавить пользователя в черный список) :расширяет 

u--(Поиск по чатам и каналам)
u--(Создавать групповые чаты)
u--(Создавать каналы)
u--(Архивировать чаты)
u--(Отправлять/Получать сообщения)
u--(Открыть информацию о пользователе)


@enduml