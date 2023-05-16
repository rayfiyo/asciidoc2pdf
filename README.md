**I found an existing service and archived it.**

# Usage asciidoctor-pdf on Japanese (日本語でのasciidoctor-pdfの使用方法)
~~~
docker run --rm -v $(pwd):/documents/ asciidoctor/docker-asciidoctor asciidoctor-pdf -a scripts=cjk -a pdf-theme=default-with-fallback-font {targetFile.adoc}
~~~
* Change {targetFile.adoc} to any path. ( {targetFile.adoc} は任意のパスに変更してください。)

# info
[asciidoctor / asciidoctor-pdf](https://github.com/asciidoctor/asciidoctor-pdf)
[Asciidoctor PDF Documentation](https://docs.asciidoctor.org/pdf-converter/latest/)

---

# asciidoc2pdf
Forked from "kenmasumitsu / asciidoc-sample". Docker operation to convert AsciiDoc to PDF.  
"kenmasumitsu / asciidoc-sample"からフォークしたもの。AsciiDocをPDFに変換する操作をDockerで行う。  

# special thx
[AsciiDocで文章作成して、PDF化](https://qiita.com/kenma/items/0866cd0f658ec1c506ec)

---
# The following is from the forked source READMD.md

# AsciiDocサンプル

次の特徴を持つAsciiDoc ドキュメントと、PDF変換スクリプト

* 表紙
* 目次
* セクション番号
* `mermaid`記載したUMLを図として埋め込む
* `PNG`画像を埋め込む
* 図番号
* クロスリファレンス
