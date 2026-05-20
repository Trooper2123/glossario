# Steams

**Categoria:** Backend | **Data de Revisão:** 19/05/2026

## O que é?
Forma de processamento de dados vindos de Array ou Collections.
É uma pipe de conversão de dados, não funciona como forma de armazenamento de dados, uma vez que 
os dados gerados existem apenas no contexto do processo.

## Características Chave
 - **Estilo Declarativo**: Concentra-se no **o que fazer** com os dados em vez de **como iterar** sobre eles,
    tornando o código mais legível. 
 - **Laziness**: As operações são otimizadas pela JVM. Por exemplo, se você usar `limit(5)`, o fluxo para de processar 
assim que encontrar os primeiros cinco elementos correspondentes. 
 - **Paralelismo**: Você pode processar dados facilmente em paralelo usando `parallelStream()` para aproveitar processadores multi-core, 
embora isso deva ser usado com cautela para conjuntos de dados pequenos.
 - **Fluxos Primitivos**: Existem especializações como `IntStream`, `LongStream` e `DoubleStream` para melhor desempenho com tipos primitivos.


| Operation Type | Examples | Description |
|---|---|---|
| Intermediate | filter(predicate) | Selects elements based on a condition. |
| Intermediate | map(function) | Transforms each element into another object. |
| Intermediate | sorted() | Sorts the elements. |
| Intermediate | distinct() | Removes duplicates. |
| Terminal | collect(Collectors.toList()) | Converts the stream back into a collection. |
| Terminal | forEach(consumer) | Performs an action for each element. |
| Terminal | findFirst() | Returns the first element found. |
| Terminal | reduce(identity, accumulator) | Combines elements into a single value. |

## Referências

## Tags
`#java` `#backend` `#sistemas`
