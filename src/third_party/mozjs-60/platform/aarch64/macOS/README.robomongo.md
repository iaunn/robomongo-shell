# aarch64 / macOS SpiderMonkey platform files

Added for the Apple Silicon port. These files are **not** generated at build time: they are copies of
the checked-in x86_64/macOS profile (`../../x86_64/macOS`), the same way MongoDB ships one
pre-generated `Unified_cpp_js_src*.cpp` / `js-confdefs.h` / `js-config.h` set per platform.

When `src/third_party/mozjs-60/extract` is updated, regenerate the x86_64 profile with
`src/third_party/mozjs-60/gen-config.sh` and mirror the result here (only the architecture-specific
defines in `js-confdefs.h` / `js-config.h` differ).
