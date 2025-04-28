📚 Filas
📖 Definição
Uma fila é uma estrutura de dados do tipo FIFO (First In, First Out), onde o primeiro elemento inserido é o primeiro a ser removido. Pode ser imaginada como uma fila de pessoas esperando para serem atendidas: a primeira pessoa a entrar na fila é a primeira a ser atendida.

Características:

Inserção (enqueue) é realizada no final da fila.

Remoção (dequeue) é realizada no início da fila.

Operações principais: enqueue (inserir), dequeue (remover), front (visualizar o primeiro da fila).

Vantagens:

Simples e eficiente para problemas onde a ordem de chegada importa.

Adequada para modelar sistemas de espera, como atendimento ao cliente.

Desvantagens:

Não permite acesso direto aos elementos no meio da fila.

Limitações para operações de inserção e remoção.

🌎 Aplicação no Mundo Real
Atendimento de Processos: Filas são utilizadas em sistemas operacionais para o agendamento de processos em espera para execução.

🛠 Exemplo Prático
Problema: Implementar uma fila para armazenar e processar números.

💻 Código em C++
cpp
Copiar
Editar
#include <iostream>
#include <queue>
using namespace std;

int main() {
    queue<int> fila;

    // Inserindo elementos na fila
    fila.push(10);
    fila.push(20);
    fila.push(30);

    cout << "Elementos da fila (do primeiro para o último):" << endl;
    while (!fila.empty()) {
        cout << fila.front() << " ";  // Visualizando o primeiro elemento
        fila.pop();  // Removendo o primeiro elemento
    }

    return 0;
}
🎯 Resumo Final
Filas são úteis em problemas de gerenciamento de tarefas ou processos em ordem de chegada.

Usadas em sistemas de impressão, redes e filas de processos.
