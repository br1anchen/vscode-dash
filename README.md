# Visual Studio Code Dash

[Dash](https://kapeli.com/dash) documentation integration for [Visual Studio Code](https://code.visualstudio.com/)

> Dash is an API Documentation Browser and Code Snippet Manager for MacOS

[![Build Status](https://travis-ci.org/deerawan/vscode-dash.svg?branch=master)](https://travis-ci.org/deerawan/vscode-dash) [![Coverage Status](https://coveralls.io/repos/deerawan/vscode-dash/badge.svg?branch=master&service=github)](https://coveralls.io/github/deerawan/vscode-dash?branch=master)

![vscode dash](https://raw.githubusercontent.com/deerawan/vscode-dash/master/images/vscode-dash.gif)

## Installation
Type `cmd + shift + p` to launch command palette and choose `Extensions: Install Extension`. Search this package and install.

## Usage
Get the text under your cursor or selected first.

- Pressing `ctrl + h`. It will search for current specific documentation depends on language.
- Pressing `ctrl + alt + h`. It will search for all documentation.

## Supported Docsets
This plugin supports almost all docset configuration based on [https://kapeli.com/dash_plugins](Dash Mapping)

Language | Dash Docset Keys | Docset Plugin Setting
------------ | ------------- | -------------
C++ | cpp,net,boost,qt,cvcpp,cocos2dx,c,manpages | dash.docset.cpp
C# | net,mono,unity3d | dash.docset.csharp
Clojure | clojure | dash.docset.clojure
CoffeeScript | coffee | dash.docset.coffee
CSS | css,bootstrap,foundation,less,awesome,cordova,phonegap | dash.docset.css
Dart | dartlang,polymerdart,angulardart | dash.docset.dart
Elixir | elixir | dash.docset.elixir
Erlang | erlang | dash.docset.erlang
Go | go,godoc | dash.docset.go
Haskell | haskell | dash.docset.haskell
HTML | html,svg,css,bootstrap,foundation,awesome,statamic,javascript,jquery,jqueryui,jquerym,angularjs,backbone,marionette,meteor,moo,prototype,ember,lodash,underscore,sencha,extjs,knockout,zepto,cordova,phonegap,yui | dash.docset.html
Jade | jade | dash.docset.jade
Java | java,javafx,grails,groovy,playjava,spring,cvj,processing | dash.docset.java
JavaScript | javascript,jquery,jqueryui,jquerym,react,angularjs,backbone,marionette,meteor,sproutcore,moo,prototype,bootstrap,foundation,lodash,underscore,ember,sencha,extjs,titanium,knockout,zepto,yui,d3,svg,dojo,coffee,nodejs,express,grunt,mongoose,moment,require,awsjs,jasmine,sails,sinon,chai,html,css,cordova,phonegap,unity3d | dash.docset.javascript
Less | less | dash.docset.less
Lua | lua,corona | dash.docset.lua
Markdown | markdown | dash.docset.markdown
Objective-C | iphoneos,macosx,watchos,tvos,appledoc,cocos2d,cocos3d,kobold2d,sparrow,c,manpages | dash.docset.objective-c
Perl | perl,manpages | dash.docset.perl
PHP | php,wordpress,drupal,zend,laravel,yii,joomla,ee,codeigniter,cakephp,phpunit,symfony,typo3,twig,smarty,craft,phpp,html,statamic,mysql,sqlite,mongodb,psql,redis | dash.docset.php
Processing | processing | dash.docset.pde
Puppet | puppet | dash.docset.puppet
Python | python,django,twisted,sphinx,flask,tornado,sqlalchemy,numpy,scipy,salt,pandas,matplotlib,cvp | dash.docset.python
R | r | dash.docset.r
Ruby | ruby,rubygems,rails | dash.docset.ruby
Rust | rust | dash.docset.rust
Sass | sass,compass,bourbon,neat,susy,css | dash.docset.sass
Scala | scala,akka,playscala | dash.docset.scala
Shell Scripts | bash,manpages | dash.docset.shellscript
SQL | mysql,sqlite,psql | dash.docset.sql
Stylus | stylus | dash.docset.stylus
Swift | swift,iphoneos,macosx,watchos,tvos,appledoc | dash.docset.swift
Tcl | tcl | dash.docset.tcl
TypeScript | typescript | dash.docset.typescript
YAML | chef,ansible | dash.docset.yaml

### Added docset in this plugin
Language | Dash Docset Keys | Plugin Setting
------------ | ------------- | -------------
React | react | dash.docset.javascriptreact

### What is `Dash Docset Keys`?
You can find dash docset key in Dash application.

![dash docset key](https://raw.githubusercontent.com/deerawan/vscode-dash/master/images/dash-docset-key.jpg)

## Change Docset Configuration
You can change docset in `settings.json` or pressing `cmd + ,`.
Every configuration start with `dash.docset.xxx`. See Supported Docset table above to find Docset Plugin setting.

Let's we change typescript docset by adding new docset "javascript". So, whenever we search from typescript files, it will search in typescript and javascript docset.

The result will look like below:

```
// settings.json
"dash.docset.typescript": [
    "typescript",
    "javascript", // we add new docset here
]
```

## License
MIT
