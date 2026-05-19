---
title: Memória
description: Conceitos gerais sobre memória na JVM (Stack e Heap), memory leaks e resposta para entrevistas.
category: Backend
review_date: 2026-05-19
---

# Memória

## Visão geral

A JVM divide a memória principalmente em duas áreas: `Stack` (memória de pilha) e `Heap` (memória de heap).

A JVM divide memória principalmente em:

### Stack (Stack Memory)
Armazena:
- variáveis locais
- parâmetros de métodos
- referências de objetos
- chamadas de métodos

Cada thread possui sua própria Stack.

### Heap (Heap Memory)
Armazena:
- objetos
- arrays
- instâncias de classes

A Heap é compartilhada entre threads e é gerenciada pelo Garbage Collector.
## Memory leak (vazamento de memória)
Mesmo com coleta de lixo (GC), um vazamento de memória ocorre quando referências desnecessárias impedem que objetos sejam coletados.

Exemplos comuns:
- objetos presos em cache
- listas nunca limpas
- listeners/registrations não removidos
## Exemplo de resposta para entrevista

“A Heap é a área de memória da JVM usada para armazenar objetos e instâncias criadas dinamicamente. Ela é compartilhada entre threads e gerenciada pelo Garbage Collector, que remove objetos sem referências ativas.”

## Referências


