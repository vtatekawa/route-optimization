
### README: Script de Otimização de Rotas usando grafos 🚗🗺️

---

## 📚 Índice

- [Visão Geral](#visão-geral)
- [Descrição do Problema](#descrição-do-problema)
- [Estrutura dos Dados de Entrada](#estrutura-dos-dados-de-entrada)
- [Dependências](#dependências)
- [Uso](#uso)
- [Saída](#saída)

---

## 📋 Visão Geral

Bem-vindo ao projeto de **Otimização de Rotas**! Este repositório contém um script em Python que utiliza as bibliotecas `OSMnx`, `NetworkX` e `Folium` em conjunto para calcular e demonstrar a rota mais eficiente entre vários pontos em uma determinada localidade. Abaixo, você encontrará um guia abrangente sobre o que este script faz, como usá-lo e como estruturar seus dados de entrada. Vamos lá! 🚀

---

## 🔍 Descrição do Problema

Este script tem como objetivo usar grafos para encontrar a rota mais eficiente entre diversos pontos de interesse em uma localidade específica. Ele resolve problemas de otimização de rotas, o que é particularmente útil para logística e transporte.

### 🏭 O Problema de Otimização

O script visa:

1. **Minimizar o Comprimento da Rota**: Calcular a rota mais curta entre múltiplos pontos utilizando um grafo de ruas.
2. **Encontrar a Rota Mais Eficiente**: Utilizar o Algoritmo do Vizinho Mais Próximo para determinar a sequência ideal de paradas.
3. **Visualizar a Rota**: Criar um mapa interativo com a rota calculada, facilitando a visualização e análise.

---

## 📂 Estrutura dos Dados de Entrada

### Endereços das Paradas

Os endereços das paradas devem ser fornecidos no arquivo excel Endereços na pasta input (a origem deve ser o primeiro endereço da lista), por exemplo:

```python
enderecos = ['Parque Villa-Lobos, Alto de Pinheiros, são paulo, Brazil',
             'Parque Povo, Vila Olimpia, São Paulo, Brazil',
             'Parque do ibirapuera, Moema, São Paulo, Brazil',
             'Estadio do Pacaembu, Pacaembu, São Paulo, Brazil',
             'Estadio do Morumbi, Morumbi, São Paulo, Brazil',
             'Estadio allianz parque, Barra Funda, São Paulo, Brazil',
             'Parque da agua branca, Barra Funda, São Paulo, Brazil'
             ]
```

---

## 🛠 Dependências

Certifique-se de ter as seguintes dependências instaladas:

- Python 3.x
- OSMnx
- NetworkX
- Folium
- Pandas

Instale-as usando `pip`:

```bash
pip install requirements.txt
```

---

## 🚀 Uso

1. Clone este repositório:

Apenas rode cada uma das celulas do notebook.

2. **Configure os endereços e a localidade** no script:

   ```python
   localidade = 'São Paulo, Brazil'
   distancia = 50000  # 50 km
   enderecos = lista criada a partir do input em Excel
   ```

3. **Execute o script**:

   ```bash
   python script_roteamento.py
   ```

---

## 📈 Saída

Após executar o script, você obterá:

- **Mapa Interativo**: Um arquivo HTML (`mapa_da_rota.html`) com a rota calculada e marcadores para cada parada.
- **Detalhes da Rota**: Um DataFrame com informações detalhadas sobre a rota, incluindo coordenadas e endereços.

### Exemplo de Saída

![Exemplo de Mapa Interativo](mapa_da_rota.html)

---

Feito com 🧠 por [Vitor Tatekawa](https://github.com/vtatekawa)

