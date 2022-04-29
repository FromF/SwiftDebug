# SwiftDebug

このパッケージはデバッグエリアに出力するときにどこからログ出力しているかわかりやすくします。

## 使い方
通常のログは`debugLog`を使います。

```swift
debugLog("デバッグログを出力します")
```

異常ルート時は、`errorLog`を使います。

```swift
errorLog("エラーが発生しました")
```

その他実行環境を判定も出来ます。

```swift
if isSimulator {
    debugLog("シミュレーター実行中")
} else if isPad {
    debugLog("iPad実行中")
} else if isPhone {
    debugLog("iPhone実行中")
}
```
