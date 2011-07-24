This is a sbt 0.10.x plugin for scct the scala code coverage tool.

* scct: http://mtkopone.github.com/scct/

## Commands:

* coverage:compile
* coverage:test
* coverage:doc

coverage:test and coverage:doc do the same, so that if you run coverage:package-doc, you get your coverage report packaged.

docDirectory is reused for the coverage report directory

## Compiling from Source

To compile the plugin from source put the source in .sbt/project/plugins/project and add the plugin as a dependency in .sbt/project/plugins/build.sbt

libraryDependencies += "ch.craven" %% "scct-plugin" % "0.2"

Don't forget to set the sbt version you're using for your project by editing the sbt-scct/project/build.properties file.