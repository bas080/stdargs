# stdargs

Enhance your script by easily allowing args or stdin.

## Usage

An example with stdin in the middle:

```bash bash
stdargs hello - world <<< 'big'
```
```
hello
big
world
```

Without stdin:

```bash bash
stdargs hello world
stdargs 'hello world'
```
```
hello
world
hello world
```

With only stdin:

> In this case the `-` arg is optional.

```bash bash
stdargs - <<< hello
stdargs <<< world
```
```
hello
world
```

## License

GPLv3
