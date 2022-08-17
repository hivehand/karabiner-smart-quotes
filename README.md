The Mac's built-in keyboard support for typographically-correct
characters is one of the little things I treasure about the platform,
and something I miss dearly when I'm using Linux. En and Em dashes,
along with ellipses, are easy to generate in conjunction with the
Option and Shift keys.

Smart quotes, unfortunately, are a slightly different story. You can
also generate them using Shift and Option in conjunction with the
`[{` and `]}` keys, but the mapping seems arbitrary and thus, for me
at least, impossible to remember.

Fortunately, it's easy to fix. You don't even have to involve any
other keys. You just have shift the existing mappings around a bit to
make things much cleaner:

|  Combination      |  Result  | Description            |
|  ---------------  |  :----:  | ---------------------- |
|  Option-\[        |  ‘       |  Opening single quote  |
|  Option-Shift-\[  |  “       |  Opening double quote  |
|  Option-\]        |  ’       |  Closing single quote  |
|  Option-Shift-\]  |  ”       |  Closing double quote  |

Now the keys become consistent with both themselves and their
immediate neighbor, the plain-quotes key just beneath them. The
opening bracket is _always_ an opener, and the closing bracket is
_always_ a closer. The absence of Shift _always_ produces a single
quote; its presence _always_ yields a double quote.

I find this arrangement infinitely easier to remember. YMMV, of course.

To deploy, just

```
cp smarter_quotes.json ~/.config/karabiner/assets/complex_modifications
```

and then activate through Karabiner's Complex Modifications UI.
