#Интеграция webpack в Visual Studio 2015 

## Установка webpack 

```
$ npm install webpack -g 
``` 

## Установка расширения Webpack Task Runner 

https://visualstudiogallery.msdn.microsoft.com/5497fd10-b1ba-474c-8991-1438ae47012a 

## Использование Webpack Task Runner

* Конфигурационный файл webpack.config.js следует разместить в директории с приложением. 
* Для автоматической компиляции файлов при открытии проекта с приложением в Visual Studio, добавьте конфигурационный файл webpack следующую строку (в самом начале файла): 
```
/// <binding ProjectOpened='Watch - Development' /> 
``` 

* Для открытия приложения выберите в меню File > Open > Website и в открывшемся диалоговом окне выберите папку с вашим приложением. 

* Для открытия диалогового окна Webpack Task Runner в Visual Studio перейдите в пункт меню Tools и выберите опцию Task Runner Explorer. 
* Для открытия файла выберите нужный файл и нажмите Ctrl+F5

## Отправка файлов на репозиторий 

При наличии большой вложености папок в проекте (node_module), рекомендуется использовать Git Bush, 
для отправки данных на GitHub. Очередность віполнения команд:

1) Stage the file for commit: 

``` 
git add .
```

2) Commit the file:
```
git commit -m "update"
```

3) Push the changes to GitHub.:
```
git push origin master
```