
# 📚 Pilhas

## 📖 Definição
Uma **pilha** é uma estrutura de dados do tipo **LIFO** (Last In, First Out), onde o último elemento inserido é o primeiro a ser removido. Pode ser imaginada como uma pilha de pratos: o último prato colocado é o primeiro a ser retirado.

**Características:**
- **Inserção** e **remoção** de elementos ocorrem apenas no topo da pilha.
- **Operações principais**: `push` (inserir), `pop` (remover), `top` (visualizar o topo da pilha).
- **Tamanho dinâmico**: A pilha cresce ou diminui conforme a inserção ou remoção de elementos.

**Vantagens:**
- Simples de implementar e entender.
- Muito eficiente para aplicações onde a ordem de execução é reversa.

**Desvantagens:**
- Não permite acesso a elementos no meio da pilha.
- Limitada ao acesso do topo, o que pode ser restritivo em alguns casos.

## 🌎 Aplicação no Mundo Real
**Recursão**: Pilhas são usadas em implementações de chamadas recursivas, mantendo o estado de cada chamada até que todas as funções sejam concluídas.

## 🛠 Exemplo Prático
**Problema:** Implementar uma pilha para armazenar e imprimir números.

## 💻 Código em C++
```cpp
#include <iostream>
#include <stack>
using namespace std;

int main() {
    stack<int> pilha;

    // Inserindo elementos na pilha
    pilha.push(10);
    pilha.push(20);
    pilha.push(30);

    cout << "Elementos da pilha (do topo para o fundo):" << endl;
    while (!pilha.empty()) {
        cout << pilha.top() << " ";
        pilha.pop();  // Removendo o topo
    }

    return 0;
}
```

## 🎯 Resumo Final
- Pilhas são úteis em problemas que envolvem a ordem de execução reversa.
- Usadas em algoritmos de navegação, recursão e desfazer/refazer operações.
