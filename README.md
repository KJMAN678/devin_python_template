### Devin

- [Devin's Machine](https://app.devin.ai/workspace) でリポジトリ追加

#### 1.Git Pull
- そのまま

#### 2.Configure Secrets
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
#### 4.Maintain Dependencies
```sh
$ uv venv && . .venv/bin/activate && uv pip install -U pip && uv pip sync requirements.txt
```

#### 5.SetUp Lint
```sh
$ uvx ruff check
```

#### 6.SetUp Tests
- no tests ran in 0.00s だと Devin の Verify が通らないっぽい
```sh
$ uvx pytest
```

#### 8.Additional Notes
- 必ず日本語で回答してください を入力
