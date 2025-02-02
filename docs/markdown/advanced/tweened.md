# `Tweened`

Tweened states update their values over a period of time.
For example, the following code snippet interpolates a value from 0 to 100 over a period of 200ms:

```rust
use std::time::Duration;

use maple_core::reactive::Tweened;
use maple_core::{easing, prelude::*};

let tweened = Tweened::new(0, Duration::from_millis(200), easing::linear);

tweened.set(100);
```

Different easing functions are provided in the `maple_core::easing` module.
