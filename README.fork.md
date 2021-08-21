# About This Fork

## Modifications

### Build System Changes

#### Use `git submodule` instead of `depo_tools` to check out dependencies.

- The specific submodule information can be found in the `DEPS` file.

#### Use `cmake` instead of `depo_tools` to build the project.

- Add several `CMakeLists.txt` files.

  Based on changes made in [getsentry/crashpad], distributed with [Apache 2.0 License].

- Add `third_party/mini_chromium/build/chromeos_buildflags.h`.

  Copy from `out/Default/gen/build/chromeos_buildflags.h` after running `ninja`.

- Update `util/mach/mig_gen.py` to fix cross build for iOS.

  Based on changes made in [getsentry/crashpad], distributed with [Apache 2.0 License].

[getsentry/crashpad]: https://github.com/getsentry/crashpad
[Apache 2.0 License]: LICENSE
