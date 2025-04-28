# 📚 Fila (Queue)

## 📖 Definição
Uma **fila** é uma estrutura de dados que segue o princípio de **FIFO** (First In, First Out), ou seja, o primeiro elemento a ser inserido é o primeiro a ser removido.

**Características:**
- Os elementos são inseridos no final da fila e removidos do início.
- Operações de inserção (enqueue) e remoção (dequeue) são feitas nas extremidades específicas.
- Tamanho pode ser variável, dependendo da implementação.

**Vantagens:**
- Organiza dados de forma eficiente quando a ordem de chegada é importante.
- Ideal para problemas em que os elementos precisam ser processados na ordem em que são adicionados.

**Desvantagens:**
- Não permite acesso direto a um elemento no meio da fila.
- Inserções e remoções são limitadas ao final (inserção) e início (remoção).

## 🌎 Aplicação no Mundo Real
**Sistemas de Atendimento**: Como filas em bancos, supermercados, ou call centers, onde o primeiro a chegar é o primeiro a ser atendido.

## 🛠 Exemplo Prático
**Problema:** Implementar uma fila de atendimento para clientes em um restaurante, onde os clientes são atendidos na ordem de chegada.

## 💻 Código em C++
```cpp
#include <iostream>
#include <queue>
using namespace std;

int main() {
    queue<string> fila;
    string nome_cliente;
    int num_clientes;

    cout << "Quantos clientes estão na fila? ";
    cin >> num_clientes;

    // Adiciona os clientes na fila
    for (int i = 0; i < num_clientes; i++) {
        cout << "Digite o nome do cliente " << i + 1 << ": ";
        cin >> nome_cliente;
        fila.push(nome_cliente);
    }

    // Processa os clientes na ordem de chegada
    cout << "\nAtendendo os clientes...\n";
    while (!fila.empty()) {
        cout << "Atendendo: " << fila.front() << endl;
        fila.pop();  // Remove o cliente da fila
    }

    return 0;
}
```

# 🎯 Resumo Final
- Filas são estruturas eficientes para gerenciar dados de forma sequencial e por ordem de chegada.
- Usadas em sistemas de atendimento, filas de impressão e processamento de tarefas.
