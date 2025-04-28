# 📚 Listas Ligadas

## 📖 Definição
Uma **lista ligada** é uma estrutura de dados composta por uma sequência de **nós**, onde cada nó contém dois elementos:
1. **Valor**: O dado armazenado no nó.
2. **Ponteiro**: Um endereço que aponta para o próximo nó na lista.

Cada nó é dinamicamente alocado e os elementos não são armazenados em posições contíguas na memória, ao contrário de arrays.

**Características:**
- **Dinâmica**: Tamanho da lista pode ser alterado durante a execução do programa.
- **Acesso sequencial**: Para acessar um nó, é necessário percorrer a lista a partir do início.
- **Inserção/remoção eficientes**: Inserções e remoções em listas ligadas podem ser feitas em tempo constante (`O(1)`), desde que o nó de inserção/remoção seja conhecido.

**Vantagens:**
- Não há necessidade de alocar memória de forma contínua.
- Facilita operações de inserção e remoção em listas grandes.

**Desvantagens:**
- Acesso aos elementos é sequencial, o que pode ser ineficiente (`O(n)`).
- Mais espaço de memória é necessário para armazenar os ponteiros.

## 🌎 Aplicação no Mundo Real
**Gerenciamento de Memória**: Em sistemas operacionais, listas ligadas são usadas para gerenciar blocos de memória que podem ser alocados ou liberados dinamicamente.

## 🛠 Exemplo Prático
**Problema:** Criar uma lista ligada para armazenar e exibir os números de uma sequência.

## 💻 Código em C++
```cpp
#include <iostream>
using namespace std;

struct Node {
    int valor;
    Node* proximo;
};

class ListaLigada {
private:
    Node* cabeca;

public:
    ListaLigada() {
        cabeca = nullptr;
    }

    void adicionar(int valor) {
        Node* novoNo = new Node();
        novoNo->valor = valor;
        novoNo->proximo = cabeca;
        cabeca = novoNo;
    }

    void exibir() {
        Node* atual = cabeca;
        while (atual != nullptr) {
            cout << atual->valor << " ";
            atual = atual->proximo;
        }
        cout << endl;
    }

    ~ListaLigada() {
        Node* atual = cabeca;
        while (atual != nullptr) {
            Node* temp = atual;
            atual = atual->proximo;
            delete temp;
        }
    }
};

int main() {
    ListaLigada lista;
    lista.adicionar(10);
    lista.adicionar(20);
    lista.adicionar(30);
    lista.exibir();

    return 0;
}
```

## 🎯 Resumo Final
- Listas ligadas são eficientes para inserções e remoções rápidas.
- Usadas para implementação de pilhas, filas e sistemas de gerenciamento de memória.
