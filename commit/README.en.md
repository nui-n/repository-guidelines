# Commit

## Frequency

- One commit per task step
- One commit per file

## Message

### Format

```
<Command>: <Subject, Description>
```

#### Command

```
<Type><Specifier[<Action><Modifier>]>
```

##### Type

- ` ` - Code
- `=` - Chore (minor/trivial tasks that don't affect code)
- `$` - Documentation
- `>` - Commands / Workflow

##### Specifier（補助記号）

###### Action

- `+` - Addition (including initial commit)
- `*` - Modification
- `^` - Quality improvement
- `-` - Removal

###### Modifier

- `?` - Experimental implementation
- `!` - Breaking change

#### Separator

- `: `

#### Subject

- Up to 50 characters
- Lowercase
- No period

#### Description

- No restrictions

### Usage

```jsonc
$+: add `README.md` // docs
+!: add arithmetic operations // feat
*: fix to prevent division by 0 // fix
+!: add linear functions // feat
*!: add a y-intercept to a linear function // fix
*: set default intercept // fix
+?: add memory feature // feat (experimental)
^: replace `if` with `switch` for arithmetic // refactor
^!: split into modules // refactor
=*: fix comment typo // style
>+: add `-minify` option // build
>+: add caching // ci
```
