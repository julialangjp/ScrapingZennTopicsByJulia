# ScrapingZennTopicsByJulia
Julia言語を使って、ZennのJuliaトピックページをスクレイピングして、見出しとURLを取り出します。  
ページネーションは考慮していないので、最初のページの情報のみを抜き出します。

## Installation
```julia
using Pkg
Pkg.add("HTTP")
Pkg.add("Gumbo")
Pkg.add("Cascadia")
Pkg.add("URIs")
```

## Usage
### コンソールで実行
```julia
> julia getZenn.jl
```

### 結果出力
日付付きのファイルに出力されます。  
例） zenn20220301.txt

TSV形式：行に一組の見出しとURLがTAB区切りで格納されます。

## 備考
　ZennのJuliaトピックページのURLを埋め込んであります。ここを書き換えることでほかのトピックページのスクレイピングも可能です。  
　ただし、トピックページのみを対象としています。ほかの構成のページついては、タグやクラス指定などを変更してください。

## 参照
　次のページに簡単な解説を書きました。  
　　  [スクレイピング：ZennのJuliaトピックページからリンクを取得](https://leadinge.co.jp/julialang/2022/03/26/scraping_zenn/)
