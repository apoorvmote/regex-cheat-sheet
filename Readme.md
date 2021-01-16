# Regular expression cheat sheet

## Most frequently used

| Flag   |      Description      | 
|:----------:|-------------:|
| `g` |  Find every instance of pattern | 
| `i` |    Case insensitive   | 
| `m` |    Multiline   | 

| Character   |      Description      | 
|:----------:|-------------:|
| `|` |    Or condition   |     
| `.` |    Any single character except newline   |     
| `+` |  Any single character/group to the left repeats one or more time | 
| `*` | Any single character/group to the left repeats zero or more time |
| `{exact}` |    Exact length of character/group to the left   |     
| `{min,}` |    Min length of character/group to the left   |     
| `{min,max}` |    Min length and maximum length of character/group to the left   |     
| `?` |    Any single character/group to the left is optional   |     
| `\` |    Use next character literally i.e. `{ } [ ] / \ + * . $ ^ | ?`  |     
| `^` |    Starting with next   |     
| `$` |    ending with before   |     

| Character Set  |      Description      | 
|:----------:|-------------:|
| `[]` |    Any single character from inside brackets   |     
| `[x-y]` |    Ranges start value `-` end value e.g.`[a-zA-Z0-9]`, `[0-3]`    |     
| `()` |    Character group. e.g. `(abc)` abc in that exact order   |     
| `[^]` |    Inverse of character set inside brackets   |     
| `\w` |    Any alphanumeric character and underscore `[a-zA-Z0-9_]`   |     
| `\W` |    Inverse of `\w` i.e. `[^\w]`   |     
| `\d` |    Any number character i.e. `[0-9]`   |     
| `\D` |    Inverse of `\d` i.e. `[^\d]`   |     
| `\s` |    Any whitespace `[\t\n\f\r]`   |     
| `\S` |    Inverse whitespace `[^\s]`   | 

| Lazy or Greedy  |      Description      | 
|:----------:|-------------:|
| `.*` `.+` |    Greedy   |     
| `.*?` `.+?` |    Lazy   |     

| Look around  |      Description      | 
|:----------:|-------------:|
| `(?=)` |    Positive lookahead   |     
| `(?!)` |    Negative lookahead   |     
| `(?<=)` |    Positive lookbehind   |     
| `(?<!)` |    Negative lookbehind   |     