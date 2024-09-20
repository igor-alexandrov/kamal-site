---
title: Aliases
---

# Aliases


Aliases are shortcuts for Kamal commands.

For example, for a Rails app, you might open a console with:

```shell
kamal app exec -i -r console "rails console"
```

By defining an alias, like this:
```yaml
aliases:
  console: app exec -r console -i "rails console"
```
You can now open the console with:
```shell
kamal console
```

## [Configuring aliases](#configuring-aliases)

Aliases are defined in the root config under the alias key

Each alias is named and can only contain lowercase letters, numbers, dashes and underscores.

```yaml
aliases:
  uname: app exec -p -q -r web "uname -a"
```