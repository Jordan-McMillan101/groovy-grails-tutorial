# Groovy/Grails Tutorial

This tutorial is for someone who is new to
**Technology stack:**
  *


## Environment Setup (for Windows):

Download the following and export the files into the directory of your choice: 

  1. Java - On the oracle website, accept the terms and agreements and download the file. Once downloaded it will prompt you to finish the installation.- [download from here](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)
  2. Grails - [download from here](https://grails.org/download.html)
  3. Groovy - [download from here]()
  

Now that you have the needed files, start up powershell (**as administrator**) and run the following commands to setup the environment variables (**be sure to use your own file paths**):

~~~ sh
Method Parameters:
   *name
   *path too directory
   *level of environment (ie. User-for specific user, Machine-entire system)

[Environment]::SetEnvironmentVariable("JAVA_HOME", "C:\Program Files (x86)\Java\jdk1.7.0_79", "Machine")
[Environment]::SetEnvironmentVariable("GRAILS_HOME", "C:\groovy-grails-dev\grails-3.1.8", "Machine")
[Environment]::SetEnvironmentVariable("GROOVY_HOME", "C:\groovy-grails-dev\groovy-2.4.7", "Machine")
~~~


 Now that we have the environment variables created, we need to add their \bin folders to our path with the following commands (**again, be sure to use your own file paths**):
 
  
~~~ sh
[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\Program Files (x86)\Java\jdk1.7.0_79\bin", [EnvironmentVariableTarget]::Machine)
[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\groovy-grails-dev\grails-3.1.8\bin", [EnvironmentVariableTarget]::Machine)
[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\groovy-grails-dev\groovy-2.4.7\bin", [EnvironmentVariableTarget]::Machine)
~~~


To double check that everything is ready to go run the following command in the terminal and you should be able to see the newly added items (** before you run this command restart your powershell**):

~~~ sh
  Get-ChildItem Env:
~~~


###Now choose your favorite text editor and start one of the following tutorials:
  *tut 1
  *tut 2
  *tut 3



## References:
(documentation links, videos ect)
* [Grails Documentation](https://grails.org/documentation.html)
* [Groovy Documentation](http://groovy-lang.org/documentation.html)
* [Seminar on building a twitter clone with groovy/grails](https://www.youtube.com/watch?v=8d1hp8n1stA)
