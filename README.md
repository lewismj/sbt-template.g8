# Scala sbt template (Multi-Module with App)

Curently under development...

A [giter8][1] template for [Scala][2] projects using [sbt][3].
This template sets up a multi-module project. It also includes an application that depends on the modules. 
An assembly plugin is referenced for building uber-jar of the application.

## Example Layout

~~~
+-- LICENSE
+-- README.md
+-- build.sbt
+-- module1
|   +-- src
|     +-- main
|       +-- scala
|         +-- com
|           +-- example
|             +-- myproject
|               +-- module1
|                 +-- Trait1.scala
+-- module2
|   +-- src
|     +-- main
|       +-- scala
|         +-- com
|           +-- example
|             +-- myproject
|               +-- module1
|                 +-- Trait1.scala
+-- app
|   +-- src
|     +-- main
|       +-- scala
|         +-- com
|           +-- example
|             +-- myproject
|               +-- app
|                 +-- HelloWorld.scala
+-- project
|  +-- Dependencies.scala
|  +-- Settings.scala
|  +-- build.properties
|  +-- plugins.sbt
~~~

[1]: https://github.com/n8han/giter8
[2]: http://www.scala-lang.org/
[3]: http://github.com/harrah/xsbt/

