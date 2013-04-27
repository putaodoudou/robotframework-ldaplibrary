robotframework-ldaplibrary
=============

A Java based Robot Framework library for accessing an LDAP directory.

Description
-----------

LdapLibrary is a library for Robot Framework that provides keywords for
interacting with an LDAP directory.

Documentation for currently available keywords is in the doc directory (generated by libdoc).

Dependencies
------------

- [UnboundID LDAP SDK](https://www.unboundid.com/products/ldap-sdk/)
- [Javalib Core](https://github.com/robotframework/JavalibCore)

Installation
------------

Either [download](https://s3-eu-west-1.amazonaws.com/maven-repository-jrkoiter/release/nl/fuselogic/robotframework-ldaplibrary/0.1/robotframework-ldaplibrary-0.1.jar) the jar file of the current version directly, or build the library from source by following the steps below. A working Maven installation is assumed:

1. Get the source of the robotframework-ldaplibrary (ie. this library)
2. Build the library. It will be generated in the subdirectory "target".

		mvn package

Usage
-----

1. Obtain the [Javalib Core](https://github.com/robotframework/JavalibCore) library
2. Obtain the [UnboundID LDAP SDK](https://www.unboundid.com/products/ldap-sdk/) library
3. Add "LdapLibrary" to your test suite's Settings table, e.g:
   
        *** Settings ***
        | Library | nl.fuselogic.robotframework.libraries.oim.LdapLibrary |

5. Run your test suites using Jython/jybot with all libraries in the classpath

		robotframework-ldaplibrary-*.jar
		javalib-core-1.1.jar
		unboundid-ldapsdk-2.3.1

Issues
------
Only a very limited set of features is currently exposed through this library. It is a work in progress.
If you encounter any problems or have a feature request please open an issue on this project's GitHub issue tracker.

License
-------
Copyright 2013 FuseLogic BV

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.