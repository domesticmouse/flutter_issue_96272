# `flutter/flutter` Issue #96272 repro case

This project is a minimised reproduction for [flutter/flutter Issue #96272](https://github.com/flutter/flutter/issues/96272)

Building on macOS:

```console
$ dart run build_runner build --delete-conflicting-outputs 
Building package executable... (1.6s)
Built build_runner:build_runner.
[INFO] Generating build script completed, took 455ms
[INFO] Reading cached asset graph completed, took 63ms
[INFO] Checking for updates since last build completed, took 554ms
[WARNING] gql_build:serializer_builder on lib/$lib$:
Your current `analyzer` version may not fully support your current SDK version.

Analyzer language version: 2.14.0
SDK language version: 2.15.0

Please update to the latest `analyzer` version (3.0.0) by running
`flutter packages upgrade`.

If you are not getting the latest version by running the above command, you
can try adding a constraint like the following to your pubspec to start
diagnosing why you can't get the latest version:

dev_dependencies:
  analyzer: ^3.0.0 

[INFO] Running build completed, took 11.2s
[INFO] Caching finalized dependency graph completed, took 44ms
[INFO] Succeeded after 11.3s with 12 outputs (12 actions)
```