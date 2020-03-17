# rust-cheat-sheet
Rust cheat sheet

Très bonne ressource : [cheats.rs](https://cheats.rs/)

## Les Variables

Variable immutable (ne peut as être réaffectée)
```rust
let ma_var: i32 = 23;
```
Variable mutable
```rust
let mut ma_var: i32 = 23;
ma_var = 45;
```

### Types numériques

#### Entiers
|Type | Taille | Interval |
|-----|--------|----------|
| `i8` | 1 octet | De -128 à 127 |
| `u8` | 1 octet | De 0 à 255 |
| `i16` | 2 octets | De -32 768 à 32 767 |
| `u16` | 2 octets | De 0 à 65 535 |
| `i32` | 4 octets | De -2 147 483 648 à 2 147 483 647 |
| `u32` | 4 octets | De 0 à 4 294 967 295 |
| `i64` | 8 octets | De -9 223 372 036 854 775 808 à 9 223 372 036 854 775 807 |
| `u64` | 8 octets | De 0 à 18 446 744 073 709 551 615 |
| `i128` | 16 octets | De -170 141 183 460 469 231 731 687 303 715 884 105 728 à 170 141 183 460 469 231 731 687 303 715 884 105 727 |
| `u128` | 16 octets | De 0 à 340 282 366 920 938 463 463 374 607 431 768 211 455 |
| `isize` | 4 ou 8 octets | Selon l'OS (32 bits => `i32` ou 64 bits => `i64`) |
| `usize` | 4 ou 8 octets | Selon l'OS (32 bits => `u32` ou 64 bits => `u64`) |

#### Flottants
|Type | Taille | Size | Exposant | Mantisse |
|-----|--------|------|----------|----------|
| `f32` | 4 octets | 1 bit | 8 bits | 23 bits |
| `f64` | 8 octets | 1 bit | 11 bits | 52 bits |

#### Texte
|Type | Taille |
|-----|--------|
| `char` | 4 octets (UTF-8) |
| `str` ou plus souvent `&str` | Tableau de char |

