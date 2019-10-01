# How to use a Java tool from Eurostat/github

This page quickly describes a way to start using one of the Java tools proposed on Eurostat Github space.

## Prerequisite

If not already installed, download and install [Java](https://www.java.com/en/download/), [Git](https://git-scm.com/) and [Maven](https://maven.apache.org/).

## Get the tool

To retrieve the code of the tool you want to use, launch a command: `git clone https://github.com/eurostat/MY_TOOL.git`, where `MY_TOOL` is the name of the tool.

To install it, move to the folder of the tool with a command: `cd path_to/MY_TOOL`. There should be a *pom.xml* file in this folder. Then run `mvn clean install`.

## Create a Java project (with Eclipse)

If not already installed, download and install [Eclipse](https://www.eclipse.org/).

- Launch Eclipse.
- On first time launch, select the desired workspace location or accept the proposed one.
- Create the Java/Maven project of your application with: *File > New > Project... > Maven > Maven Project*.
- Check the box: *Create a simple project*
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
- Save and launch the application with *Run > Run* (or Ctrl+F11). You should see the text *Hello Europe !* displayed in the output console.

## Use the tool

Edit the *pom.xml* file located at the base of the project folder. This file describes the application. To indicate the application uses the tool, include the following `<dependencies>` section:

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
where `MY_TOOL` is the name of the tool and `X.Y` the version tag.

Hit F5 and Alt+F5 to refresh the project. It should then be possible to use the tool in the `main` function of the application.

## Feedback

Something missing, outdated or wrong? Feel free to [report it](https://github.com/eurostat/README/issues/new).
