_This project has been created as part of the 42 curriculum by bucolak._

# ft_printf

A re-implementation of the C standard library `printf` using **variadic functions** (`stdarg.h`).

## Supported Conversions

| Specifier | Output |
|---|---|
| `%c` | single character |
| `%s` | string (`(null)` for NULL) |
| `%p` | pointer address in hexadecimal |
| `%d` `%i` | signed decimal integer |
| `%u` | unsigned decimal integer |
| `%x` `%X` | hexadecimal (lower / upper case) |
| `%%` | percent sign |

Returns the number of characters printed, like the original.

## Usage

```bash
make        # builds libftprintf.a
cc main.c libftprintf.a
```

```c
ft_printf("%s has %d items, ptr: %p, hex: %X\n", "list", 42, &x, 255);
```

## Concepts Practised

Variadic functions (`va_list`, `va_arg`) · number base conversion · writing a static library

## Author

**Buket Çolak** (bucolak) — [github.com/bucolak](https://github.com/bucolak)
