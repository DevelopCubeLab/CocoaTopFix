# CocoaTopFix
iOS Utils CocoaTop fix enable Bold Text crash  
CocoaTop TrollStore version will crash when opening this app after enabling the "Bold Text". The issue is fixed after re-signing the permissions with ldid.  
CocoaTop TrollStore版本在开启系统自带“粗体文字”后打开这个app会闪退，使用ldid重新签名权限后修复。  

## Fix steps
1. Download the original version [CocoaTopTS](https://raw.githubusercontent.com/baziex/TrollStoreApps/main/TrollStoreApps/CocoaTopTS_BZ.ipa)
2. Rename it to `.zip` and get the app after decompression
3. Download [entitlements.plist](https://github.com/DevelopCubeLab/CocoaTopFix/blob/main/CocoaTop_entitlements.plist)
4. Use ldid to re-sign `ldid -SCocoaTop_entitlements.plist CocoaTop.app/CocoaTop`
5. Repackage the Payload directory into `zip` and rename it to `.ipa` or `.tipa`

## 修复步骤
1. 下载原版[CocoaTopTS](https://raw.githubusercontent.com/baziex/TrollStoreApps/main/TrollStoreApps/CocoaTopTS_BZ.ipa)
2. 重命名为`.zip`，解压后获取到app
3. 下载[entitlements.plist](https://github.com/DevelopCubeLab/CocoaTopFix/blob/main/CocoaTop_entitlements.plist)
4. 使用ldid重新签名`ldid -SCocoaTop_entitlements.plist CocoaTop.app/CocoaTop`
5. 重新打包Payload目录为`zip`并且重命名为`.ipa`或者`.tipa`

## Reference
[Reddit](https://www.reddit.com/r/jailbreak/comments/x6lok9/free_release_filza_file_manager_and_cocoatop_for/)  
[CocoaTop](https://github.com/D0m0/CocoaTop)  
ChatGPT 4o
