# desktopEntry Task #

## Task definition in your build file ##
To use the desktopEntry task, you will have to define it in your build file. This is done by following code:
```
    <path id="ant-deb.classpath">
        <fileset dir="enterHereYourDirectoryPathTo_ant-deb.jar" includes="*.jar"/>
    </path>

    <taskdef name="desktopEntry" classname="com.googlecode.ant_deb_task.DesktopEntry" classpathref="ant-deb.classpath"/>
```

Here you can find the ant-deb-{version}.jar http://code.google.com/p/ant-deb-task/downloads/list

## Attributes ##

  * **toFile**
  * **type** - one of: ("Application", "Link", "Directory"), default is "Application"
  * **name**
  * **genericName**
  * **noDisplay** - boolean
  * **comment**
  * **icon**
  * **onlyShowIn**
  * **notShowIn**
  * **tryExec**
  * **exec**
  * **path**
  * **terminal** - boolean
  * **mimeType**
  * **categories**
  * **url**

## Nested Elements ##

All the nested elements are used for localized content.

  * **name**
  * **genericName**
  * **comment**
  * **icon**

### Attributes of Nested Localized Content ###

  * **lang**
  * **country**
  * **encoding**
  * **modifier**
  * **value** - the actual localized content

## Examples ##
Some examples are provided in examples-{version}.tar.gz at http://code.google.com/p/ant-deb-task/downloads/list