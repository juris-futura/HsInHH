# Molecules and scripts


## Juvo molecule highlights

* intended as replacement to expressions
* molecule langague is based on our type based DI concept e.g.
   - call atom, add result to DI context available in next atom call step
   - DI "lenses" inside all types availabe in the DI context and steps can request very specific inputs
* syntax in yaml and consist of built-in steps

* lots of steps are based on internal optics (Juvo type traversed using other Juvo type).
* support for type variables


## Pros

* imperative
* more declarative alternative to writing python
* simpler to use than expressions
* ideal for testing atoms

## Cons

* newer, still being worked on

## Examples

[example app](2_4_example_app/example-app.schema)

(available inside HH network only)
https://github.com/juris-futura/mod-blob/tree/main/agent-scripts
https://github.com/juris-futura/mod-blob/blob/main/app.schema





