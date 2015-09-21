# accidental-value



## usage

```js
var accval = require('accidental-value');
```

### accval(accidental)

Returns the *value* of the accidental from the table below.
This is useful for manipulating notes and intervals.

 - 'x' = 2
 - '#' = 1
 - '' = 0
 - 'b' = -1
 - 'bb' = -2

### accval.interval(accidental)

Returns the relative interval (given in `[steps, semitones]` format)
of the accidental. E.g.:
```js
accval.interval('#') // [0, 1]
accval.interval('bb') // [0, -2]
```
