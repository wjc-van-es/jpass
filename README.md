<p align="center">
 <img src="https://raw.githubusercontent.com/gaborbata/jpass/master/resources/bannerReadMe.png" width=750 align="center">
</p>

JPass [![Build Status](https://travis-ci.org/gaborbata/jpass.svg?branch=master)](https://travis-ci.org/gaborbata/jpass) ![Java CI with Maven](https://github.com/gaborbata/jpass/workflows/Java%20CI%20with%20Maven/badge.svg)
=====

Overview
--------
JPass is a simple, small, portable password manager application with strong encryption. It allows you to store user names, passwords, URLs and generic notes in an encrypted file protected by one master password.

Features:

* Strong encryption - AES-256-CBC algorithm (SHA-256 is used as password hash)
* Portable - single jar file which can be carried on a USB stick
* Built-in random password generator
* Organize all your user name, password, URL and notes information in one file
* Data import/export in XML format

![JPass](https://raw.githubusercontent.com/gaborbata/jpass/master/resources/jpass-capture.png)

Usage
-----
Java 8 or later is recommended to run JPass. Most platforms have a mechanism to execute `.jar` files (e.g. double click the `jpass-0.1.21-SNAPSHOT.jar`).
You can also run the application from the command line by typing (the password file is optional):

    java -jar jpass-0.1.21-SNAPSHOT.jar [password_file]

Download
--------
You can find the latest distribution package under the [releases](https://github.com/gaborbata/jpass/releases) link.

How to compile
--------------
* Maven: `mvn clean package`
* Gradle: `gradle clean build`
* sbt: `sbt clean package`

Configuration
-------------
Default configurations can be overridden in `jpass.properties` file:

| Configuration key                  | Value type | Default value  |
| ---------------------------------- | ---------- | -------------- |
| ui.theme.dark.mode.enabled         | boolean    | false          |
| clear.clipboard.on.exit.enabled    | boolean    | false          |
| default.password.generation.length | integer    | 14             |
| date.format                        | string     | yyyy-MM-dd     |
| entry.details                      | list       | TITLE,MODIFIED |

Contributors
------------
Thanks for Jibbie R. Eguna (@jbeguna04) for the nice application logo.
