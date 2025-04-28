# 📚 Grafo (Graph)

## 📖 Definição
Um **grafo** é uma estrutura de dados composta por **vértices** (ou nós) e **arestas** (ou arcos) que conectam os vértices. Ele pode ser **direcionado** (onde as arestas possuem uma direção) ou **não direcionado** (onde as arestas não possuem direção).

**Características:**
- **Vértices** são os pontos de conexão.
- **Arestas** conectam os vértices.
- Pode ser **ponderado** (as arestas têm um peso associado) ou **não ponderado** (sem pesos nas arestas).
- Pode ser **conexo** (há um caminho entre todos os vértices) ou **desconexo** (não há caminho entre todos os vértices).

**Vantagens:**
- Flexível e capaz de representar uma grande variedade de relações complexas.
- Ideal para problemas como redes de computadores, mapas, fluxos, entre outros.

**Desvantagens:**
- Operações de busca e manipulação de grafos podem ser mais complexas, especialmente para grafos grandes.
- O uso de memória pode ser alto dependendo da implementação (listas de adjacência vs. matrizes de adjacência).

## 🌎 Aplicação no Mundo Real
**Redes de Comunicação**: A arquitetura da internet, onde os computadores e roteadores são vértices e as conexões entre eles são arestas.

## 🛠 Exemplo Prático
**Problema:** Implementar um grafo não direcionado e não ponderado para representar conexões entre cidades, e buscar se existe um caminho entre duas cidades.

## 💻 Código em C++
```cpp
#include <iostream>
#include <list>
#include <queue>
using namespace std;

// Classe para representar um grafo
class Grafo {
    int V; // Número de vértices
    list<int>* adj; // Lista de adjacência

public:
    Grafo(int V); // Construtor
    void adicionarAresta(int v, int w); // Adiciona aresta
    bool buscaLargura(int origem, int destino); // Verifica se há caminho
};

// Construtor do grafo
Grafo::Grafo(int V) {
    this->V = V;
    adj = new list<int>[V];
}

// Função para adicionar uma aresta entre dois vértices
void Grafo::adicionarAresta(int v, int w) {
    adj[v].push_back(w); // Adiciona w à lista de adjacência de v
    adj[w].push_back(v); // Como é um grafo não direcionado
}

// Função para verificar se há caminho entre dois vértices
bool Grafo::buscaLargura(int origem, int destino) {
    bool* visitado = new bool[V];
    for (int i = 0; i < V; i++) {
        visitado[i] = false;
    }

    queue<int> fila;
    visitado[origem] = true;
    fila.push(origem);

    while (!fila.empty()) {
        int v = fila.front();
        fila.pop();

        // Verifica se chegou ao destino
        if (v == destino) {
            return true;
        }

        // Visita todos os vizinhos do vértice v
        for (int adjacente : adj[v]) {
            if (!visitado[adjacente]) {
                visitado[adjacente] = true;
                fila.push(adjacente);
            }
        }
    }

    return false; // Não há caminho entre origem e destino
}

int main() {
    Grafo g(5); // Criando grafo com 5 vértices

    // Adicionando arestas
    g.adicionarAresta(0, 1);
    g.adicionarAresta(0, 2);
    g.adicionarAresta(1, 3);
    g.adicionarAresta(3, 4);

    int origem, destino;
    cout << "Digite o vértice de origem e o de destino para verificar o caminho: ";
    cin >> origem >> destino;

    if (g.buscaLargura(origem, destino)) {
        cout << "Há um caminho entre os vértices " << origem << " e " << destino << "." << endl;
    } else {
        cout << "Não há caminho entre os vértices " << origem << " e " << destino << "." << endl;
    }

    return 0;
}
```

# 🎯 Resumo Final
- Grafos são estruturas poderosas para representar relações complexas entre objetos.
- Usados em redes de computadores, rotas de transporte, redes sociais e muitos outros problemas relacionados à conectividade e fluxo de dados.
