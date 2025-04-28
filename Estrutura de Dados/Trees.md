# 📚 Árvore (Tree)

## 📖 Definição
Uma **árvore** é uma estrutura de dados hierárquica composta por **nós** conectados por **arestas**. Cada nó contém um valor e pode ter referências para outros nós (chamados de filhos), formando uma estrutura em formato de árvore.

**Características:**
- Cada nó tem **um nó pai** e **nós filhos** (exceto o nó raiz, que não tem pai).
- O primeiro nó é chamado de **raiz**.
- As **folhas** são nós que não têm filhos.
- Pode ser binária (cada nó tem no máximo dois filhos), ou pode ter mais filhos (árvores n-árias).

**Vantagens:**
- Permite organização hierárquica dos dados.
- Eficiência em operações como busca, inserção e remoção, com tempo médio de complexidade `O(log n)` em árvores balanceadas.

**Desvantagens:**
- Árvore desbalanceada pode levar a operações mais lentas (complexidade `O(n)` no pior caso).
- Implementação mais complexa que outras estruturas como listas e pilhas.

## 🌎 Aplicação no Mundo Real
**Estruturas de Diretórios**: Sistemas de arquivos em computadores utilizam árvores para organizar diretórios e arquivos.

## 🛠 Exemplo Prático
**Problema:** Implementar uma árvore binária de busca (BST) para inserir números e buscar um número específico na árvore.

## 💻 Código em C++
```cpp
#include <iostream>
using namespace std;

// Estrutura de um nó
struct Node {
    int valor;
    Node* esquerda;
    Node* direita;

    // Construtor para inicializar o nó
    Node(int val) : valor(val), esquerda(nullptr), direita(nullptr) {}
};

// Função para inserir um novo nó na árvore binária de busca
Node* inserir(Node* raiz, int valor) {
    if (raiz == nullptr) {
        return new Node(valor);
    }

    if (valor < raiz->valor) {
        raiz->esquerda = inserir(raiz->esquerda, valor);
    } else {
        raiz->direita = inserir(raiz->direita, valor);
    }

    return raiz;
}

// Função para buscar um valor na árvore
bool buscar(Node* raiz, int valor) {
    if (raiz == nullptr) {
        return false;
    }

    if (raiz->valor == valor) {
        return true;
    }

    if (valor < raiz->valor) {
        return buscar(raiz->esquerda, valor);
    } else {
        return buscar(raiz->direita, valor);
    }
}

int main() {
    Node* raiz = nullptr;
    raiz = inserir(raiz, 50);
    inserir(raiz, 30);
    inserir(raiz, 70);
    inserir(raiz, 20);
    inserir(raiz, 40);
    inserir(raiz, 60);
    inserir(raiz, 80);

    int valor;
    cout << "Digite um valor para buscar: ";
    cin >> valor;

    if (buscar(raiz, valor)) {
        cout << "Valor " << valor << " encontrado na árvore!" << endl;
    } else {
        cout << "Valor " << valor << " não encontrado na árvore." << endl;
    }

    return 0;
}
```

# 🎯 Resumo Final
- Árvores são estruturas hierárquicas ideais para representar dados com relações pai-filho.
- Usadas em sistemas de arquivos, algoritmos de busca (como árvores binárias de busca) e diversas outras aplicações em computação.
