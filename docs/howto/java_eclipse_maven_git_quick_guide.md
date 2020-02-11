# How to use a Java library from Eurostat/github

This page describes a quick way to start using one of the Java libraries proposed on Eurostat Github space such as [JGiscoTools](https://github.com/eurostat/JGiscoTools) or [Java4Eurostat](https://github.com/eurostat/Java4Eurostat).

## 1- Create a Java project (with Eclipse)

- If not already installed, download and install [Eclipse](https://www.eclipse.org/)
- Launch Eclipse.
- On first time launch, select the desired workspace location or accept the proposed one.
- Create the Java/Maven project of your application with: *File > New > Project... > Maven > Maven Project*.
- Check the box: *Create a simple project*.
- Choose a *Group Id* such as *org.myorganisation* and an *Artifact Id* such as *my_application*. Keep the other options and hit *Finish* button. You application is now created.
- To test it, right click on *src/main/java* and select *New > Class*. Choose *MyApplication* or another preferred class name and hit *Finish* button.
- Insert the following test code:

```java
package MyApplication

public class MyApplication {

  public static void main(String[] args) {
    System.out.println("Hello Europe !");
  }

}
```

- Finally, save and launch the application with *Run > Run* (or Ctrl+F11). You should see the text *Hello Europe !* displayed in the output console.

## 2- Use the tool

Edit the *pom.xml* file located at the base of the project folder. This file describes your application, including its dependencies. To indicate the application uses the tool, include the following `<dependencies>` section:

```
<project (...) >
  (...)

  <dependencies>
    <dependency>
      <groupId>eu.europa.ec.eurostat</groupId>
      <artifactId>MY_TOOL</artifactId>
      <version>X.Y</version>
    </dependency>
  </dependencies>

</project>
```

where `MY_TOOL` is the name of the tool and `X.Y` its last version as it appears in [Maven central repository](https://mvnrepository.com/artifact/eu.europa.ec.eurostat).

Hit F5 and Alt+F5 to refresh the project. It should then be possible to use the tool in the `main` function of the application. You could start with the code snippets usually proposed in the tool documentation.

## Feedback

Something missing, not clear, outdated or wrong on this page? Feel free to [report it](https://github.com/eurostat/README/issues/new).
