# Отчёт по работе с Git
## Часть 1: обзор базовых команд при помощи терминала

Сначала откроем выбранную локально папку и создадим там файл: **echo. >  readme.txt**. Команда **git status** показывает на какой мы сейчас ветке, историю коммитов и несохранённых изменений: <img width="893" height="293" alt="image" src="https://github.com/user-attachments/assets/ebb1f984-a374-40ef-ba74-93bb75883a1f" />

<img width="914" height="216" alt="image" src="https://github.com/user-attachments/assets/9c250f64-2462-4ea4-a054-3abe99635a76" />



Добавим репозиторий для удвлённого доступа и выберем ветку для выгрузки. **git remote add origin <ссылка на репозиторий>** и **git push** <img width="974" height="707" alt="image" src="https://github.com/user-attachments/assets/a03e3814-c090-47df-9a6f-ac8679707111" />



Проверим последние изменения репозитория при помощи команды **git pull origin master**:
<img width="974" height="376" alt="image" src="https://github.com/user-attachments/assets/bfd04e38-488a-441e-a302-dcf46803c15b" />

Увидеть, какие изменения произошли в гите, можно с помощью команды **git diff HEAD**, в команда **git merge <ветка, с которой совершить слияние>** совершит слияние выбранной ветки с текущей:
<img width="974" height="412" alt="image" src="https://github.com/user-attachments/assets/ea2dc6a4-df43-4158-972a-4bfcaa4d8b32" />


## Часть 2: обзор базовых команд в гит используя среду разработки и надстройки для гита

Дополнительно использую расширение GitLens для работы с гитом. Сначала нужно подключиться к репозиторию. Я зажала клавишу «F1» и ввела ссылку на свой репозиторий в гит: https://github.com/ddarlaa/ddarlaa.github.io
После этого изменила код своей индексной страницы:
<img width="1011" height="497" alt="image" src="https://github.com/user-attachments/assets/22563ffa-1fa1-40bc-af53-07bb3d6550ff" />

Для того, чтобы обновить все данные, перед коммитом нужно сделать синхронизацию. Использовала кнопку «Sync All»:


Использовали кнопку «Fetch All», чтобы получить все предыдущие изменения репозитория.
После этого использовала кнопку «Commit & Push» в интерфейсе **Source Control**. Для обратного действия (получить удалённые изменения локально) в том же **Source Control**, нажав на троеточие, можно совершить команду **Pull**: <img width="456" height="630" alt="image" src="https://github.com/user-attachments/assets/ab85d5dd-7ba5-4940-b7d6-686777f04054" />
<img width="608" height="378" alt="image" src="https://github.com/user-attachments/assets/9f6d563d-a222-4611-8a90-349e116a3a43" />


Для слияния зажала горячие клавиши «Ctrl+Shift+Р», ввела **Git: Merge** и выбрала из выпадающего списка ветку, из которой хочу получить слияние с текущей. В данном случае я сделала слияние из ветки **main** в ветку **master**:
<img width="1090" height="264" alt="image" src="https://github.com/user-attachments/assets/44ed58b9-4f73-4705-b42b-a573de94c3b4" />


Для команды **reset** использовала другую команду: **> Git: Undo Last Commit**
Эта операция совершила **soft reset** — последний коммит отменен, но все изменения остались в рабочей директории
