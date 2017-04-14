# Generating Classes

To add a class called `User`, run:

```bash
  $ ng g cl user

  installing class
    create src/app/user.ts
```

- To enable `.spec` files creation add `--spec` or `-sp` flag

```bash
  $ ng g cl user --spec

  installing class
    create src/app/user.spec.ts
    create src/app/user.ts
```

All `generate class` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Enable `.spec` files creation   | `--spec`                                |`-sp`          | `false`
