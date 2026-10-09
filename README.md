# ComparaSort

Projeto acadêmico que compara quatro algoritmos de ordenação em Java: Bubble Sort, Selection Sort, Quick Sort e Shell Sort. Desenvolvido no quarto semestre da graduação em Ciência da Computação.

## Objetivo e funcionalidades

O programa lê valores de um arquivo de texto, executa cada algoritmo sobre uma cópia do mesmo vetor e apresenta o tempo de execução e a quantidade de trocas em uma janela de diálogo.

## Tecnologias

Java, Swing (`JOptionPane`), leitura de arquivos e projeto NetBeans com Apache Ant. A configuração de compilação utiliza Java 8.

## Como executar

1. Instale um JDK compatível com Java 8 e o Apache NetBeans.
2. Clone o projeto:
   ```bash
   git clone https://github.com/Joice-O/APS-2024-2.git
   ```
3. Abra a pasta `ComparaSort` como projeto no NetBeans.
4. Configure `ComparaSort.Main` como classe principal.
5. Execute com a pasta `ComparaSort` como diretório de trabalho, pois o código busca `M01_2024 - 129615.txt` por um caminho relativo.
6. Aguarde a janela de resultados. Vetores grandes podem levar bastante tempo nos algoritmos quadráticos.

Não são necessárias bibliotecas externas. A janela de resultados requer ambiente com interface gráfica.

## Arquivos de entrada

A primeira linha indica a quantidade de valores; as linhas seguintes contêm os números a ordenar. O arquivo atualmente selecionado está definido em `src/ComparaSort/Main.java`. Para utilizar outra amostra, altere essa referência e confira o formato dos dados.

## Estrutura

- `src/ComparaSort/Main.java`: leitura e comparação.
- `BubbleSort.java`, `SelectionSort.java`, `QuickSort.java`, `ShellSort.java`: algoritmos.
- `Resultado.java`: registro das trocas.
- Arquivos `.txt`: amostras.
- `build.xml` e `nbproject`: configuração do projeto.

## Autoria

Projeto acadêmico publicado por [Joice Oliveira Jardim](https://github.com/Joice-O). O histórico de commits registra as contribuições ao código.

## Limitações da comparação

A medição usa `System.currentTimeMillis()`, sem aquecimento da JVM ou repetições estatísticas. Os resultados representam um experimento didático, não um benchmark rigoroso. A correção de cada implementação deve ser validada antes de tirar conclusões gerais.

