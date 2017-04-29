
The Show type class represents those types which can be converted into a
human-readable String representation.

While not required, it is recommended that for any expression `x`, the
string `x.show()` be executable JavaScript code which evaluates to the same
value as the expression `x`.

```haskell
class Show a where
    show :: a -> String
```

### implements

```haskell
implements :: Type a -> { show :: a -> String } -> Show a
```

Adds `show` method onto the passed concrete class.

