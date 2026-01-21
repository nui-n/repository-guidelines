# Commit

## Frequency

- 工程毎に1コミット
- ファイル毎に1コミット

## Message

### Format

```
<Command>: <Subject, Description>
```

#### Command

```
<Type><Specifier[<Action><Modifier>]>
```

##### Type

- ` ` - コード
- `=` - 些事・雑事（基本的に変更がコードに影響のないもの）
- `$` - ドキュメント
- `>` - コマンド・ワークフロー関連

##### Specifier（補助記号）

###### Action

- `+` - 追加（初回コミットを含む）
- `*` - 修正
- `^` - 品質向上
- `-` - 削除

###### Modifier

- `?` - 実験的実装
- `!` - 破壊的変更

#### Separator

`: `

- コロンの後にはスペースが必要

#### Subject

- 50文字以内
- 小文字
- ピリオド無し

#### Description

- 特に制限なし

### Example

```ini
$+: `README.md`の追加 # docs
+!: 四則演算の追加 # feat
*: 0で割れないように修正 # fix
+!: 一次関数の追加 # feat
*!: 一次関数に切片の追加 # fix
*: 切片にデフォルト値を追加 # fix
+?: メモリ機能の追加 # feat (experimental)
^: 四則演算の分岐を`if`文から`switch`文に変更 # refactor
^!: ファイルの分割 # refactor
=*: コメントのタイポ修正 # style
>+: `-minify`オプションの追加 # build
>+: キャッシュの追加 # ci
```
