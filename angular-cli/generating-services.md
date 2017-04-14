# Generating Services

To add a service with a dependency injection name `UserService`, run:

```bash
  $ ng g s user

  installing service
    create src/app/user.service.spec.ts
    create src/app/user.service.ts
```

- To prevent `.spec` files creation add `--spec false` or `-sp false` flag

```bash
  $ ng g s user --spec false
  
  installing service
    create src/app/user.service.ts
```

- To enable folder creation add `--flat false` or `-f false` flag

```bash
  $ ng g s user --flat false

  installing service
    create src/app/user/user.service.spec.ts
    create src/app/user/user.service.ts
```

You can also combine flags listed above. For example, to create only `user.service.ts` file inside `user` folder without `.spec` file use the following command.

```bash
  $ ng g s user -f false -sp false

  installing service
    create src/app/user/user.service.ts
```

All `generate service` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Prevent folder creation         | `--flat false`                          | `-f false`    | `true`
Prevent `.spec` files creation  | `--spec false`                          | `-sp false`   | `true`


