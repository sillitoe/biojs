BioJS 2.0
=========

```

88888888ba  88                     88  ad88888ba      ad888888b,  
88      "8b ""                     88 d8"     "8b    d8"     "88  
88      ,8P                        88 Y8,                    a8P  
88aaaaaa8P' 88  ,adPPYba,          88 `Y8aaaaa,           ,d8P"   
88""""""8b, 88 a8"     "8a         88   `"""""8b,       a8P"      
88      `8b 88 8b       d8         88         `8b     a8P'        
88      a8P 88 "8a,   ,a8" 88,   ,d88 Y8a     a8P    d8"          
88888888P"  88  `"YbbdP"'   "Y8888P"   "Y88888P"     88888888888 

 ```

Annoucements
----------------

We recently switched to a new concept, so maybe you are looking for the old [BioJS 1](https://github.com/biojs/biojs1)?

You can already browse the new [registry][registry]. Transition of components from BioJS1 is in progress.

Objectives
----------

* Represent consistently biological information across different projects
* Ease discovery, test and integration of graphical components
* Standardize and facilitate components development

What is different in BioJS 2.0?
-------------------------------

↝ [Summary presentation](https://docs.google.com/presentation/d/17Q4olwMEd0hFKa0MA01Dx9RHEWbNiI1hJ0Ng2v_1D30/) of the differences between BioJS1 and BioJS 2.0.

Upgrading to BioJS 2.0
----------------------

Old Components of BioJS 0.1 can rely on [biojs-legacy][migrationguide]. But we highly encourage you to write your code more [modular][101].

We can ensure that if you have contributed with a component in the BioJS1 registry, it will continue to work in BioJS2.
In fact we will script the migration and at some day in November or December migrate all remaining BioJS1 components.
The final update of the EBI registry will be at the end of this year.


Contact
-------

↝ [There are many ways to contact us](http://biojs.net/get_involved.html)

For technical queries (questions, suggestions, proposal or bug reports) [Github issues](https://github.com/biojs/biojs/issues) are preferred.


Why is nothing in this repo?
---------------------------

For BioJS 2.0 every component is a separate github repository - here you see only the template project for our  [101 tutorial][101]. To search for a package, visit our [registry][registry].

Documentation
--------------

We are working on a new platform [edu.biojs.net](http://edu.biojs.net/).
[Pull requests](https://github.com/biojs/tutorials) are welcome.

For beginners there is a [BioJS 2 101 tutorial series][101].
For a quick migration to BioJS 2 we created [this document][migrationguide].

What is a package?
------------------

A tiny building block like a FASTA parser or a visualization piece. If it obeys the rule "do one thing and do it well" , then it is (most likely) a package. The BioJS packages are published on the JavaScript package manager [npm](npmjs.org).

What do I need to use a package?
-------------------------------

A web browser. For convenience you can grab a recent CDN version of

* [all parsers](https://github.com/biojs/biojs-meta-parser)
* [all visulization components](https://github.com/biojs/biojs-meta-vis)

Normally the author provides also provides you with a minimized version of his component, but you can always easily build it yourself by running "npm run build-browser".

How do I use a package?
-------------------------------

In general the `README.md` of each project should explain you how to interact with it.

Guidelines
-----------

We have a few guidelines like 

* [biojs-events](https://github.com/biojs/biojs-events) (Convention for the Observer pattern)
* [example snippets](https://github.com/greenify/biojs-sniper) (coming soon: generic snippets on JSBin)

Especially the snippets should give you a quick start on how to use a component.

Gold standards
--------------

Our [gold standards](https://github.com/biojs/biojs/wiki/Gold-standards) are conventions we highly encourage you to follow (especially for JS beginners). They will help you to create a great package!

What do I need to develop?
-------------------------------

* [git](https://try.github.io/levels/1/challenges/1)
* [npm](http://nodejs.org/download/)


[Detailed installation instructions](http://edu.biojs.net/series/101/02_getting_started.html).

Even tough you can easily install node on Windows, a Unix-like OS is generally a more productive development enviroment.

How to build a BioJS package
----------------------------

In the package folder

```
npm install # this downloads all the dependencies of a package
npm test # optional
npm run build-browser # this will generate a JS file usuable in every browser (normally in the build folder)
```

Working examples of the component can be found in the [`snippets`](https://github.com/greenify/biojs-sniper) folder of a package.


How to create a package?
-------------------------

↝ read our [guide][101]


How to publish a package?
-------------------------

Publish it on [npm](npmjs.org) and just send us a pull request to the [index.toml](https://github.com/biojs/registry/blob/master/index.toml).

License
-------

[Apache 2](http://www.apache.org/licenses/LICENSE-2.0)


[101]: http://edu.biojs.net/categories/101_tutorial/index.html
[migrationguide]: http://edu.biojs.net/tutorials/aQuickGuideForMigrating.html
[registry]: http://registry.biojs.net/client/
