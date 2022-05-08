Java Maven Build Executable Jar Demo
====================================

需要使用maven的`maven-dependency-plugin`和`maven-jar-plugin`插件，才能生成一个可以通过`java -jar`运行的jar，
否则会报`no main manifest attribute, in target/demo.jar`错误。

另外：在pom.xml中可以通过`<finalName>demo</finalName>`来指定生成的jar名字。

```
mvn clean package
java -jar target/demo.jar
```