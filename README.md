# Проект по автоматизации тестирования для сервиса [Petstore](https://petstore.swagger.io/)

> This is a sample server Petstore server.

## **Содержание:**

____

* <a href="#tools">Технологии и инструменты</a>

* <a href="#cases">Примеры автоматизированных тест-кейсов</a>

* <a href="#jenkins">Сборка в Jenkins</a>

* <a href="#console">Запуск из терминала</a>

* <a href="#allure">Allure отчет</a>

* <a href="#allure-testops">Интеграция с Allure TestOps</a>

* <a href="#telegram">Уведомление в Telegram при помощи бота</a>

## ☑️ Использованные технологии и инструменты

<p align="center">
<a href="https://www.jetbrains.com/idea/"><img width="7%" title="IntelliJ IDEA" src="media/logo/IntelliJ_IDEA.png"></a>
<a href="https://www.java.com/"><img width="7%" title="Java" src="media/logo/Java.png"></a>
<a href="https://gradle.org/"><img width="7%" title="Gradle" src="media/logo/Gradle.png"></a>
<a href="https://junit.org/junit5/"><img width="7%" title="JUnit5" src="media/logo/JUnit5.png"></a>
<a href="https://selenide.org/"><img width="7%" title="Selenide" src="media/logo/Selenide.png"></a>
<a href="https://www.jenkins.io/"><img width="7%" title="Jenkins" src="media/logo/Jenkins.png"></a>
<a href="https://aerokube.com/selenoid/"><img width="7%" title="Selenoid" src="media/logo/Selenoid.png"></a>
<a href="https://allurereport.org/"><img width="7%" title="Allure Report" src="media/logo/AllureReports.png"></a>
<a href="https://qameta.io/"><img width="7%" title="Allure TestOps" src="media/logo/AllureTestOps.svg"></a>
<a href="https://github.com/"><img width="7%" title="GitHub" src="media/logo/GitHub.png"></a>
<a href="https://web.telegram.org/k/"><img width="7%" title="Telegram" src="media/logo/Telegram.png"></a>
</p>

- Язык для написания тестов : [Java](https://www.java.com/ru/)
- Фреймворк для модульного тестирования : [Junit5](https://github.com/junit-team/junit5)
- Система автоматической сборки : [Gradle](https://github.com/gradle)
- Удаленный запуск с выбором параметров для тестов реализован при помощи :  [Jenkins](https://www.jenkins.io/)
- Отчеты о пройденных тестах формируются при помощи : [Allure](https://github.com/allure-framework)
- Так же отчеты о тестировании отправляются в мессенджер при помощи <code>Telegram</code> бота
- Реализована интеграция с [Allure TestOps](https://qameta.io/)
- Реализация API тестов при помощи <code>RestAssured</code>

____
<a id="cases"></a>

## <a name="Примеры автоматизированных тест-кейсов">**Примеры автоматизированных тест-кейсов:**</a>

____

- ✓ *Получение данных зарегистрированного пользователя*
- ✓ *Обновление данных пользователя*
- ✓ *Успешная авторизация пользователя*
- ✓ *Успешное удаление пользователя*
- ✓ *Успешное оформление заказа*
- ✓ *Получение данных о заказе*

____
<a id="jenkins"></a>

## <img alt="Jenkins" height="25" src="media/logo/Jenkins.png" width="25"/></a><a name="Сборка"></a>Сборка в [Jenkins](https://jenkins.autotests.cloud/job/Petstore/)</a>

____
<p align="center">  
<a href="https://jenkins.autotests.cloud/job/Petstore/"><img src="media/screenshots/Jenkins.png" alt="Jenkins" width="950"/></a>  
</p>

### **Параметры сборки в Jenkins:**

- *task (выбор группы тестов для запуска, по умолчанию все - test)*

<a id="console"></a>

## Команды для запуска из терминала

___
***Локальный запуск:***

```bash  
gradle clean test
```

***Удалённый запуск через Jenkins:***

```bash  
clean ${TASK}
```

___
<a id="allure"></a>

## <img alt="Allure" height="25" src="media/logo/AllureReports.png" width="25"/></a> <a name="Allure"></a>Allure [отчет](https://jenkins.autotests.cloud/job/Petstore/3/allure/)</a>

___

### *Основная страница отчёта*

<p align="center">  
<img title="Allure Overview Dashboard" src="media/screenshots/AllureDashBoard.png" width="850">  
</p>  

### *Тест-кейсы*

<p align="center">  
<img title="Allure Tests" src="media/screenshots/AllureTestCases.png" width="850">  
</p>

### *Графики*

  <p align="center">  
<img title="Allure Graphics" src="media/screenshots/AllureGraphics.png" width="850">
</p>

___
<a id="allure-testops"></a>

## <img alt="Allure" height="25" src="media/logo/AllureTestOps.svg" width="25"/></a>Интеграция с <a target="_blank" href="https://allure.autotests.cloud/launch/43618/">Allure TestOps</a>

____

### *Allure TestOps Dashboard*

<p align="center">  
<img title="Allure TestOps Dashboard" src="media/screenshots/TestOpsDashBoard.png" width="850">  
</p>

### *Авто тест-кейсы*

<p align="center">  
<img title="Allure TestOps Tests" src="media/screenshots/TestOpsTestCases.png" width="850">  
</p>

____
<a id="telegram"></a>

## <img alt="Telegram" height="25" src="media/logo/Telegram.png" width="25"/></a> Уведомление в Telegram при помощи бота

____
<p align="center">  
<img title="Telegram" src="media/screenshots/Telegramm.png" width="550">  
</p>
