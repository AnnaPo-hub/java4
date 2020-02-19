# Отчет о тестировании приложения бонусной системы.
## Краткое описание 
 18.02.20-18.02.20 было проведено функциональное тестирование приложения бонусной системы.

На тестирование затрачено 30 минут. 

### В результате тестирования был выявлен баг: 
В программе задан неверный тип переменной из-за чего отображается неверный финальный процент бонуса.


Подробнее в баг репорте в Issues 
https://github.com/AnnaPo-hub/java4/issues/1



## Описание процесса тестирования 

В качестве тестовых данных использовались данные: 
```java
public class precision {
    public static void main(String[] args) {
        double regularBonus = 0.3F;
        double specialBonus = 0.6F;
        double totalBonus = regularBonus + specialBonus;
        System.out.println(totalBonus);

    }
} 
```

 -  regularBonus = 0.3;
  - specialBonus = 0.6;
 



Тестирование производилось в следующем окружении:
 - macOS Catalina 10.15.3
 - openjdk version "1.8.0_242
 - IntelliJ IDEA 2019.3.2


