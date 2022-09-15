# Automation_Selenide_Allure [![Build status](https://ci.appveyor.com/api/projects/status/6sp4s9tdcfdyeihs?svg=true)](https://ci.appveyor.com/project/holyblaz/automation-selenide-allure)

# Обучение в Нетологии.

## Курс Автоматизированное тестирование

## Тема: Репортинг: Allure, Report Portal

- Настройка Allure, интегрированного с Selenide
- Настройка ReportPortal (в работе, планирую дальнейшее изучение ReportPortal)

# Инструкция по настройке Allure
1. В проекте в build.gradle прописать  

``` 
plugins {
    id 'java'
    id 'io.freefair.lombok' version '5.3.0'
    id 'io.qameta.allure' version '2.9.6'
}

group 'ru.netology'
version '1.0-SNAPSHOT'

sourceCompatibility = 11
compileJava.options.encoding = "UTF-8"
compileTestJava.options.encoding = "UTF-8"

allure {
    version = '2.18.1'
    useJUnit5 {
        version = '2.18.1'
    }
}

repositories {
    mavenCentral()
}
 ```
 
**Для запуска использовать команду**
```
gradlew clean test allureReport
```
``` 
gradlew allureServe
```
# Allure report

![Allure_report_1](https://user-images.githubusercontent.com/98361526/190460415-8fa554b0-d844-4603-af6e-5b089b61bfb6.png)
![Allure_report_2](https://user-images.githubusercontent.com/98361526/190460437-9d61ccee-6f3c-4a39-a81d-145a4b23e94a.png)


