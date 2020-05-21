# Dep 

Dep is a dependency management tool in golang. The best option is to create your project within your $GOPATH, cd into that directory and then call ```dep init```
Dep init creates 3 files : `Gopkg.toml` `Gopkg.lock` and `vendor`. When you do `dep init`, dep finds out all your dependencies(using
import paths) and gets all the dependencies of the highest compatible version.

## Gopkg.toml

This is the file where you mention constraints on the version of packages you imported in your project. This is not autofilled except in case of `dep init` i.e. setting up the project for the first time. If its a existing project, constraints are to be hand written or added using `dep ensure add package`. For handwritten, copy it from the Gopkg.lock after you have imported the package  and ran `dep ensure`.

## dep ensure

`dep ensure` makes sure that my project is in sync: that Gopkg.lock satisfies all the imports in my project, and all the rules in Gopkg.toml, and that vendor/ contains exactly what Gopkg.lock says it should. `dep ensure -vendor-only` takes a look at the existing Gopkg.lock and fills the vendor folder. dep ensure -no-vendor does not update the vendor but will update the Gopkg.lock file.

  

## Transitive Dependencies

These are dependencies which are not a dependency of the actual project but the dependency of a dependency you have added.
Since they are not imported by the project, dep ensure will remove it since its not a part of the imports of the actual project. In order to keep transitive dependencies , we need to either import it as a `dummy import` or add it as `required` in `Gopkg.toml`

 
  


