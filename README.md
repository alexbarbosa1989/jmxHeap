# jmxHeap
JBoss EAP jmx basic client


USAGE

1. Clone project in local environment:

~~~
git clone https://github.com/alexbarbosa1989/jmxHeap
~~~

2. Look the file distribution:

~~~
$ tree .
.
└── src
    └── jmxHeap
        └── jmxTest.java
~~~

3. navigate into the src/ directory

~~~
cd src/
~~~

4. Compile jmxTest.java class, including **jboss-client.jar** full path in the classpath

~~~
javac -classpath .:${CLIENT-PATH}/jboss-client.jar jmxHeap/jmxTest.java
~~~

5. Review if .class file was generated:

~~~
$ tree .
.
└── src
    └── jmxHeap
        ├── jmxTest.class
        └── jmxTest.java
~~~

6. Execute the class pointing to the running JBoss EAP/Wildfly instance, also including **jboss-client.jar** full path in the classpath

~~~
java -classpath .:${CLIENT-PATH}/jboss-client.jar jmxHeap.jmxTest
~~~
