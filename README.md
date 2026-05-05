# Analise-biomecanica

# Atividade Prática 1 - Grupo 3

Este notebook é parte de um exercício prático desenvolvido por um grupo de alunos de Engenharia Biomédica. O objetivo é processar dados biomecânicos coletados de marcadores em diferentes velocidades, e realizar análises como a comparação de dados e visualização dos resultados.

## 0. Importações e Funções Auxiliares

O código faz uso das bibliotecas:
- **NumPy** e **Pandas** para manipulação de dados.
- **Matplotlib** para a criação de gráficos.
- **SciPy** para o uso de funções como `find_peaks` (detecção de picos), `butter` e `filtfilt` (filtros digitais), e interpolação com `interp1d`.
- **Warnings** para gerenciar as mensagens de alerta.

Essas bibliotecas são essenciais para a análise e visualização dos dados de forma eficiente.

## 1. Carregamento dos Dados

Os dados utilizados no projeto são coordenadas de marcadores posicionados em diferentes partes do corpo humano. Os marcadores são:
- **A** = Acrômio
- **T** = Trocânter
- **E** = Epicôndilo lateral do fêmur
- **M** = Maléolo lateral
- **C** = Calcâneo
- **5Mt** = 5º Metatarso

Existem três arquivos de dados disponíveis:
- `bel_4_dados.txt` → dados a 4 km/h
- `bel_5_dados.txt` → dados a 5 km/h
- `bel_6_dados.txt` → dados a 6 km/h

A função `load_data(filepath)` é utilizada para carregar os dados, tratando os valores e preparando-os para análise.

### Saída esperada após o carregamento:
- **Velocidade 4**: 541 amostras
- **Velocidade 5**: 829 amostras
- **Velocidade 6**: 1084 amostras

## Instruções de Uso

1. **Importação das bibliotecas**: Certifique-se de ter todas as dependências instaladas (NumPy, Pandas, Matplotlib, SciPy).
2. **Carregamento dos dados**: Os dados podem ser carregados a partir dos arquivos `.txt` mencionados. O notebook está configurado para carregar os arquivos `bel_4_dados.txt`, `bel_5_dados.txt`, e `bel_6_dados.txt`.
3. **Análise**: Após carregar os dados, você pode proceder com a análise gráfica e interpretação dos resultados.
