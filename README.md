# Отчет о тестировании Precision

22.09.2021 - 22.09.2021 было проведено санитарное тестирование приложения Precision.

На тестирование затрачено: 1 часа

В результате тестирования выявлены следующие дефекты:
* [Расчет произведен неверно в приложении Precision после сложения переменных "double regularBonus" и "double specialBonus"](https://github.com/bigsurmoon/java2.2/issues/1)

## Описание процесса тестирования

В качестве тестовых данных использовался код, переданный нам программистами:
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


Тестирование производилось в следующем окружении:
* ОС: Windows 10 19043.1165 x64
* Java: 11.0.11
* Среда разработки: IntelliJ IDEA 2021.2.1
