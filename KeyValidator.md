# Отчёт о тестировании KeyValidator

## Краткое описание
* 31.03.2021 - 31.03.2021. Выполнили установку приложения по инструкци установки OpenJDK11 на ОС Windows 10 Home 64 bit
* 31.03.2021 - 31.03.2021. Выполнили запуск приложения и проверили совместимо Windows 10 Home 64 bit с Java 11
* 31.03.2021 - 31.03.2021. Выполнили провеку приложения на корректность работы согласно руководству использования


На тестирование затрачено: 4 часа

В результате тестирования выявлены следующие дефекты:

* [Некорректный номер валидного ключа](https://github.com/Aleks4404/KeyValidator/issues/1)
* [При проверке валидного ключа появляется сообщение FAIL](https://github.com/Aleks4404/KeyValidator/issues/2)
* [При проверке не валидного ключа появляется сообщение OK](https://github.com/Aleks4404/KeyValidator/issues/3)

Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:

* [Домашнее задание к занятию «1.1. Введение в Java: JDK, JRE, JVM, IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/tree/master/intro)
* [Ссылка для скачивания приложения OpenJDK11](https://adoptopenjdk.net/)
* [Отчёт о тестировании KeyValidator](https://github.com/Aleks4404/KeyValidator.git)


В качестве тестовых данных использовались данные:
* [Инструкция по установке OpenJDK 11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md)
   
    Ввести следующие команды в терминале:
    java -version - Ожидаемый результат - openjdk version "11.0.10" 2021-01-19
                                          OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.10+9)
                                          OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.10+9, mixed mode)

* [Руководство использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)

Валидные ключи:

* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998 - Ожидаемый результат - ок.
* 80b427f8-92cd-3aae-ba04-3927fbe17c6. - Ожидаемый результат - ок.
* b295bc63-9f03-3b4b-af80-969b39f8c262 - Ожидаемый результат - ок.
* 387eedc6-12e9-3b32-9881-63b6b5e85317 - Ожидаемый результат - ок.
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180 - Ожидаемый результат - ок.

Невалидные ключи:

* 18252235-78e0-44a5-8720-556f0c7da17a - Ожидаемый результат - fail.
* e66075b6-ddad-445e-baf6-161b3289522b - Ожидаемый результат - fail.
* b6d53250-f07e-4352-a293-6102ddf7f1ca - Ожидаемый результат - fail.
* c2bc778a-1cb9-46c6-b435-0489649d2a42 - Ожидаемый результат - fail.
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1 - Ожидаемый результат - fail.

Тестирование производилось в следующем окружении:
* Windows 10 Home 64 bit
* версия Java 11.0.10