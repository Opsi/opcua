# Changelog

## v0.3.3 (8 Apr 2022)

* Don't panic on close (#562)
* Set minimum Go version to go1.17 (#573)
* Refactor the use of the `subMux` lock (#572)

## v0.3.2 (14 Mar 2022)

* Add support for arrays (#564)

## v0.3.1 (27 Jan 2022)

* Refresh cached namespaces on reconnect (#552)

* Add more `WithContext(ctx)` methods and use context in more places (#555)

## v0.3.0 (21 Jan 2022)

* Add `WithContext(ctx)` variants to all methods of `Client` and `Node` and migrate existing methods
  to use `context.Background()`. The existing methods without a context are deprecated and starting
  with v0.5.0 we will drop the `WithContext(ctx)` prefix and all `Client` and `Node` methods will
  require a `context`. (#541, #542, #548, #549)

## v0.2.7 (18 Jan 2022)

* Add a `FindNamespace` method to `Client`. (#546)

## v0.2.6 (4 Jan 2022)

* Fix invalid session id regression introduced with v0.2.4 (#539)
