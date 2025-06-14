### Devin

- [Devin's Machine](https://app.devin.ai/workspace) でリポジトリ追加

#### Git Pull
- そのまま

#### Configure Secrets
```sh
# 環境変数用のファイル作成
$ touch .envrc

# 環境変数を読み込む
$ direnv allow
```

- ローカル用
```sh
$ brew install direnv
```
#### Maintain Dependencies
```sh
$ uv venv && uv pip sync requirements.txt
```

#### 5.SetUp Lint
```sh
$ uvx ruff check
```

#### 6.SetUp Tests
```sh
$ uvx pytest
```
