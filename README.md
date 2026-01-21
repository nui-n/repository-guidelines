<div align="center">

# Repository Guidelines

独自のリポジトリ運用ガイドライン

[Available in English](https://github.com/nui-n/repository-guidelines/blob/main/README.en.md)

</div>

---

- [Overview](#overview)
- [Guidelines](#guidelines)
  - [Branch](#branch)
  - [Commit](#commit)
- [License](#license)

---

## Overview

nuinが自身のリポジトリを運用していく上で、守るべき規則をまとめているリポジトリです。

## Guidelines

### Branch

| 名称       | 説明                                             |
|------------|-------------------------------------------------|
| `main`     | 開発が行われる主要なブランチ                       |
| `work/*`   | 新しい機能や要素、改善を作業するための一時的ブランチ |
| `hotfix/*` | 緊急の修正が必要な場合に使用される一時的ブランチ     |
| `stable`   | リリースが行われる集積（保管）用のブランチ          |

詳しくは[branch](https://github.com/nui-n/repository-guidelines/blob/main/branch/README.md)を参照

### Commit

基本は工程毎にコミットを行い、メッセージフォーマットは以下のようになっている。

```
<Command>: <Subject, Description>
```

| 名称          | 説明                                                                                        |
|---------------|--------------------------------------------------------------------------------------------|
| `Command`     | タイプ識別子とアクション・修飾子からなる補助記号の二つを組み合わせ、コミット内容を簡易的に表す接頭辞 |
| `Subject`     | コミット内容をわかりやすく表示するタイトル、要約                                                |
| `Description` | `Subject`だけでは伝えられないより詳細な内容を記述する場                                         |

詳しくは[commit](https://github.com/nui-n/repository-guidelines/blob/main/commit/README.md)を参照

## License

[MITライセンス](https://choosealicense.com/licenses/mit/)のもとで公開されています。
