# Описание
Часто используемые, полезные, интересные и нужные команды Git терминала.

## Оглавление

1. [Стянуть определённый файл из другой ветки в текущую](#Стянуть-определённый-файл-из-другой-ветки-в-текущую);
2. [Удалить локальную ветку](#Delete-local-branch);
3. [Отменить изменения в Git](#Отменить-изменения-в-Git);
  
____

## Стянуть определённый файл из другой ветки в текущую
```
git checkout [current branch]                               # first get back to [current branch]    
git checkout [branch 'from'] -- [neededFile.js/txt/...]     # then copy the version of file from [branch 'from']    
```
____

## Delete local branch

Local branches can be removed from VS Code by opening the Command Pallete (**Ctrl-Shift-P**) then Selecting ```Git: Delete Branch...```, you can then delete the local branch by selecting the appropriate one from the list.

## Отменить изменения в Git

**```git revert```**: Команда отмены, однако принцип её действия отличается от привычной отмены изменений. Вместо удаления коммита эта команда отменяет внесённые в нём изменения и добавляет новый коммит с обращённым содержимым. В результате история в Git не теряется, что важно для обеспечения целостной истории версий и надёжной совместной работы.

**```git reset```** : Универсальная команда Git для отмены изменений. У команды ```git reset``` есть ряд режимов:  
```--soft```: только сброс указателя HEAD до выбранного коммита. Действие команды аналогично ```git checkout <номер коммита>```, но в этом режиме указатель HEAD не открепляется.  
```--mixed```: сброс указателя HEAD до выбранного коммита в истории и отмена изменений в индексе.  
```--hard```: сброс указателя HEAD до выбранного коммита в истории, отмена изменений в индексе и отмена изменений в рабочем каталоге. 

P.S. Подробное описание принципа работы команды git reset приведено в разделе сайта git-scm.com [Git Tools — Reset Demystified (Инструменты Git — Раскрытие тайн reset)](https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified).  
P.P.S. Также подробнее можно прочитать по [ссылке](https://www.atlassian.com/ru/git/tutorials/learn-undoing-changes-with-bitbucket).
