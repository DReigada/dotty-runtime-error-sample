# Steps to reproduce
1. sbt run
2. change `case Bar extends Foo[Int]` to `case Bar extends Foo[String]` (in `Foo.scala`)
3. sbt run
4. ???
5. `java.lang.NoSuchFieldError: Bar`

If you run `sbt clean` between steps 2 and 3 the program works.