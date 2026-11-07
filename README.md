# FoundationEssentials shim

This package re-exports `Foundation` as `FoundationEssentials` for Linux-hosted builds that target Apple platforms.

Swift's `#Predicate` macro can generate references to `FoundationEssentials`, while Apple's SDK provides those declarations through `Foundation`. Add this package to an iOS target when you build it from Linux.
