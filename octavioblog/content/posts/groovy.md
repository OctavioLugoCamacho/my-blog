+++
title = "What is Groovy and how do I install it?"
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
### Sum square difference
The sum of the squares of the first ten natural numbers is, 1^2+2^2+...+10^2 = 385

The square of the sum of the first ten natural numbers is, (1+2+...+10)^2 = 55^2 = 3025 Hence the difference between the sum of the squares of the first ten natural numbers and the square of the sum is 3025 - 385 = 2640.

Find the difference between the sum of the squares of the first one hundred natural numbers and the square of the sum.

```groovy
def num = 100

def sumOfSquares = (num * (num + 1)) / 2
sumOfSquares *= sumOfSquares

def squareOfSum = (num * (num + 1) * (2 * num + 1)) / 6

def difference = sumOfSquares - squareOfSum
```

We need to run the next command:

```
$ groovy exercise.groovy
```

And we get the reult that is 233168.