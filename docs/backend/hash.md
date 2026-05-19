# Streams

**Categoria:** Backend | **Data de Revisão:** 19/05/2026

## O que é?
É um algoritmo matemático que transforma qualquer conjunto de dados de entrada (como um texto, uma senha ou um arquivo inteiro)
em uma sequência de caracteres de tamanho fixo.

## Características Principais  
- **Tamanho Fixo**: Não importa se a entrada é uma única letra ou um livro de mil páginas; o hash resultante terá sempre a mesma 
quantidade de caracteres (ex: o algoritmo SHA-256 sempre gera 64 caracteres).
- **Determinístico**: A mesma entrada sempre gerará exatamente o mesmo hash.
- **Irreversível (Unidirecional)**: É matematicamente inviável descobrir os dados originais a partir do hash. 
É uma via de mão única.
- **Efeito Avalanche**: Qualquer alteração mínima na entrada (como mudar uma letra minúscula para maiúscula) altera completamente o hash resultante.

## Qual a diferença entre HashMap e ConcurrentHashMap?

`HashMap` não é thread-safe, então múltiplas threads acessando simultaneamente podem causar inconsistência de dados.

`ConcurrentHashMap` foi criado para ambientes concorrentes. Ele permite múltiplas leituras e controla bloqueios de forma
segmentada, reduzindo contenção e melhorando a performance em aplicações multithread.

### Quando usar?

* `HashMap`: aplicações single-thread
* `ConcurrentHashMap`: aplicações concorrentes, APIs, microsserviços

## Referências

## Tags
`#java` `#backend` `#sistemas`