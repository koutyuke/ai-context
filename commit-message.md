## **コミットメッセージコンテキスト**

- 日本語は使用せずに全て英語で作成する

### **Dynamic Template**

`{type}({scope}){breaking_change_exclamation}: {description}`

### **type**

- 変更の種類
- `{emoji} {label}`
- 以下の中から使用すること

| emoji | label       | description                                   |
| ----- | ----------- | --------------------------------------------- |
| ✨    | `feat`      | 新機能の実装                                  |
| 🎈    | `feat`      | 機能の改善・更新                              |
| 🪦    | `feat`      | 機能の削除                                    |
| 🐛    | `fix`       | バグ修正                                      |
| 🔥    | `hotfix`    | 重大バグ修正・緊急対応                        |
| 📝    | `doc`       | ドキュメント変更                              |
| 💄    | `style`     | スタイル調整（フォーマット、空白、typo など） |
| ♻️    | `refactor`  | リファクタリング                              |
| 🏎️    | `perf`      | パフォーマンス向上                            |
| 🧪    | `test`      | テストコードの追加・修正                      |
| 📦️   | `build`     | ビルドや依存変更                              |
| 🦺    | `ci`        | CI 設定変更                                   |
| 🚀    | `cd`        | CD 設定変更                                   |
| 🔧    | `chore`     | その他の変更                                  |
| ⚙️    | `chore`     | 設定ファイルの変更                            |
| 🛠️    | `chore`     | スクリプトの変更                              |
| 📦    | `chore`     | 依存関係の更新                                |
| 🗑     | `chore`     | 不要ファイルやコードの削除                    |
| ⏪️   | `revert`    | 変更の取り消し                                |
| 🐳    | `container` | Dockerfile の変更                             |
| 🐙    | `compose`   | docker-compose の変更                         |
| 🚧    | `wip`       | WIP（作業中）                                 |
| 🎉    | `initial`   | 最初のコミット                                |

### **breaking_change_exclamation**

- `!`: 破壊的変更であることを示す記号
- 破壊的な変更でない場合は記述しない

### **scope**

- 変更対象の範囲
- 基本的には 3 階層まで(それより小さくなる分には問題ない)
- `{application}/{layer}/{detail}`
  - `application`: アプリケーションの分類. (例: api, mobile, web)
  - `layer`: アーキテクチャのレイヤーの分類. 基本的にディレクトにあるものを使用する. (例: domain, models, features)
  - `detail`: エンティティなどの分類. 基本的にディレクトリにある. (例: user, order, menu)

### **description**

- コミットの簡潔な説明
- 64 字以内
- 英語で記述する
- 日本語は使用しない
- Markdown 表記で記述してもよい

### **example**

- `🎈 feat(api/common/constant): add client type constant header and update session expires`
- `♻️ refactor(api/repository/session):  remove unused SessionConstructor type from session repository interface`
- `✨ feat(api/repositories/password-reset-session)!: add PasswordResetSession repository and interface for password reset functionality`
