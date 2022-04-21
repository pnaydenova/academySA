@startuml
left to right direction
skinparam usecase {
 BackgroundColor Lightgreen
 FontColor Black
}

:автризованный user: as u

rectangle Telegram {
 (Добавить контакты) as dk
(Редактировать личные данные) as rld
(Найти другого пользователя) as find
(Отправить сообщение другому пользователю) as write
(Позвонить другому пользователю) as call
(Получать сообщения от других пользователей) as get
(Создавать групповые чаты) as creategroup
(Создавать каналы) as createch
}

u--dk
u--rld
u--find
u--write
u--call
u--get
u--createch
u--creategroup

@enduml