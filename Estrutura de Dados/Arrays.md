
# 📚 Arrays

## 📖 Definição
Arrays são estruturas de dados que armazenam **múltiplos elementos do mesmo tipo** em **posições contíguas de memória**.
Cada elemento é acessado por um **índice**, que geralmente começa em 0.

**Características:**
- Tamanho fixo (definido na criação).
- Acesso rápido a elementos individuais (`O(1)` tempo).
- Inserções e remoções podem ser custosas (`O(n)` tempo).
- Ideal para dados densos e bem definidos.

**Vantagens:**
- Simples de usar e entender.
- Permite acesso direto a qualquer elemento.

**Desvantagens:**
- Difícil de redimensionar.
- Inserir/remover no meio do array exige deslocamento de elementos.

## 🌎 Aplicação no Mundo Real
**Processamento de Imagens**: Imagens digitais são representadas como arrays 2D de pixels.

## 🛠 Exemplo Prático
**Problema:** Calcular a média da temperatura da semana armazenada em um array.

## 💻 Código em C++
```cpp
#include <iostream>
using namespace std;

int main() {
    const int dias_semana = 7;
    float temperaturas[dias_semana];

    cout << "Digite as temperaturas dos 7 dias:
";
    for (int i = 0; i < dias_semana; i++) {
        cout << "Dia " << i + 1 << ": ";
        cin >> temperaturas[i];
    }

    float soma = 0;
    for (int i = 0; i < dias_semana; i++) {
        soma += temperaturas[i];
    }

    float media = soma / dias_semana;

    cout << "
A temperatura média da semana foi: " << media << "°C" << endl;

    return 0;
}
```

# 🎯 Resumo Final
- Arrays são essenciais para dados homogêneos.
- Usados em sistemas de imagem, áudio e IA.
