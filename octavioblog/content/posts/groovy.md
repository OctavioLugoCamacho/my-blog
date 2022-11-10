+++
title = "Groovy"
date = 2022-10-15
tags = ["Groovy", "Course", "Experience"]
+++

![Groovy](../../groovy.svg)

# What is Groovy?
Groovy is powerful, optionally typed and dynamic language to develop an application on Java Platform where its syntax is Java-like. Its typing discipline is strong, static, and dynamic. The best things about Groovy are that since it extends JDK, it accepts Java code. Groovy can be used as both programming and scripting Language. Groovy is a superset of Java which means Java program will run in Groovy environment but vice-versa may or may not be possible. Whereas Java is strongly and statically typed programming language. 

You can check the documentation [Here](https://groovy-lang.org/syntax.html "Here")!

# How to install Groovy with SDK?
### SDKMAN! (The Software Development Kit Manager)
This tool makes installing Groovy on any Bash platform (Mac OSX, Linux, Cygwin, Solaris or FreeBSD) very easy.

Simply open a new terminal and enter:

```
$ curl -s get.sdkman.io | bash
```

Follow the instructions on-screen to complete installation.

Open a new terminal or type the command:

```
$ source "$HOME/.sdkman/bin/sdkman-init.sh"
```

Then install the latest stable Groovy:

```
$ sdk install groovy
```

After installation is complete and you’ve made it your default version, test it with:

```
$ groovy -version
```

That’s all there is to it!

# Let's do an exercise
### Multiples of 3 or 5
If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below 1000.

```groovy
def sum = 0

for(int i in 1..999) {
  if (i % 3 == 0 || i % 5 == 0) { sum += i}
}

println sum
```

We need to run the next command:

```
$ groovy exercise.groovy
```

And we get the reult that is 233168.