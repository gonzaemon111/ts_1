#1 導入編

## 1-2 tscコマンドで始めよう！

```shell
$ tsc --init # tscコマンドでtsconfig.jsonを作成できる
```

`tsc --init`で作成されるtsconfig.jsonの内容は以下である。

```json
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "strict": true,
    "esModuleInterop": true
  }
}
```

`strict: true`にすると、これが型チェックを有効にしている！

型チェックの厳密さを弱くする。-> `noImplicitAny: false`にすると、`any関係`ではエラーがなくなる！

`strictNullChecks: false`に設定するのは、typescriptのNullチェックという醍醐味を失うので、これは設定してはいけない！
-> 基本的に`strict: true`に設定する!


## 出力先をしてする！

TypeScriptでは`tsconfig.json`配下にあるプロジェクト全てをビルドする！
出力するディレクトリも、プロジェクトのrootディレクトリである！