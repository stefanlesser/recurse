# plThesaurus

*While I'm learning Haskell, I'm trying to reference symbols in Haskell to symbols in other languages I know.*

### Operators

| Operator   | Purpose             | C   |Swift|Haskell|
|------------|---------------------|-----|-----|-----|
| + plus     | addition            | [x] | [x] | [x] |
| - minus    | subtraction         | [x] | [x] | [x] |
| * asterisk | multiplication      | [x] | [x] | [x] |
| / slash    | fractional division | [x] | [x] | [x] |
| div        | divide              |     |     | [x] |
| mod        | modulo              |     |     | [x] |
| quod       | quotient            |     |     | [x] |
| %, rem     | remainder           |     | %   | rem |
| +          | unary plus          |     | [x] | [x] |
| -          | unary minus         | [x] | [x] | [x] |

### Function definitions

### Other stuff

| Purpose | C | Swift | Haskell |
|---------|---|-------|---------|
| Refer to operators as value (1st class function) | *function pointers?* | Just use operator. | Use infix function with parentheses (). |
| Use infix operator as prefix | | | Use infix function with parentheses (). |
| Sectioning: pass around partially applied functions | | *currying with (A) -> (B) -> C* | `(1/) 2 -- 0.5`, `(/1) 2 -- 2.0` |
