# A Clojure playground for fun & curiosity

Notes : 
- A JVM language,compiles to JVM bytecode (supports all Java LTS releases)
- Can consume Java library code (think FFI)
- it can do Runtime Polymorphism
- it features concurrent programming
- A member of the Lisp family language
- Resources seemed scarce and dispersed, and deprecated
- Some instructions were unclear regarding the tooling, the tooling seem possible in 3 ways : deps.dn, "in leiningen", in maven

Leiningen is the Swiss Army Knife of Clojure development. It handles:
Project compilation. Deployment of library code. package/dependency management.
It's a lesser cargo for Clojure

If a port is specified to the docker image, it will output
the following error message :" WARNING: Implicit use of clojure.main with options is deprecated, use -M
Execution error (FileNotFoundException) at java.io.FileInputStream/open0 (FileInputStream.java:-2).
-p (No such file or directory) "


## Requirements
Your system needs to have these installed : Java, bash, curl, rlwrap

### Commands

#### try via Docker

clone


```shell
git clone git@github.com:Neal-C/hello-clojure.git
```

build & run


```shell
docker build -t clojure:hello .
docker run clojure:hello
```

or local install 

```shell
curl -L -O https://github.com/clojure/brew-install/releases/latest/download/linux-install.sh
chmod +x linux-install.sh
sudo ./linux-install.sh
```
To install to a custom location (like /opt/infrastructure/clojure), use the option --prefix:
```shell
sudo ./linux-install.sh --prefix /opt/infrastructure/clojure
```

- To create a brand new project

```shell
lein new helloworld
```

