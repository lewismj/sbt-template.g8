# Scala sbt template (Multi-Module with App)

A [giter8][1] template for Scala projects using sbt. 
This template sets up a multi-module project. It also includes an application that depends on the modules. 
An assembly plugin is referenced for building uber-jar of the application.

## Usage

```sbt new lewismj/sbt-template.g8```

You can then run:

~~~
sbt compile
sbt publish-local
sbt assembly
~~~

The assembly command will put the uber-jar into a top level 'bin' directory.

## Example Layout

~~~
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
|                 +-- Trait2.scala
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
