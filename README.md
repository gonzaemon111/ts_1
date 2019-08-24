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