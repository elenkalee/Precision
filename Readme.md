# Отчёт о тестировании приложения "Precision"

## Краткое описание

В приложении некорректно исчисляется сумма вещественных чисел

## Описание тестов

 Проводилось позитивное функциональное тестирование приложения. Было проведено санитарное тестирование функции расчета  дополнительного бонуса новым клиентам.

 [Исходные данные взяты из Задачи №2 - Precision](https://github.com/netology-code/javaqa-homeworks/tree/master/programming)

Код приложения:

```java
public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
````
Ожидаемый результат: 0.9 

## Результаты

1. 100% неуспешных тестов
2. [Некорректная сумма дополнительных бонусов при вычислении в программе Precision](https://github.com/elenkalee/Precision/issues/1)

## Общие рекомендации

Рекомендуем обратить внимание на синтаксис записи вещественных числе в коде, так как сумма чисел в формате `0.0` выдает в итоге некорректное значение.
