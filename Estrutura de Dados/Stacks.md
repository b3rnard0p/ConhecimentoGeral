# 📚 Pilha (Stack)

## 📖 Definição
Uma **pilha** é uma estrutura de dados que segue o princípio de **LIFO** (Last In, First Out), ou seja, o último elemento a ser inserido é o primeiro a ser removido.

**Características:**
- Elementos são inseridos e removidos no topo da pilha.
- Operações de inserção (push) e remoção (pop) são feitas no topo, o que garante a ordem LIFO.
- Tamanho pode ser variável, dependendo da implementação.

**Vantagens:**
- Permite acesso rápido ao último elemento inserido.
- Ideal para problemas que exigem retrocesso ou devolução de estados anteriores (como em desfazer/retomar ações).

**Desvantagens:**
- Acesso aos elementos não é possível de maneira aleatória, somente ao topo da pilha.
- Não permite inserção ou remoção em posições específicas.

## 🌎 Aplicação no Mundo Real
**Desfazer/Refazer em Editores de Texto**: A pilha é usada para manter um histórico de ações do usuário, permitindo desfazer ou refazer as ações na ordem inversa.

## 🛠 Exemplo Prático
**Problema:** Implementar uma pilha para controlar as páginas visitadas em um navegador de internet, permitindo voltar para a última página acessada.

## 💻 Código em C++
```cpp
#include <iostream>
#include <stack>
using namespace std;

int main() {
    stack<string> pilha;
    string url;
    int num_paginas;

    cout << "Quantas páginas foram visitadas? ";
    cin >> num_paginas;

    // Adiciona as URLs na pilha
    for (int i = 0; i < num_paginas; i++) {
        cout << "Digite o URL da página " << i + 1 << ": ";
        cin >> url;
        pilha.push(url);
    }

    // Navegar para trás (voltar para a última página visitada)
    cout << "\nVoltando para as páginas visitadas...\n";
    while (!pilha.empty()) {
        cout << "Voltando para: " << pilha.top() << endl;
        pilha.pop();  // Remove a página da pilha
    }

    return 0;
}
```

# 🎯 Resumo Final
- Pilhas são ideais para lidar com tarefas de retrocesso ou devolução de estados.
- Usadas em controle de histórico de navegação, execução de funções recursivas e algoritmos que necessitam de ordem inversa.
