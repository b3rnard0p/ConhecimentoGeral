# 📚 Tabela Hash (Hash Table)

## 📖 Definição
Uma **tabela hash** é uma estrutura de dados que associa **chaves** a **valores** utilizando uma função de hash para calcular um índice de armazenamento em uma tabela. Essa estrutura é muito eficiente para operações de busca, inserção e remoção, com complexidade média de `O(1)`.

**Características:**
- **Chave**: É a entrada usada para acessar o valor armazenado.
- **Valor**: O dado associado à chave.
- **Função de Hash**: Função que converte a chave em um índice de array.
- **Colisões**: Quando duas chaves diferentes geram o mesmo índice, elas são chamadas de colisões e precisam ser tratadas (geralmente usando listas encadeadas ou sondagem linear).

**Vantagens:**
- Acesso rápido aos dados (complexidade `O(1)` no caso ideal).
- Eficiência em operações de busca, inserção e remoção.
- Ideal para situações onde é necessário acessar dados com rapidez a partir de uma chave.

**Desvantagens:**
- Requer uma boa função de hash para evitar colisões.
- O tamanho da tabela precisa ser bem dimensionado para evitar a sobrecarga de colisões.
- Gerenciamento de colisões pode complicar a implementação.

## 🌎 Aplicação no Mundo Real
**Caches de Navegadores**: Os navegadores web usam tabelas hash para armazenar URLs e suas respectivas páginas cacheadas, permitindo acesso rápido.

## 🛠 Exemplo Prático
**Problema:** Implementar uma tabela hash simples para armazenar e buscar valores associados a chaves (por exemplo, nomes de pessoas e suas idades).

## 💻 Código em C++
```cpp
#include <iostream>
#include <list>
#include <string>
using namespace std;

// Tamanho da tabela hash
const int TABELA_HASH_SIZE = 10;

// Classe para implementar a tabela hash
class TabelaHash {
    list<pair<string, int>>* tabela;  // Lista encadeada para cada índice
public:
    TabelaHash();
    ~TabelaHash();
    int funcaoHash(string chave);
    void inserir(string chave, int valor);
    int buscar(string chave);
};

// Construtor da tabela hash
TabelaHash::TabelaHash() {
    tabela = new list<pair<string, int>>[TABELA_HASH_SIZE];
}

// Destruidor da tabela hash
TabelaHash::~TabelaHash() {
    delete[] tabela;
}

// Função de hash: converte a chave em um índice
int TabelaHash::funcaoHash(string chave) {
    int soma = 0;
    for (char c : chave) {
        soma += c;
    }
    return soma % TABELA_HASH_SIZE;
}

// Função para inserir chave e valor na tabela
void TabelaHash::inserir(string chave, int valor) {
    int indice = funcaoHash(chave);
    tabela[indice].push_back(make_pair(chave, valor));
}

// Função para buscar o valor associado a uma chave
int TabelaHash::buscar(string chave) {
    int indice = funcaoHash(chave);
    for (auto& par : tabela[indice]) {
        if (par.first == chave) {
            return par.second;
        }
    }
    return -1; // Retorna -1 se a chave não for encontrada
}

int main() {
    TabelaHash th;
    
    // Inserindo dados
    th.inserir("Ana", 25);
    th.inserir("Carlos", 30);
    th.inserir("Maria", 22);
    
    // Buscando dados
    string chave;
    cout << "Digite o nome para buscar a idade: ";
    cin >> chave;
    
    int idade = th.buscar(chave);
    if (idade != -1) {
        cout << "A idade de " << chave << " é " << idade << " anos." << endl;
    } else {
        cout << "Chave não encontrada!" << endl;
    }

    return 0;
}
```

# 🎯 Resumo Final
- As tabelas hash são ideais para acesso rápido a dados através de chaves.
- Usadas em caches, bancos de dados e sistemas de indexação, são fundamentais quando a eficiência na busca é crucial.
- A chave para o bom desempenho de uma tabela hash é a escolha de uma boa função de hash e o gerenciamento eficiente de colisões.
