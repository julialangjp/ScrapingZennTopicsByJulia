# ScrapingZennTopicsByJulia
Julia言語を使って、ZennのJuliaトピックページをスクレイピングする

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
'''
> julia get_zenn.jl
'''

### 結果出力
日付付きのファイルに出力されます
例） Zenn20220301.txt

## 備考
　ZennのJuliaトピックページのURLを埋め込んであります。ここを書き換えることでほかのトピックページのスクレイピングも可能です。
　ただし、トピックページのみを対象としています。ほかの構成のページついては、タグやクラス指定などを変更してください。

## 参照
　次のページに簡単な解説を書きました
  スクレイピング：ZennのJuliaトピックページからリンクを取得(julialang.jp)
