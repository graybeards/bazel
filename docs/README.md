# Bazel and Bagels

> Documenting our journey to using Bazel for our large enterprise Angular/AngularjS application

## Where did we start

## Goals
1. Build Login SPA with bazel (requires myadp/common & espresso)
1. Horse race: Repeatedly build the Login SPA on Jenkins - **webpack** vs. **bazel**

## TODOs
* Make a module in espresso/core/components
    * Is there a bug with sass_binary or should we write our own to make files relative. Or option to ngc to say where root of assets are located.
* Look at source to sass_binary
    * See if we can make the name one thing and output file named something else
* Instructions on how to add new components
* Tool to compare (SHA hash) of bagel output vs. webpack
* Run a dev server
* Run tests

## Nuggets of wisdom
* Use **module_name** within **ng_module** to expose **@something/foo** module names.

## Troubleshooting

## References
* [rules_nodejs](https://github.com/bazelbuild/rules_nodejs)
* [rules_typescript](https://github.com/bazelbuild/rules_typescript)
* [rules_sass](https://github.com/bazelbuild/rules_sass)
* [angular bazel defs](https://github.com/angular/angular/tree/master/packages/bazel)
* [angular-bazel-example](https://github.com/alexeagle/angular-bazel-example/wiki/Angular-rules)
* [bazel rule examples](https://github.com/bazelbuild/examples/tree/master/rules)
* [Angular rules](https://github.com/alexeagle/angular-bazel-example/wiki/Angular-rules#setup)
* [Angular Bazel Closure slides](https://docs.google.com/presentation/d/153iZaxNvGrizB4JJuNL7Rjb9cWAfezt8s73W5NBIAaw/preview#slide=id.g26d86d3325_0_0)
