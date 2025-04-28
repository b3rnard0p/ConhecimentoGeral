# 📚 Algoritmos de Ordenação

## 📖 Definição
Algoritmos de ordenação são métodos usados para **organizar** um conjunto de dados (geralmente uma lista ou array) em uma ordem específica, geralmente **crescente** ou **decrescente**. A ordenação é uma operação fundamental em muitos algoritmos e sistemas, e sua eficiência pode impactar significativamente o desempenho geral.

**Características:**
- **Estabilidade**: Um algoritmo é considerado estável se ele mantiver a ordem relativa dos elementos iguais após a ordenação.
- **Complexidade de Tempo**: Refere-se ao tempo de execução do algoritmo em termos de entradas de tamanho `n`. A complexidade pode variar de acordo com o algoritmo, podendo ser `O(n^2)`, `O(n log n)`, entre outras.
- **Espaço de Memória**: Algumas ordenações requerem mais memória, enquanto outras podem ser feitas in-place (no próprio array).

## 🌎 Aplicação no Mundo Real
**Sistemas de Recomendação**: Algoritmos de ordenação são usados para classificar produtos ou conteúdos em plataformas de e-commerce ou streaming com base em popularidade, avaliação ou outros critérios.

## 🛠 Tipos Comuns de Algoritmos de Ordenação

### 1. **Bubble Sort (Ordenação por Troca)**
- **Complexidade**: `O(n^2)` no pior caso.
- **Princípio**: Compara elementos adjacentes e os troca de lugar se estiverem na ordem errada. Repete até que a lista esteja ordenada.
- **Vantagem**: Simples de implementar.
- **Desvantagem**: Ineficiente para grandes listas.

### 2. **Selection Sort (Ordenação por Seleção)**
- **Complexidade**: `O(n^2)` no pior caso.
- **Princípio**: Encontra o menor (ou maior) elemento da lista e coloca-o na posição correta. Repete para os outros elementos.
- **Vantagem**: Não necessita de memória extra.
- **Desvantagem**: Ineficiente para listas grandes.

### 3. **Insertion Sort (Ordenação por Inserção)**
- **Complexidade**: `O(n^2)` no pior caso, mas `O(n)` no melhor caso (quando a lista já está parcialmente ordenada).
- **Princípio**: Insere cada elemento na posição correta em uma sublista ordenada.
- **Vantagem**: Muito eficiente para listas pequenas ou quase ordenadas.
- **Desvantagem**: Lento para grandes listas.

### 4. **Merge Sort (Ordenação por Mesclagem)**
- **Complexidade**: `O(n log n)` no pior caso.
- **Princípio**: Divide a lista em sublistas menores, ordena-as recursivamente e depois as mescla.
- **Vantagem**: Eficiência garantida.
- **Desvantagem**: Requer memória extra.

### 5. **Quick Sort (Ordenação Rápida)**
- **Complexidade**: `O(n log n)` no pior caso (com a escolha correta de pivô).
- **Princípio**: Seleciona um pivô e particiona a lista em duas partes (menores e maiores que o pivô), e então ordena as partes recursivamente.
- **Vantagem**: Muito eficiente na prática.
- **Desvantagem**: Requer cuidado na escolha do pivô para evitar o pior caso.

## 💻 Exemplo Prático
**Problema:** Ordenar um vetor de números inteiros usando o algoritmo **Quick Sort**.

## 💻 Código em C++ (Quick Sort)
```cpp
#include <iostream>
using namespace std;

// Função para realizar a troca de elementos
void trocar(int& a, int& b) {
    int temp = a;
    a = b;
    b = temp;
}

// Função de partição para o Quick Sort
int particionar(int arr[], int baixo, int alto) {
    int pivo = arr[alto];  // Escolhe o último elemento como pivô
    int i = (baixo - 1);    // Índice do menor elemento
    for (int j = baixo; j <= alto - 1; j++) {
        if (arr[j] < pivo) {
            i++;
            trocar(arr[i], arr[j]);
        }
    }
    trocar(arr[i + 1], arr[alto]);
    return (i + 1);
}

// Função recursiva de Quick Sort
void quickSort(int arr[], int baixo, int alto) {
    if (baixo < alto) {
        int pivo = particionar(arr, baixo, alto);  // Encontra o pivô
        quickSort(arr, baixo, pivo - 1);  // Ordena os elementos à esquerda do pivô
        quickSort(arr, pivo + 1, alto);   // Ordena os elementos à direita do pivô
    }
}

int main() {
    int arr[] = {12, 4, 7, 9, 2, 5, 10, 3};
    int n = sizeof(arr) / sizeof(arr[0]);

    cout << "Vetor original: ";
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
    cout << endl;

    quickSort(arr, 0, n - 1);  // Ordena o vetor

    cout << "Vetor ordenado: ";
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
}
```

# 🎯 Resumo Final
- **Bubble Sort, Selection Sort e Insertion Sort** são eficientes para listas pequenas, mas ineficazes para grandes volumes de dados.
- **Merge Sort e Quick Sort** oferecem eficiência superior, com complexidade `O(n log n)` no pior caso.
- A escolha do algoritmo de ordenação depende do tamanho da lista e das condições de dados (por exemplo, listas quase ordenadas).
- **Quick Sort** é geralmente o mais eficiente para listas grandes, mas exige cuidado com a escolha do pivô.
