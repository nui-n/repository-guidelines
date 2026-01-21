<div align="center">

# Repository Guidelines

Custom repository operation guidelines

[日本語版はこちら](https://github.com/nui-n/repository-guidelines/blob/main/README.md)

</div>

---

- [Overview](#overview)
- [Guidelines](#guidelines)
  - [Branch](#branch)
  - [Commit](#commit)
- [License](#license)

---

## Overview

This repository documents the rules nuin should follow when operating the repository.

## Guidelines

### Branch

| Name       | Description                                                    |
|------------|----------------------------------------------------------------|
| `main`     | Primary branch where canonical project content is maintained   |
| `work/*`   | Temporary branches for changes (features, edits, improvements) |
| `hotfix/*` | Temporary branches for urgent fixes                            |
| `stable`   | Branch for accumulating/storing release-ready snapshots        |

See the [branch](https://github.com/nui-n/repository-guidelines/blob/main/branch/README.en.md) for details

### Commit

The basic rule is to commit per task step, and the commit message format is as follows:

```
<Command>: <Subject, Description>
```

| Name          | Description                                                                                             |
|---------------|---------------------------------------------------------------------------------------------------------|
| `Command`     | A prefix that succinctly represents the commit by combining a type identifier with a helper symbol; an action and a modifier. |
| `Subject`     | A title or summary that clearly presents the commit's content.                                          |
| `Description` | A place to write more detailed information that cannot be conveyed by the `Subject` alone.             |

See the [commit](https://github.com/nui-n/repository-guidelines/blob/main/commit/README.en.md) for details

## License

Made available under the [MIT license](https://choosealicense.com/licenses/mit/).
