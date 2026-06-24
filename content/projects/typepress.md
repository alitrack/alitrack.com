+++
title = "TypePress"
description = "Pure Rust HTML→PDF engine — zero browser dependency"
repo = "https://github.com/alitrack/typepress"
lang = "Rust"
+++

纯 Rust 实现的 HTML→PDF 排版引擎。不依赖 Chrome、WebKit 或任何浏览器引擎。

- HTML parser (html5ever)
- Custom CSS cascade + box layout
- PDF backend (printpdf)
- CJK font support with fallback chains
- ~15K lines of Rust

客户的生产环境没有 GUI——所以不需要浏览器。
