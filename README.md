# kawamataryoの職務経歴書

[Web](https://kawamataryo.github.io/resume/)  
[PDF](https://github.com/kawamataryo/resume/releases)  
[Markdown](https://github.com/kawamataryo/resume/blob/master/docs/README.md)  

# Usage


## Edit resume

[docs/README.md](https://github.com/kawamataryo/resume/blob/master/docs/README.md) を編集してください。

## Lint text

[textlint](https://github.com/textlint/textlint) での校正が可能です。

```
$ yarn lint
```

[husky](https://github.com/typicode/husky) によってcommit前にも自動で実行されます。  
校正のルールは`.textlintrc`をご覧ください。


## Build PDF

[md-to-pdf](https://www.npmjs.com/package/md-to-pdf) でのPDF生成が可能です。

```
$ yarn build:pdf
```


出力されるPDFはCSSで任意のスタイルを設定可能です。詳細は`pdf-configs`をご覧ください。  

## Release

`v**` tagをつけてpushするとGitHub Actionsでビルドが走り、PDFの生成、Releaseの作成、AssetsへPDFの登録が実行されます。

```
$ git commit -m "add job"
$ git tag v1.0
$ git push origin --tags
```



