# Reconhecedor Javascript - BNF


### Regras
```
<program> -> <stmts>
<stmts> -> <stmt>
<stmt> -> <type> <var> = <expr> | <var> = <expr> | <type> <var> = <declare>
<declare> { } | [ ]
<type> -> let | const | var
<var> -> a...z, A...Z, 0...9
<expr> -> 0...9 | a...z, A...Z |<expr> <sinal> <expr>
<sinal> -> + | - | / | * |

```

### Exemplos de atribuições
```
<program> => <stmts> => <stmt> => <type> <var> = <expr> => let <var> = <expr>
=> let soma = <expr> => let soma = <expr> <sinal> <expr> => let soma = 7 <sinal> <expr>
=> let soma = 7 + <expr> => let soma = 7 + “ola”
<program> => <stmts> => <stmt> => <type> <var> = <declare> => let <var> = <declare>
=> let pessoa = <declare> => let pessoa = { }

```
