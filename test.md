1391499931841894891491494119491409491949194
4419418914881481484814848841818488481481481481848148481488141481848189418481948198491981518г581985915814545
Привет, Гитхаб! Здесь будет информация о первых командах из 3 семинара
> git push - отправить изменения в удаленный репозиторий 
Привет мы пробуем работу с удаленным репозиторием =)
## ИНСТРУКЦИЯ РАБОТЫ С Git
>**git init** - создание пустого репозитория в выбранной папке

>**git add** - сохранить все файлы, которые мы добавили в наш репозиторий

>**git commit** - команда git commit берёт все данные, добавленные в индекс с помощью git add, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок

>**git diff** - команда git diff используется для вычисления разницы между любыми двумя Git деревьями

>**git difftool** - команда git difftool просто запускает внешнюю утилиту сравнения для показа различий в двух деревьях, на случай если вы хотите использовать что-либо отличное от встроенного просмотрщика git diff

>**git clean** - команда git clean используется для удаления мусора из рабочего каталога. Это могут быть результаты сборки проекта или файлы конфликтов слияний

![Photo](image-2.png)

[ссылка](https://git-scm.com/book/ru/v2/Git-%D0%B8%D0%B7%D0%BD%D1%83%D1%82%D1%80%D0%B8-%D0%A1%D1%81%D1%8B%D0%BB%D0%BA%D0%B8-%D0%B2-Git)


![another photo](image.png)

[ссылка на инструкцию](https://www.bing.com/ck/a?!&&p=8d1218153ff51c7bJmltdHM9MTY5ODk2OTYwMCZpZ3VpZD0yZTZiMDkxOS1hNDg3LTZiNjgtMjY3My0xYjJiYTA4NzZkNGYmaW5zaWQ9NTQxNw&ptn=3&hsh=3&fclid=2e6b0919-a487-6b68-2673-1b2ba0876d4f&psq=git+%d0%b8%d0%bd%d1%81%d1%82%d1%80%d1%83%d0%ba%d1%86%d0%b8%d1%8f&u=a1aHR0cHM6Ly9zZWxlY3RlbC5ydS9ibG9nL3R1dG9yaWFscy9naXQtc2V0dXAtYW5kLWNvbW1vbi1jb21tYW5kcy8jOn46dGV4dD0lRDAlOTIlRDAlQjIlRDAlQjUlRDAlQjQlRDAlQjUlRDAlQkQlRDAlQjglRDAlQjUlMjAlRDAlQjIlMjBHaXQlM0ElMjAlRDAlQkQlRDAlQjAlRDElODElRDElODIlRDElODAlRDAlQkUlRDAlQjklRDAlQkElRDAlQjAlMjAlRDAlQjglMjAlRDAlQkUlRDElODElRDAlQkQlRDAlQkUlRDAlQjIlRDAlQkQlRDElOEIlRDAlQjUlMjAlRDAlQkElRDAlQkUlRDAlQkMlRDAlQjAlRDAlQkQlRDAlQjQlRDElOEIlMjAxLCVEMCVCNCVEMCVCMiVEMCVCMCUyMCVEMCVCMiVEMCVCMCVEMSU4MCVEMCVCOCVEMCVCMCVEMCVCRCVEMSU4MiVEMCVCMCUyMCVEMCVCRCVEMCVCMCVEMSU4NyVEMCVCMCVEMSU4MiVEMSU4QyUyMCVEMSU4MCVEMCVCMCVEMCVCMSVEMCVCRSVEMSU4MiVEMSU4MyUyMCVEMSU4MSUyMCVEMSU4MCVEMCVCNSVEMCVCRiVEMCVCRSVEMCVCNyVEMCVCOCVEMSU4MiVEMCVCRSVEMSU4MCVEMCVCOCVEMCVCNSVEMCVCQyUyMEdpdCUzQSUs

## Просмотр удалённых репозиториев

>Для того, чтобы просмотреть список настроенных удалённых репозиториев, вы можете запустить команду **git remote**. Она выведет названия доступных удалённых репозиториев. Если вы клонировали репозиторий, то увидите как минимум 

>**origin** — имя по умолчанию, которое Git даёт серверу, с которого производилось клонирование

## Добавление удалённых репозиториев
>В предыдущих разделах мы уже упоминали и приводили примеры добавления удалённых репозиториев, сейчас рассмотрим эту операцию подробнее. Для того, чтобы добавить удалённый репозиторий и присвоить ему имя (*shortname*), просто выполните команду **git remote add** (*shortname*) (*url*)

>Теперь вместо указания полного пути вы можете использовать *pb*. Например, если вы хотите получить изменения, которые есть у другого человека, но нету у вас, вы можете выполнить команду **git fetch pb**

## Получение изменений из удалённого репозитория — Fetch и Pull

>Как вы только что узнали, для получения данных из удалённых проектов, следует выполнить:

>*$ git fetch [remote-name]*

>Данная команда связывается с указанным удалённым проектом и забирает все те данные проекта, которых у вас ещё нет. После того как вы выполнили команду, у вас должны появиться ссылки на все ветки из этого удалённого проекта, которые вы можете просмотреть или слить в любой момент.

>Когда вы клонируете репозиторий, команда **clone** автоматически добавляет этот удалённый репозиторий под именем *«origin»*. Таким образом, **git fetch origin** извлекает все наработки, отправленные на этот сервер после того, как вы его клонировали (или получили изменения с помощью *fetch*). Важно отметить, что команда **git fetch** забирает данные в ваш локальный репозиторий, но не сливает их с какими-либо вашими наработками и не модифицирует то, над чем вы работаете в данный момент. Вам необходимо вручную слить эти данные с вашими, когда вы будете готовы.

>Если ветка настроена на отслеживание удалённой ветки, то вы можете использовать команду **git pull** чтобы автоматически получить изменения из удалённой ветки и слить их со своей текущей. Этот способ может для вас оказаться более простым или более удобным. К тому же, по умолчанию команда **git clone** автоматически настраивает вашу локальную ветку master на отслеживание удалённой ветки *master* на сервере, с которого вы клонировали репозиторий. Название веток может быть другим и зависит от ветки по умолчанию на сервере. Выполнение **git pull**, как правило, извлекает (*fetch*) данные с сервера, с которого вы изначально клонировали, и автоматически пытается слить (*merge*) их с кодом, над которым вы в данный момент работаете.

## Просмотр удалённого репозитория

>Если хотите получить побольше информации об одном из удалённых репозиториев, вы можете использовать команду **git remote show** *remote*

>Она выдаёт URL удалённого репозитория, а также информацию об отслеживаемых ветках. Эта команда любезно сообщает вам, что если вы, находясь на ветке *master*, выполните **git pull**, ветка *master* с удалённого сервера будет автоматически влита в вашу сразу после получения всех необходимых данных. Она также выдаёт список всех полученных ею ссылок

>**git remote show** - Данная команда показывает какая именно локальная ветка будет отправлена на удалённый сервер по умолчанию при выполнении git push. Она также показывает, каких веток с удалённого сервера у вас ещё нет, какие ветки всё ещё есть у вас, но уже удалены на сервере, и для нескольких веток показано, какие удалённые ветки будут в них влиты при выполнении **git pull**

## Удаление и переименование удалённых репозиториев

>Для переименования удалённого репозитория можно выполнить **git remote rename**. Например, если вы хотите переименовать *pb*, вы можете это сделать при помощи **git remote rename**

>Стоит упомянуть, что это также изменит имена удалённых веток в вашем репозитории. То, к чему вы обращались как *pb/master*, теперь стало *paul/master*

>Если по какой-то причине вы хотите удалить удалённый репозиторий — вы сменили сервер или больше не используете определённое зеркало, или кто-то перестал вносить изменения — вы можете использовать **git remote rm**

>При удалении ссылки на удалённый репозиторий все отслеживаемые ветки и настройки, связанные с этим репозиторием, так же будут удалены