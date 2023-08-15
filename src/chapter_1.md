# Task master application

## Install 

* Install dependency cbindgen: cargo install cbindgen (may need latest version, thanks @gmorenz)
* Install dependency ffigen: dart pub global activate ffigen, and install LLVM.
* Install this code generator binary by cargo install flutter_rust_bridge_codegen.
* Add flutter_rust_bridge = "1.0" (where 1.0 should be the latest version) to Rust's Cargo.toml.
* Add flutter_rust_bridge: ^1.0 (same as above, should be latest version) to Flutter/Dart's pubspec.yaml under the section of dependencies.
## Run 
```
flutter_rust_bridge_codegen --rust-input path/to/your/api.rs --dart-output path/to/file/being/bridge_generated.dart
```
