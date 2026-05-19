# Operadores

**Categoria:** Backend | **Data de Revisão:** 19/05/2026

## O que é?


## Diferença entre == e equals()

`==` compara referência de memória.

`equals()` compara conteúdo/valor do objeto.

Exemplo:

```java
String a = new String("teste");
String b = new String("teste");

a == b // false
a.equals(b) // true
```

### Em resumo
Pode usar `==` quando:
* tipos primitivos (int, long, etc.)
* deseja comparar referência de objetos

* Use `equals()` quando:
* quiser comparar conteúdo/valor de objetos (Integer, String, BigDecimal, etc.)

“Em Java usamos == para comparar valores de tipos primitivos. Já para objetos, == compara referência de memória. Para comparar conteúdo usamos equals().”

#### Curiosidade 

 **Integer Cache**

Java mantém cache automático para valores entre -128 e 127.
Isso acontece porque:

* 127 reutiliza o mesmo objeto do cache
* 128 cria objetos diferentes

## Referências