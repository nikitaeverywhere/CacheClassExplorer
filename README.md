# CacheUMLExplorer
An UML Class explorer for InterSystems Caché.

##### Key features
+ Build class diagrams;
+ Build diagrams for any package or subpackage;
+ Edit diagrams after build;
+ Export diagrams as an image;
+ View class methods code;
+ Zoom in and out, explore big packages and more.

## Screenshots

![Demo](https://cloud.githubusercontent.com/assets/4989256/7622499/9cb98048-f9d8-11e4-9c27-4257e53ec70d.png)

## Installation

To install Caché UML Explorer, you need to import UMLExplorer package to Caché and then set up a WEB-application.

###### Import classes to Caché
To install Caché UML class explorer, download the [latest release](https://github.com/intersystems-ru/UMLExplorer/releases) or build project by yourself. Then import XML file inside <code>Cache</code> directory of archive or directory.

###### Set up WEB application
When you have imported and compiled <b>UMLExplorer package</b> in Caché, make sure the namespace is the same you have imported classes to. Then go to <code>system management portal -> administering -> security -> applications -> web applications</code> and create there a new web application. Fill the <code>name</code> field of it with <code>/UMLExplorer</code> (slash is required) and set the value of <code>dispatch class</code> to <code>UMLExplorer.Router</code>. Click save. Now your WEB application is ready.

###### Use it
Visit <code>[server domain and port]/UMLExplorer/</code> (with slash at end) to enter application.

## Build

To build project, you need [NodeJS](https://nodejs.org) platform to be installed. Then, clone source code and run <code>npm install</code> from the root of the project. This will install all necessary modules from NPM. Also run <code>npm install -g gulp</code> if you have no gulp builder in your modules.

After that and each next time just run <code>gulp</code> command from the project root. This will generate <code>build</code> directory, where you will found all what you need.
