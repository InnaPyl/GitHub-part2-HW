# GitHub.-HW_2
Создаем  внешний репозиторий c названием GitHub. HW_2 , копируем ссылку **https://github.com/InnaPyl/GitHub.-HW_2.git**
В терминале Bash : 
```
git clone https://github.com/InnaPyl/GitHub.-HW_2.git 
```
1.На локальном репозитории сделать ветки для: 
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing
```
Git branch Postman
Git branch  Jmeter
Git branch  CheckLists и т.д.
```
2.Запушить все ветки на внешний репозиторий
```
git push -u origin Postman
git push -u origin Jmeter 
git push -u origin CheckLists  и т.д.
```
3.В ветке Bag Reports сделать текстовый документ со структурой баг репорта
```
Touch Bag Reports.txt -> vim Bag Reports.tx -> I
ID:номер
summary:краткое описание
description:полное описание
environment:окружение
steps_to_reproduce:шаги воспроизведения
actual_result:фактический результат
expected_result:ожидаемый результат
severity:серьезность
priority:приоритет
additional_information:дополнения
Esc -> :wq
```
4.Запушить структуру багрепорта на внешний репозиторий 
```
Git push
```
5.Вмержить ветку Bag Reports в Main
```
Git checkout main
Git merge -m “Merging BagReports into main” BagReports
```
6. Запушить main на внешний репозиторий.
```
git push
```
7. В ветке CheckLists набросать структуру чек листа.
```
Cat >> Checklist.txt
Номер
Описание
Пример
Результат
```
8.Запушить структуру на внешний репозиторий
```
Git add .
Git commit -m "AddChecklist"
Git push
```
9.На внешнем репозитории сделать Pull Request ветки CheckLists в main
```
Нажать в вебе на Pull requests -> New Pull Request
Base: main   compare: CheckLists
```
10. Синхронизировать Внешнюю и Локальную ветки Main
```
git checkout main
git pull
```
