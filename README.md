## Laboratory work III

Данная лабораторная работа посвещена изучению систем автоматизации сборки проекта на примере **CMake**

```sh
$ open https://cmake.org/
```

## Tasks

- [x] 1. Создать публичный репозиторий с названием **lab03** на сервисе **GitHub**
- [x] 2. Ознакомиться со ссылками учебного материала
- [x] 3. Выполнить инструкцию учебного материала
- [x] 4. Составить отчет и отправить ссылку личным сообщением в **Slack**

## Homework
### Задание 1
Вам поручили перейти на систему автоматизированной сборки **CMake**.
Исходные файлы находятся в директории [formatter_lib](formatter_lib).
В этой директории находятся файлы для статической библиотеки *formatter*.
Создайте `CMakeList.txt` в директории [formatter_lib](formatter_lib),
с помощью которого можно будет собирать статическую библиотеку *formatter*.
`$ git clone git@github.com:LatyshevBogdan/Lab3.git
`

![image](https://user-images.githubusercontent.com/126398794/228633068-ee397443-b26c-4426-b753-f1f551b77b17.png)

 `
 клонирование репозитория и создание CMakeList.txt для formatter_lib
 `
 
 ![image](https://user-images.githubusercontent.com/126398794/228633588-96c5396c-371f-4030-883e-c64692f9b8a9.png)
 
### Задание 2
У компании "Formatter Inc." есть перспективная библиотека,
которая является расширением предыдущей библиотеки. Т.к. вы уже овладели
навыком созданием `CMakeList.txt` для статической библиотеки *formatter*, ваш 
руководитель поручает заняться созданием `CMakeList.txt` для библиотеки 
*formatter_ex*, которая в свою очередь использует библиотеку *formatter*.

![image](https://user-images.githubusercontent.com/126398794/228634026-79be7be3-636e-4cd6-afe6-99989a6ce067.png)
`
создание CMakeList.txt для formatter_ex_lib на основе созданного в formatter_lib
`
![image](https://user-images.githubusercontent.com/126398794/228634347-a3b8fa21-0d9e-46b7-8564-7482563bd8f2.png)

### Задание 3
Конечно же ваша компания предоставляет примеры использования своих библиотек.
Чтобы продемонстрировать как работать с библиотекой *formatter_ex*,
вам необходимо создать два `CMakeList.txt` для двух простых приложений:
* *hello_world*, которое использует библиотеку *formatter_ex*;
* *solver*, приложение которое испольует статические библиотеки *formatter_ex* и *solver_lib*.

![image](https://user-images.githubusercontent.com/126398794/228635035-d452cd53-1d3c-4707-bba8-2c60eab68fe1.png)

![image](https://user-images.githubusercontent.com/126398794/228635120-4153eaad-c85b-4c59-b938-af4f71bab6a0.png)
`
CMakeList.txt для приложения hello_world (подключение библиотеки formatter_ex_lib с указанием возможности ее линковки под именем hello; подключение исходного hello_world.cpp файла)
`

![image](https://user-images.githubusercontent.com/126398794/228635248-1c444c88-3c73-406d-bae2-640c487e3347.png)
`
создание CMakeList.txt для библиотеки solver_lib
`

![image](https://user-images.githubusercontent.com/126398794/228635413-cb677efa-6317-4bef-bd26-b14b4d5e15eb.png)
![image](https://user-images.githubusercontent.com/126398794/228635570-ea59f9b5-df37-4cd1-ba89-7b905a6583fb.png)

`
CMakeList.txt для приложения solver_application
`

