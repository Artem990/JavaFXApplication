# Программа для поиска текста в log файлах (JavaFX)

Если не запускается JavaFX нужно: 
1. Установить sdk 12 — https://gluonhq.com/products/javafx/
2. Подключить библиотеку все файлы jar из папки lib
3. В Run добавить new configuration и указать в VM Options (--module-path "PATH_TO_LIBRARY_JAR" --add-modules javafx.controls,javafx.fxml)

-----
![FXApp](https://user-images.githubusercontent.com/35997083/61596915-1a2c2400-ac12-11e9-88aa-b8914e5b36a6.png)

### Написать программу для поиска заданного текста в лог файлах

Пользователь должен иметь возможность указать папку в сети или на жестком диске, в которой будет происходить поиск заданного текста, включая все вложенные папки.

Должна быть возможность ввода текста поиска и ввода типа расширения файлов, в которых будет осуществляться поиск(расширение по умолчанию *.log).

Результаты поиска можно вывести в левой части приложения в виде дерева файловой системы только те файлы в которых был обнаружен заданный текст.

В правой части приложения выводить содержимое файла с возможностью навигации по найденному тексту (выделить все, вперед/назад).

Плюсом будет многопоточность приложения, «не замораживание» приложения на время поиска, возможность открывать «большие» (более 1Г) файлы и осуществлять по ним быструю навигацию, возможность открывать файлы в новых «табах», т. е. использовать TabFolder или MDI.

Для отображения разрешается использовать любые Java GUI-фреймворки (AWT, Swing, SWT, JavaFX, NetBeans Platform и т.п.).

Приложение может быть как десктопным, так и веб-клиентом.