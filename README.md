# Groovy/Grails Tutorial
(description- what technologies and versions will be used)

## Setup:

Download the following and export the files into the directory of your choice: 

  1. Java: On the oracle website, accept the terms and agreements and download the file. Once downloaded it will be installed.- [download from here](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)
  2. Grails - [download from here](https://grails.org/download.html)
  3. Groovy - [download from here]()
  
  Now that you have the needed files, start up the powershell and run the following commands to setup the environment variables (**be sure to use your own file paths**):
~~~ sh
Method Parameters:
  *name
  *path too directory
  *level of environment (ie. User-for specific user, Machine-entire system)

[Environment]::SetEnvironmentVariable("JAVA_HOME", "C:\Program Files (x86)\Java\jdk1.7.0_79", "Machine")
[Environment]::SetEnvironmentVariable("GRAILS_HOME", "C:\groovy-grails-dev\grails-3.1.8", "Machine")
[Environment]::SetEnvironmentVariable("GROOVY_HOME", "C:\groovy-grails-dev\groovy-2.4.7", "Machine")
~~~


  Now that we have the envirment variables, we need to add them to our path with the following commands (**again, be sure to use your own file paths**):
~~~ sh
[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\groovy-grails-dev\grails-3.1.8\bin", [EnvironmentVariableTarget]::Machine)
[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\groovy-grails-dev\grails-3.1.8\bin", [EnvironmentVariableTarget]::Machine)
[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\groovy-grails-dev\groovy-2.4.7\bin", [EnvironmentVariableTarget]::Machine)
~~~
## References:
(documentation links, videos ect)
