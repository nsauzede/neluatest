# neluatest
Testing the Nelua Programming Language..

## Hello, QuiNelua
A minimalist [Quine](https://en.wikipedia.org/wiki/Quine_(computing)) in Nelua
```lua
require'C.stdio'local s="require'C.stdio'local s=%c%s%c C.printf(s,34,s.data,34,10)%c" C.printf(s,34,s.data,34,10)
```
I know, this is probably not the best usage of the language but we always must start somewhere ;-)

Try it :
```shell
neluatest$ nelua -q qui.nelua > quine
neluatest$ md5sum qui.nelua quine
b0a9b053cc7898502a772263d8073be8  qui.nelua
b0a9b053cc7898502a772263d8073be8  quine
```
