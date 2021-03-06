# Backend сервиса "После уроков"

"После уроков" - сервис, предоставляющий возможность организациям дополнительного образования 
организовать систему информирования родителей и классных руководителей учеников
об их успеваемости и интересах, интересных для них событиях. 

## Описание модуля

Backend сервиса представляет из себя REST API, реализованное с помощью headless cms 
[Directus](https://docs.directus.io/getting-started/introduction/)

На данном этапе были созданы соответствующие сущности, необходимые для работы сервиса:

1) Child - профиль ребёнка
2) Section - профиль секции (хранит в себе соответствующий id сообщества vk + дополнительную информацию, 
необходимую для поддержания работы рекомендательной системы)
3) Group - профиль группы (хранит в себе соответствующий id сообщества vk + доп. информацию)
4) Tags - создаваемые пользователями теги для секций/групп/мероприятия
5) MasterPlan - стандартный сборник целей для секции, на основе которого

... *Нужно дописать*

## Дополнительные модули 

1. [Модуль авторизации](https://github.com/SemBystrov/posle_urokov_auth-adapter)

*Необходим для реализации сценария подтверждения прав на действия с данными, между directus и vk mini app* 

2. [Рекомендательная система](https://github.com/naignatiev/posle_urokov_tags)

*Рекомендательная система, обслуживающая сервис*
