## Available Projects for Scala 2.12

Library maintainers, library users, please [submit a pull request](https://github.com/scala/make-release-notes/edit/2.12.x/projects-2.12.md) and let the world know what libraries are available.

### Scala 2.12.0-RC1

Scala modules, add in sbt using `libraryDependencies += ...`

    "org.scala-lang.modules"           %% "scala-xml"                 % "1.0.5"
    "org.scala-lang.modules"           %% "scala-parser-combinators"  % "1.0.4"
    "org.scala-lang.modules"           %% "scala-swing"               % "2.0.0-M2"
    "org.scala-lang.modules"           %% "scala-async"               % "0.9.6-RC5"
    "org.scala-lang.modules"           %% "scala-java8-compat"        % "0.8.0-RC7"

Testing frameworks, add in sbt using `libraryDependencies += ... % "test"`

    "org.scalatest"                    %% "scalatest"                 % "3.0.0"           % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.13.2"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.12.5"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.11.6"          % "test"
    "org.specs2"                       %% "specs2-core"               % "3.8.5"           % "test"
    "com.github.scalaprops"            %% "scalaprops"                % "0.3.4"           % "test"

Other libraries, add in sbt using `libraryDependencies += ...`

    "edu.eckerd"                       %% "google-api-scala"          % "0.1.0"
    "org.scalaz"                       %% "scalaz-core"               % "7.2.6"
    "org.scalaz"                       %% "scalaz-core"               % "7.1.10"
    "org.scalactic"                    %% "scalactic"                 % "3.0.0"
    "org.typelevel"                    %% "macro-compat"              % "1.1.1"
    "org.typelevel"                    %% "discipline"                % "0.7"
    "org.typelevel"                    %% "machinist"                 % "0.5.0"
    "com.github.nscala-time"           %% "nscala-time"               % "2.14.0"
    "com.github.xuwei-k"               %% "zeroapply"                 % "0.2.1"
    "com.github.xuwei-k"               %% "msgpack4z-core"            % "0.3.5"
    "com.github.xuwei-k"               %% "applybuilder"              % "0.2.2"
    "org.scodec"                       %% "scodec-bits"               % "1.1.1"
    "co.fs2"                           %% "fs2-core"                  % "0.9.0"
    "co.fs2"                           %% "fs2-io"                    % "0.9.0"
    "com.github.ghik"                  %% "silencer-lib"              % "0.5"
    "com.typesafe.akka"                %% "akka-actor"                % "2.4.10"
    "com.typesafe.akka"                %% "akka-stream"               % "2.4.10"
    "com.typesafe.akka"                %% "akka-http-core"            % "2.4.10"

Note that [Shapeless](https://github.com/milessabin/shapeless) will not be
published for 2.12.0-RC1; see [#5395](https://github.com/scala/scala/pull/5395).

Compiler plugins, add in sbt using `addCompilerPlugin(...)`:

    "org.spire-math"                   %% "kind-projector"            % "0.8.2"
    "org.scalamacros"                  %% "paradise"                  % "2.1.0"
    "com.typesafe.genjavadoc"          %% "genjavadoc-plugin"         % "0.10"
    "com.github.ghik"                  %% "silencer-plugin"           % "0.5"
    "org.psywerx.hairyfotr"            %% "linter"                    % "0.1.15"

Sbt plugins. Most plugins do not need to be re-published for 2.12, but certain plugins did require changes. Add using `addSbtPlugin`:

    "org.scala-js"                     %  "sbt-scalajs"               % "0.6.12"

### Scala 2.12.0-M5

Scala modules, add in sbt using `libraryDependencies += ...`

    "org.scala-lang.modules"           %% "scala-xml"                 % "1.0.5"
    "org.scala-lang.modules"           %% "scala-parser-combinators"  % "1.0.4"
    "org.scala-lang.modules"           %% "scala-swing"               % "2.0.0-M2"
    "org.scala-lang.modules"           %% "scala-java8-compat"        % "0.8.0-RC3"

Testing frameworks, add in sbt using `libraryDependencies += ... % "test"`

    "org.scalatest"                    %% "scalatest"                 % "3.0.0"           % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.13.2"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.12.5"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.11.6"          % "test"
    "org.specs2"                       %% "specs2-core"               % "3.8.4"           % "test"

Other libraries, add in sbt using `libraryDependencies += ...`

    "org.scalactic"                    %% "scalactic"                 % "3.0.0"
    "com.typesafe.akka"                %% "akka-actor"                % "2.4.8"
        // and other akka libraries such as akka-stream, akka-http, etc. (same version number)
    "org.scalaz"                       %% "scalaz-core"               % "7.3.0-M4"
    "org.scalaz"                       %% "scalaz-core"               % "7.2.4"
    "org.scalaz"                       %% "scalaz-core"               % "7.1.9"
    "com.chuusai"                      %% "shapeless"                 % "2.3.1"
    "org.typelevel"                    %% "macro-compat"              % "1.1.1"
    "com.github.nscala-time"           %% "nscala-time"               % "2.12.0"
    "org.scodec"                       %% "scodec-bits"               % "1.1.0"
    "org.scodec"                       %% "scodec-core"               % "1.10.2"
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.8.3a"
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.8.3"
    "co.fs2"                           %% "fs2-core"                  % "0.9.0-RC1"
    "co.fs2"                           %% "fs2-io"                    % "0.9.0-RC1"
    "com.typesafe.slick"               %% "slick"                     % "3.2.0-M1"
    "io.spray"                         %% "spray-json"                % "1.3.2"
    "com.github.nscala-time"           %% "nscala-time"               % "2.12.0"

Compiler plugins, add in sbt using `addCompilerPlugin(...)`:

    "org.scalamacros"                  %% "paradise"                  % "2.1.0"

Sbt plugins. Most plugins do not need to be re-published for 2.12, but certain plugins required changes. Add using `addSbtPlugin`:

    "org.scala-js"                     %  "sbt-scalajs"               % "0.6.11"
    "com.typesafe"                     %  "sbt-mima-plugin"           % "0.1.9"

### Scala 2.12.0-M4

Scala modules, add in sbt using `libraryDependencies += ...`

    "org.scala-lang.modules"           %% "scala-xml"                 % "1.0.5"
    "org.scala-lang.modules"           %% "scala-parser-combinators"  % "1.0.4"
    "org.scala-lang.modules"           %% "scala-swing"               % "2.0.0-M2"
    "org.scala-lang.modules"           %% "scala-java8-compat"        % "0.8.0-RC1"

Testing frameworks, add in sbt using `libraryDependencies += ... % "test"`

    "org.scalatest"                    %% "scalatest"                 % "2.2.6"           % "test"
    "org.scalatest"                    %% "scalatest"                 % "3.0.0-M16-SNAP4" % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.11.6"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.12.5"          % "test"
    "org.scalacheck"                   %% "scalacheck"                % "1.13.1"          % "test"
    "org.specs2"                       %% "specs2-core"               % "3.7.3.1"         % "test"

Other libraries, add in sbt using `libraryDependencies += ...`

    "org.scalactic"                    %% "scalactic"                 % "2.2.6"
    "org.scalactic"                    %% "scalactic"                 % "3.0.0-M16-SNAP3"
    "org.typelevel"                    %% "macro-compat"              % "1.1.1"
    "com.chuusai"                      %% "shapeless"                 % "2.2.5"
    "com.chuusai"                      %% "shapeless"                 % "2.3.0"
    "com.github.nscala-time"           %% "nscala-time"               % "2.12.0"
    "org.scalaz"                       %% "scalaz-core"               % "7.1.7"
    "org.scalaz"                       %% "scalaz-core"               % "7.2.2"
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.8.1"
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.8.1a"
    "org.scodec"                       %% "scodec-bits"               % "1.0.12"
    "org.scodec"                       %% "scodec-bits"               % "1.1.0"
    "com.github.scopt"                 %% "scopt"                     % "3.4.0"
    "com.typesafe.akka"                %% "akka-actor"                % "2.4.4"

Compiler plugins, add in sbt using `addCompilerPlugin(...)`:

    "org.scalamacros"                  %% "paradise"                  % "2.1.0"
    "org.spire-math"                   %% "kind-projector"            % "0.8.0"

Sbt plugins. Most plugins do not need to be re-published for 2.12, but certain plugins required changes. Add using `addSbtPlugin`:

    "org.scala-js"                     %  "sbt-scalajs"               % "0.6.8"
    "com.typesafe"                     %  "sbt-mima-plugin"           % "0.1.9"

### Scala 2.12.0-M3

Scala modules, add in Sbt using `libraryDependencies += ...`

    "org.scala-lang.modules"           %% "scala-xml"                 % "1.0.5"
    "org.scala-lang.modules"           %% "scala-parser-combinators"  % "1.0.4"
    "org.scala-lang.modules"           %% "scala-swing"               % "2.0.0-M2"
    "org.scala-lang.modules"           %% "scala-java8-compat"        % "0.7.0"

Testing frameworks, add in Sbt using `libraryDependencies += ...`

    "org.scalacheck"                   %% "scalacheck"                % "1.11.6"
    "org.scalacheck"                   %% "scalacheck"                % "1.12.5"
    "org.scalatest"                    %% "scalatest"                 % "2.2.5-M3"
    "org.specs2"                       %% "specs2-core"               % "3.7.1"

Other libraries, add in Sbt using `libraryDependencies += ...`

    "org.scalaz"                       %% "scalaz-core"               % "7.1.4"
    "org.scalaz"                       %% "scalaz-core"               % "7.0.8"
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.8a"
    "org.scalactic"                    %% "scalactic"                 % "2.2.5-M3"
    "org.scodec"                       %% "scodec-bits"               % "1.0.10"
    "com.chuusai"                      %% "shapeless"                 % "2.2.5"
    "org.scalikejdbc"                  %% "scalikejdbc"               % "2.3.5"
    "com.github.scopt"                 %% "scopt"                     % "3.4.0"

Sbt plugins, add using `addSbtPlugin`; note that sbt 0.13 plugins always run on Scala 2.10, so most plugins don't need any changes to work with projects targeting 2.12; but the following plugins did need changes

    "org.scala-js"                     %  "sbt-scalajs"               % "0.6.5"
    "com.typesafe"                     %  "sbt-mima-plugin"           % "0.1.8"

### Scala 2.12.0-M2

Libraries, add using `libraryDependencies += ...`

    "org.scalacheck"                   %% "scalacheck"                % "1.11.6"
    "org.scalacheck"                   %% "scalacheck"                % "1.12.4"
    "org.scalatest"                    %% "scalatest"                 % "2.2.5-M2"
    "org.scalactic"                    %% "scalactic"                 % "2.2.5-M2"
    "com.chuusai"                      %% "shapeless"                 % "2.2.5"
    "org.scalaz"                       %% "scalaz-core"               % "7.0.8"
    "org.scalaz"                       %% "scalaz-core"               % "7.1.3"
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.7.2"     // for scalaz 7.0
    "org.scalaz.stream"                %% "scalaz-stream"             % "0.7.2a"    // for scalaz 7.1
    "com.github.nscala-time"           %% "nscala-time"               % "2.0.0"
    "org.scodec"                       %% "scodec-bits"               % "1.0.9"

may or may not be usable, see [issue](https://github.com/etorreborre/specs2/issues/399):

    "org.specs2"                       %% "specs2-core"               % "3.6.3"

### Scala 2.12.0-M1

Libraries, add using `libraryDependencies += ...`

    "org.scalacheck"                   %% "scalacheck"                % "1.11.6"
    "org.scalatest"                    %% "scalatest"                 % "2.2.5-M1"
    "org.scalactic"                    %% "scalactic"                 % "2.2.5-M1"
    "org.scalaz"                       %% "scalaz-core"               % "7.0.7"
    "org.scalaz"                       %% "scalaz-core"               % "7.1.2"
    "com.github.nscala-time"           %% "nscala-time"               % "2.0.0"

Compiler Plugins, add using `addCompilerPlugin(...)`:

    "org.spire-math"                   %% "kind-projector             % "0.5.4" // resolvers += "bintray/non" at "http://dl.bintray.com/non/maven"
