# Отчёт о тестировании приложения "Credit Card Number Validator"

## Краткое описание

С 10.06.2021 по 11.06.2021 было проведено функциональное тестирование приложения "Credit Card Number Validator".

На тестирование затрачено: 2 часа.

В результате тестирования выявлены следующие дефекты:
* [Номера карт American Express из 15 цифр не проходят валидацию](https://github.com/Ekaterina-Isabel/javaqa-homeworks/issues/1#issue-917628565)
* [Номера карт Diners Club - Carte Blanche и Diners Club - International из 14 цифр не проходят валидацию](https://github.com/Ekaterina-Isabel/javaqa-homeworks/issues/2)
* [Номера карт VISA, Discover, JCB из 19 цифр не проходят валидацию](https://github.com/Ekaterina-Isabel/javaqa-homeworks/issues/4)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* [код автотеста](https://github.com/Ekaterina-Isabel/javaqa-homeworks/blob/master/src/Main.java)

В качестве тестовых данных использовались номера карт с сайтов: [Get Credit Card Numbers](https://www.getcreditcardnumbers.com/) и [Credit Card Number Generator & Validator](https://www.freeformatter.com/credit-card-number-generator-validator.html) (данные с ожидаемым результатом):
* номера карт, состоящие из 15 цифр проходят валидацию (результат автотестирования "Result is OK")
* номера карт, состоящие из 14 цифр проходят валидацию (результат автотестирования "Result is OK")
* номера карт, состоящие из 19 цифр проходят валидацию (результат автотестирования "Result is OK")

Тестирование производилось в следующем окружении:
* 64-разрядная операционная система, процессор x64, версия 20H2
* версия Java "14.0.2" 2020-07-14
* IntelliJ IDEA Community Edition 2021.1.2 x64
