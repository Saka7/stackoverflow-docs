# Generating Services

To add a service with a dependency injection name `UserService`, run:

```bash
  $ ng g s user

  installing service
    create src/app/user.service.spec.ts
    create src/app/user.service.ts
```

- To prevent `.spec` files creation, use `--spec false` or `-sp false` flag

```bash
  $ ng g s user --spec false
  
  installing service
    create src/app/user.service.ts
```

- To prevent folder creation add `--flat` or `-f` flag

```bash
  $ ng g s user --flat

  installing service
    create src/app/user.service.spec.ts
    create src/app/user.service.ts
```

You can also combine flags listed above. For example, to create only `.service.ts` file without `.spec` file and folder use following command.

```bash
  $ ng g s user -f -sp false

  installing service
    create src/app/user.service.ts
```

All `generate service` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Prevent folder creation         | `--flat`                                | `-f`          | `false`
Prevent `.spec` files creation  | `--spec false`                          | `-sp false`   | `true`


