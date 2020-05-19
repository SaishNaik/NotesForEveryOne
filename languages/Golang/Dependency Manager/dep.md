# Dep 

Dep is a dependency management tool in golang. The best option is to create your project within your $GOPATH, cd into that directory and then call ```dep init```
Dep init creates 3 files : `Gopkg.toml` `Gopkg.lock` and `vendor`. When you do `dep init`, dep finds out all your dependencies(using
import paths) and gets all the dependencies of the highest compatible version.


