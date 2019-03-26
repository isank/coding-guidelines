# Coding Guidelines

## Git

- Make small `commits`. For example, when you create a new `Model/Entity`, it's fine to `commit` it. Remember `commit` and `push` are two different things in Git. Also, if you think your `commit` list is too big, you can `squash` them.

- Always take a `pull` before you `commit`.

- Do not create new branches on Bitbucket to start with. Create them on `local` and `push` it only when needed.

- Make sure your code is in sync with Master from time to time to avoid unnecessary conflicts.

## Spring

- Use `constructor` based `injection` over `field` based `injection`.

- Use `configuration properties` instead of `@value`.

- Try to minimise the dependencies of your service.

## Principles

- `DRY` - Don't repeat yourself
- `SRP` - Single Responsibility Principle
- `YAGNI` - You ain't gonna need it
- Code to `interface`
- Low Coupling and High Cohesion

## General Coding

- A `public` method shouldn't do too much of work and should be small. Try to keep it at 15 lines max.

- Do not use `public` instance fields in Models/Entities unless you have a very good reason to do so.

- `public static` without `final` is evil. This applies to constants and fields.

- A `private` method should do only one work and, it must be a pure function.

- Do not make a `private` method `protected` just to test it. Your `private` methods should be so concise that they can be tested through the `public` methods using them.

- `Early exists` makes the code easy to understand and follow. Also, it removes unnecessary nestings and spaghetti code.

- `Immutability` is very powerful. Try to use it whereever possible.

- `Flux` & `Mono` has plethora of operations that are very useful and are suitable for many existing cases.

- Make use of `Java 8's` features to it's fullest.

- If your method's accepting more than 2/3 parameters then there's definitely a problem and that method can be broken.

- Consider moving commonly used methods to a `Utility Class`.

## Testing

- Unit test for a `class` is meant to test the functionality of that particular `class` only. No more, no less.

- Do not use `mock` too much. It takes away the whole purpose of unit tests.
