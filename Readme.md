## Простое GWT приложение с Material UI.

Spring Boot нет. Приложение компилируется в js.

### Сборка:

````shell
./mvnw package
````

java version 11

````shell
export JAVA_HOME=/usr/lib/jvm/java-1.11.0-openjdk-amd64/
echo $JAVA_HOME
/usr/lib/jvm/java-1.11.0-openjdk-amd64/
````

Открыть в браузере [index.html](target/gwt-boot-sample-ui-gwtmaterial-1.2.0-SNAPSHOT/gwtmaterial/index.html)

Результат ![результат](/doc/gwt-boot-sample-ui-gwtmaterial_screen.png)

![на телефоне](/doc/screen_phone1.jpg)

__Устраивает.__

### Структура приложения
В public/index.html в <div id="mainPanel" /> подключается GwtMaterialEntryPoint через RootPanel.get("mainPanel").add(helloWorldView);

### Размещение на сайте (apache2).

После _mvn package_, содержимое target/gwt-boot-sample-ui-gwtmaterial-1.2.0-SNAPSHOT/gwtmaterial скопировать в папку __/var/www/main/gwtmaterial__.<br/>
Имя папки __gwtmaterial__ указано в pom.xml в секции __build__, в конфигурации plugin __gwt-maven-plugin__.

Результат [https://v.perm.ru/gwtmaterial/](https://v.perm.ru/gwtmaterial/)

### Разное

[Последняя версия GWT 2.11.0 9 января 2024](https://ru.wikipedia.org/wiki/Google_Web_Toolkit)

"Утилита командной строки webAppCreator, поставляемая вместе с GWT, автоматически создает все файлы, необходимые для нового GWT-проекта."

"Многие обычные виджеты, отсутствующие в GWT, реализованы в сторонних библиотеках, таких как Sencha GXT, GWT Component Library, GWT-Ext, GWT Widget Library, GWTiger, Rocket GWT, Dojo, SmartGWT и т. д."

"Некоторые из наиболее распространенных мобильных библиотек GWT: GwtMobile, GWT-мобильный-WebKit, jqm4gwt, м-GWT"

[https://www.baeldung.com/gwt](https://www.baeldung.com/gwt)
[https://github.com/gwtproject](https://github.com/gwtproject)
[https://github.com/gwtproject/gwt](https://github.com/gwtproject/gwt)
[gwt-editor](https://github.com/gwtproject/gwt-editor)
[http://www.g-widgets.com/gwt-doc/doc/latest/tutorial/buildui.html](http://www.g-widgets.com/gwt-doc/doc/latest/tutorial/buildui.html)
[https://github.com/samvandesteen/vogella](https://github.com/samvandesteen/vogella)