# How to use a Java tool from Eurostat/github

This page quickly describes a way to start using one of the Java tools proposed on Eurostat Github space.

## Prerequisite

If not already installed, download and install [Java](https://www.java.com/en/download/), [Git](https://git-scm.com/) and [Maven](https://maven.apache.org/).

## Get the tool

To retrieve the code of the tool you want to use, launch a command `git clone https://github.com/eurostat/MY_TOOL.git` where `MY_TOOL` is the name of the tool.

To install it, go to the folder of the tool with `cd path_to/MY_TOOL`. There should be a *pom.xml* file in this folder. Then run `mvn clean install`.

## Create a Java project (with Eclipse)

If not already installed, download and install [Eclipse](https://www.eclipse.org/).

- Launch Eclipse
- Select your desired workspace location or accept the proposed one.
- Create a new project with *File > New > Project... > Maven > Maven Project*.
- Check the box *Create a simple project*
- Choose a *Group Id* such as *org.myorganisation* and an *Artifact Id* such as *my_application*. Keep the other options and hit *Finish* button.
- Right click on *src/main/java* and select *New > Class*. Choose *MyApplication* as class name and or another preferred class name and hit *Finish* button.
- Insert the following code:
```java
package MyApplication

public class MyApplication {

  public static void main(String[] args) {
    System.out.println("Hello Europe !");
  }

}
```
and launch it with *Run > Run* (or Ctrl+F11). You should see the text *Hello Europe !* displayed in the output console.

## Use the tool

At the base of your project folder, there should be a *pom.xml* file, which describes your application. To indicate the application uses the tool, include the following `<dependencies>` section:

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


## Feedback

Something missing, outdated or wrong? Feel free to [report it](https://github.com/eurostat/README/issues/new).
