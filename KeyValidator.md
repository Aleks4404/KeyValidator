# Отчёт о тестировании KeyValidator

## Краткое описание

30.03.2021 - 30.03.2021. Было проведено функциональное тестирование (валидация лицензионных ключей) приложения KeyValidator

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:

https://github.com/Aleks4404/KeyValidator/issues/1
https://github.com/Aleks4404/KeyValidator/issues/2
https://github.com/Aleks4404/KeyValidator/issues/3

Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:

1.Домашнее задание к занятию «1.1. Введение в Java: JDK, JRE, JVM, IntelliJ IDEA» https://github.com/netology-code/javaqa-homeworks/tree/master/intro
2.Отчёт о тестировании <Название приложения> https://github.com/netology-code/javaqa-homeworks/blob/master/intro/report.md


В качестве тестовых данных использовались данные из Руководства использования KeyValidator https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md

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