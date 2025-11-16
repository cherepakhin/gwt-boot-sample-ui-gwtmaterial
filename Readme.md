## Простое GWT приложения.

Spring Boot нет.

### Сборка:

````shell
./mvnw package
````

Открыть в браузере [index.html](file:///home/vasi/prog/java/gwt/gwt-boot-samples/gwt-boot-sample-ui-gwtmaterial/target/gwt-boot-sample-ui-gwtmaterial-1.2.0-SNAPSHOT/gwtmaterial/index.html)

Результат ![результат](/doc/gwt-boot-sample-ui-gwtmaterial_screen.png)

__Устраивает.__

### Размещение на сайте (apache2).

После _mvn package_, содержимое target/gwt-boot-sample-ui-gwtmaterial-1.2.0-SNAPSHOT/gwtmaterial скопировать в папку __/var/www/main/gwtmaterial__.<br/>
Имя папки __gwtmaterial__ указано в pom.xml в секции __build__, в конфигурации plugin __gwt-maven-plugin__.

Результат [https://v.perm.ru/gwtmaterial/](https://v.perm.ru/gwtmaterial/)
