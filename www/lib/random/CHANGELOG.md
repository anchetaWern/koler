# 1.0.5 (2015-03-03)

- `sample()` results are no longer biased toward the final element.
- `discard(count)` on the `mt19937` engine properly works when count is less than 625
- Clarify that the built-in engines return signed 32-bit integers (not unsigned).

# 1.0.4 (2014-05-11)

- `string('')` now throws an error
- `hex(upper)` now returns a cached function, for efficiency.
- add `int32()`, which returns an integer from `-0x80000000` to `0x7fffffff`.
- performance enhancements
- add benchmark suite, covers engines, integer, bool, and real.
- add `date(start, end)`, which returns a Date within a uniform distribution.

# 1.0.3 (2014-04-23)

- `Random` no longer needs to be called with new, allowing `var r = require('random-js')()`
- Add `begin` and `end` arguments to `pick` and `picker`.

# 1.0.2 (2014-03-20)

- Even if `shuffle` receives an empty array, it should return that same array.

# 1.0.1 (2014-03-20)

- Fix `sample` and `shuffle` when they are passed an empty array.
- Include `-c` (compress) option when uglifying.

# 1.0.0 (2014-02-16)

Initial release