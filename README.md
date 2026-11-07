# FoundationEssentials shim

This package re-exports `Foundation` as `FoundationEssentials` for Linux-hosted builds that target Apple platforms.

Swift's `#Predicate` macro can generate references to `FoundationEssentials`, while Apple's SDK provides those declarations through `Foundation`. Add this package to an iOS target when you build it from Linux.

Keep it out of OpenSwiftData's root package. On Linux, a target named `FoundationEssentials` can shadow the toolchain module and create a dependency cycle. Builds run on macOS should use Apple's `Foundation` directly.
