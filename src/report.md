# Отчёт о тестировании приложения "Precision"

## Краткое описание

Для внедрения дополнительного бонуса новым клиентам компании ее программистами был написан следующий код:

```java
public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
  }
}
```

При функциональном тестировании кода было обнаружено, что в приложении при суммировании значений бонусов его итоговое значение не округляется до вида 1 знака после запятой. Результат выдается в виде 0.8999999999999999 вместо 0.9  



## Описание тестов

Было проведено функциональное тестирование приложения. 

## Результаты

1. 100 % не успешных тестов
2. [Приложение "Precision" не округляет итоговый результат, полученный при сложении чисел](https://github.com/domainlover/Java_Zadanie2.2/issues/1)

## Общие рекомендации

Необходимо произвести соответствующие корректировки в коде приложения, чтобы при сложении чисел значение результата округлялось до 1 знака после запятой.
