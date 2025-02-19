
# Expressions

## Challenge:

How to combine, manipulate existing atoms?


## Juvo Expression highlights:

* 1/2 of LC (application, no abstraction)
* atoms are viewed as fixed set of arrows
* this LC is seeded with a few operators:
  * `>>>`
  * `fmap`
  * `<*>` (applicative)
  * `pure`
  * currying
  * construction of input params
  * ... and a few other constructors
* Hindley-Milner typing (with support for type variables)
* JSON-able

Grammar in JSON:

```json
expr :=
  {
    "json": <json representation of Juvo data>
  }
| {
    "atom": "<atom-name>"
  }
| {
     "operator": "<operator-name>"
  }
| {
    "fxn": expr
    "x": expr
  }
```

More complex example

```json
{
    "fxn": {
        "fxn": {
            "operator": ":*:"
        },
        "x": {
            "fxn": {
                "fxn": {
                    "operator": ":$:"
                },
                "x": {
                    "operator": "__constrNT__p1;p2"
                }
            },
            "x": {
                "atom": "atom1"
            }
        }
    },
    "x": {
        "fxn": {
            "operator": "pure"
        },
        "x": {
            "json": "P2 value"
        }
    }
}
```

## Examples:

compose atom1 and atom2
```json
{
    "fxn": {
        "fxn": {
            "operator": ">>>"
        },
        "x": {
            "atom": "atom1"
        }
    },
    "x": {
        "atom": "atom2"
    }
}
```


(available inside HH network only)

https://github.com/juris-futura/juvo-way/blob/master/Expressions.md
https://github.com/juris-futura/lib-juvo-common/tree/main/test/TestEval


## Issues / Take Aways:

* hard to use
* low popularity