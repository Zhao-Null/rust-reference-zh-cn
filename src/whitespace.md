# 空白

> [whitespace.md](https://github.com/rust-lang/reference/blob/master/src/whitespace.md)
> <br />
> commit 4a2bdf896cd2df370a91d14cb8ba04e326cd21db

空白是任何仅具有 `Pattern_White_Space` Unicode 属性的非空字符串，也就是：

- `U+0009` （水平制表符，`'\t'`）
- `U+000A` （换行符，`'\n'`）
- `U+000B` （垂直制表符）
- `U+000C` （分页符）
- `U+000D` （回车符，`'\r'`）
- `U+0020` （空格符，`' '`）
- `U+0085` （下移符）
- `U+200E` （自左向右符）
- `U+200F` （自右向左符）
- `U+2028` （行分隔符）
- `U+2029` （段落分隔符）

Rust 是一个“形式自由”的语言，这意味着任何形式的空白仅用来分隔语法中_记号_，并无语义意义。

Rust 程序中，如果每个空白元素被替换为任何合法的其它空格元素（如单个空格字符），则它们仍有相同的意义。
