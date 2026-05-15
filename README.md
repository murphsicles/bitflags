# @std/bitflags — Bit Flag Types for Zeta

Auto-converted from [bitflags](https://crates.io/crates/bitflags) v2.11.1 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **bitflags! macro** — define type-safe bit flag structs
- **Full operations** — intersection, union, difference, symmetric difference, complement
- **Parser** — from_bits, from_name, from_bits_truncate, from_bits_retain
- **Iterator** — iterate over set flags
- **Formatting** — binary, octal, hex display, and custom formatting
- **Serde** — serialize/deserialize support

## Usage
```zeta
use @std/bitflags::bitflags;

bitflags! { struct Flags: u32 {
    const A = 1;
    const B = 2;
    const C = 4;
    const AB = Self::A.bits() | Self::B.bits();
}}
```

## Stats: 43 source files, ~1,451 lines, 0 unsupported items

## License
MIT