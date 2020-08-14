Words Count
====================

[![Build Status](https://travis-ci.org/magiclen/words-count.svg?branch=master)](https://travis-ci.org/magiclen/words-count)

Count the words and characters, with or without whitespaces.

## Examples

```rust
extern crate words_count;

use words_count::WordsCount;

assert_eq!(WordsCount {
    words: 20,
    characters: 31,
    whitespaces: 2,
    cjk: 18,
}, words_count::count("Rust是由 Mozilla 主導開發的通用、編譯型程式語言。"));
```

```rust
extern crate words_count;

let result = words_count::count_separately("apple banana apple");

assert_eq!(2, result.len());
assert_eq!(Some(&2), result.get("apple"));
```

## Crates.io

https://crates.io/crates/words-count

## Documentation

https://docs.rs/words-count

## License

[MIT](LICENSE)