# fp.pow

```rust
fn pow(self: FixedType, b: FixedType) -> FixedType;
```

Returns the result of raising the fixed point number to the power of another fixed point number.

## Args

* `self`(`FixedType`) - The input fixed point.
* `b`(`FixedType`) - The exponent fixed point number.

## Returns

A fixed point number representing the result of x^y.

## Examples

```rust
fn pow_fp_example() -> FixedType {
    // We instantiate FixedTrait points here.
    let a = FixedTrait::from_unscaled_felt(3); 
    let b = FixedTrait::from_unscaled_felt(4);
    
    // We can call `pow` function as follows.
    a.pow(b)
}
>>> {mag: 5435817984, sign: false} // = 81
```
