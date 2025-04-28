# Estruturas de Dados — Conteúdo Aprofundado

## Arrays

### O que é?
Uma coleção de elementos de mesmo tipo, armazenados em posições contíguas de memória. Permite acesso rápido via índices.

### Características
- Tamanho fixo
- Acesso rápido (O(1))
- Inserção/remoção custosa (O(n))

### Exemplos de aplicação
- Vetores de física
- Representação de imagens

---

## Listas Ligadas (Linked Lists)

### O que é?
Uma estrutura onde cada elemento (nó) aponta para o próximo, permitindo tamanho dinâmico.

### Características
- Tamanho dinâmico
- Inserção/remoção eficiente (O(1) se referência for conhecida)
- Acesso sequencial (O(n))

### Tipos
- Lista Simples
- Lista Duplamente Ligada
- Lista Circular

### Exemplos de aplicação
- Listas de tarefas dinâmicas
- Implementação de filas e pilhas

---

## Pilhas (Stacks)

### O que é?
Estrutura LIFO (**Last In, First Out**), onde o último elemento inserido é o primeiro a ser removido.

### Operações
- `push()`: inserção
- `pop()`: remoção
- `peek()`: olhar o topo

### Exemplos de aplicação
- Controle de chamadas de funções (call stack)
- Desfazer/refazer operações

---

## Filas (Queues)

### O que é?
Estrutura FIFO (**First In, First Out**), onde o primeiro elemento inserido é o primeiro removido.

### Operações
- `enqueue()`: adicionar
- `dequeue()`: remover

### Tipos
- Fila normal
- Fila circular
- Fila de prioridade

### Exemplos de aplicação
- Impressão de documentos
- Sistemas de atendimento

---

## Árvores (Trees)

### O que é?
Estrutura hierárquica onde cada nó aponta para um ou mais filhos.

### Tipos comuns
- Árvore Binária
- Árvore de Busca Binária (BST)
- Heap
- Árvore Balanceada (AVL, Red-Black)

### Operações
- Inserção
- Remoção
- Busca

### Exemplos de aplicação
- Sistemas de arquivos
- Compiladores

---

## Grafos (Graphs)

### O que é?
Conjunto de nós (vértices) conectados por arestas.

### Tipos
- Direcionado / Não-direcionado
- Ponderado / Não-ponderado

### Representação
- Matriz de adjacência
- Lista de adjacência

### Exemplos de aplicação
- Mapas e rotas
- Redes sociais

---

## Tabelas Hash (Hash Tables)

### O que é?
Estrutura que associa **chaves** a **valores** usando função de hash para acesso rápido.

### Características
- Inserção/busca/remover em tempo médio O(1)
- Tratamento de colisões: encadeamento, endereçamento aberto

### Exemplos de aplicação
- Indexação de bancos de dados
- Implementação de caches

---

## Algoritmos de Ordenação

### Bubble Sort
- Comparar pares adjacentes e trocar se está fora de ordem.
- Complexidade: O(n²)

### Quick Sort
- Escolhe pivô, particiona menores/maiores e ordena recursivamente.
- Complexidade: O(n log n) média, O(n²) pior caso

### Merge Sort
- Divide recursivamente e mescla as partes ordenadas.
- Complexidade: O(n log n)

### Exemplos de aplicação
- Ordenação de listas, arquivos grandes
- Bases de dados

---

# Conclusão

Dominar essas estruturas é essencial para resolver problemas de forma eficiente e criar sistemas de alta performance.
Cada estrutura tem forças e fraquezas dependendo da situação prática.
