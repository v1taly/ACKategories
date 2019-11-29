# Changelog

- please enter new entries in format 

```
- <description> (#<PR_number>, kudos to @<author>)
```

## Next

- add `tapestry` for automating future releases (#56, kudos to @fortmarek)
- update [FlowCoordinator](ACKategories/Base/FlowCoordinator.swift) to count with iOS 13 modal presentations (#55, kudos to @olejnjak)
    
    ⚠️ **BREAKING CHANGE:** as `FlowCoordinator.start(from viewController:)` now expects that its `rootViewController` is already set, you might need to adjust some of your code

## 6.2
- add `forceIntrinsic()` to `UIView` to set its `contentHuggingPriority` and `contentCompressionResistance` to `UILayoutPriority.required` (#48, kudos to @olejnjak)
- add `hexString` closure into `UIColorExtension` that will return hex string from `UIColor` (#49, kudos to @majkcajk)
- add SwiftPM manifest (#52, kudos to @olejnjak)
- add `type` parameter to `dequeueCell(...)` methods so using it is more convenient (#53, kudos to @olejnjak)

  From now you can also use
  ```swift
  tableView.dequeueCell(for: indexPath, type: YourCell.self)
  ```

## 6.1
- added deep link generic for `Base.FlowCoordinator` (#47, kudos to @fortmarek)
- Swift 5 & Xcode 10.2 migration (#45, kudos to @janmisar)
- base classes for VCs, VMs, FCs (#45, kudos to @janmisar)

## 6.0.3
- fix init emoji in `FlowCoordinator` (#42, kudos to @Dominoo)

## 6.0.2
- move from NSLog to unified logging (#39, kudos to @fortmarek)
- allow additional logic for isEmpty for collections (#40, kudos to @fortmarek) 
- add LICENSE file to Cocoapods source files
