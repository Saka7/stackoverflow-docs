# Generating builiding blocks

You can use the `ng generate` command to generate Angular building blocks (components, services, pipes, etc.).

`ng generate component component-name` (`ng g c component-name`) command creates Angular component in the directory where you have run it.

So, for example, if you are in `src/app/` folder and you have run `ng g c user-list` - Angular Cli will: 
 - create `user-list` directory
 - inside that directory generate 4 files (`user-list.component.ts`, `user-list.component.html`, `user-list.component.css` and `user-list.component.spec.ts`)
 - add `user-list` as a declaration in the `@NgModule` decorator of the nearest module.

You can find all possible **blueprints** in the table below:

Scaffold  | Usage                                   | Shortened
---       | ---                                     | ---   
Component | `ng generate component component-name`  | `ng g c component-name`
Directive | `ng generate directive directive-name`  | `ng g d directive-name`
Pipe      | `ng generate pipe pipe-name`            | `ng g p pipe-name`
Service   | `ng generate service service-name`      | `ng g s service-name`
Class     | `ng generate class class-name`          | `ng g cl class-name`
Guard     | `ng generate guard guard-name`          | `ng g g guard-name`
Interface | `ng generate interface interface-name`  | `ng g i interface-name`
Enum      | `ng generate enum enum-name`            | `ng g e enum-name`
Module    | `ng generate module module-name`        | `ng g m module-name`

