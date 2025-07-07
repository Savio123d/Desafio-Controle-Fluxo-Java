# Desafio de Controle de Fluxo - Contador

Este projeto é a resolução do desafio "Controle de Fluxo" do bootcamp da DIO. O objetivo é criar um programa que recebe dois números inteiros como parâmetros e imprime no console a contagem de números no intervalo entre eles.

## 📝 Descrição do Projeto

O programa, chamado `Contador`, solicita ao usuário a inserção de dois valores inteiros via terminal. Em seguida, ele verifica se o segundo número é maior que o primeiro. Caso seja, o programa realiza uma iteração, imprimindo no console os números de 1 até a diferença entre os dois valores fornecidos. Se o primeiro número for maior ou igual ao segundo, o programa lança uma exceção customizada para tratar a entrada inválida.

## 🚀 Funcionalidades

  - **Entrada de Dados**: O programa utiliza a classe `Scanner` para receber dois parâmetros numéricos inteiros do usuário.
  - **Validação de Parâmetros**: Um método `contar` é responsável por verificar se o primeiro parâmetro é maior que o segundo. Se essa condição for verdadeira, uma exceção `ParametrosInvalidosException` é lançada.
  - **Contagem e Impressão**: Se os parâmetros forem válidos, o programa calcula a diferença entre eles e utiliza um laço `for` para imprimir os números sequencialmente.
  - **Tratamento de Exceção**: O bloco `main` utiliza uma estrutura `try-catch` para capturar a `ParametrosInvalidosException` e exibir uma mensagem de erro amigável ao usuário.

## 🛠️ Tecnologias Utilizadas

  - **Java**: O projeto foi desenvolvido inteiramente em Java.
  - **IDE**: O repositório contém arquivos de configuração para a IDE IntelliJ IDEA (conforme os arquivos no diretório `.idea`).

## 📂 Estrutura do Repositório

O projeto está estruturado da seguinte forma:

```
├── .gitignore
├── .idea/
│   ├── .gitignore
│   ├── misc.xml
│   ├── modules.xml
│   └── vcs.xml
├── out/
└── src/
    ├── Contador.java
    └── ParametrosInvalidosException.java
```

  - `src/Contador.java`: Classe principal que contém a lógica para solicitar os dados, chamar o método de contagem e tratar a exceção.
  - `src/ParametrosInvalidosException.java`: Classe de exceção customizada que herda de `RuntimeException`.
  - `.gitignore`: Arquivo que especifica os arquivos e diretórios a serem ignorados pelo Git, como os gerados pela IDE.
  - `.idea/`: Diretório com arquivos de configuração específicos da IDE IntelliJ IDEA.

## ▶️ Como Executar

1.  **Clone o repositório:**

    ```bash
    git clone <URL-DO-SEU-REPOSITORIO>
    ```

2.  **Navegue até o diretório do projeto:**

    ```bash
    cd <NOME-DO-DIRETORIO>
    ```

3.  **Compile os arquivos Java:**
    Navegue até a pasta `src` e execute o seguinte comando:

    ```bash
    javac *.java
    ```

4.  **Execute o programa:**
    Ainda no diretório `src`, execute a classe principal:

    ```bash
    java Contador
    ```

5.  **Interaja com o programa:**
    O terminal solicitará que você digite os dois parâmetros.

    **Exemplo de execução válida:**

    ```
    Digite o primeiro parâmetro:
    2
    Digite o segundo parâmetro:
    5
    Imprimindo o número: 1
    Imprimindo o número: 2
    Imprimindo o número: 3
    ```

    **Exemplo de execução inválida:**

    ```
    Digite o primeiro parâmetro:
    10
    Digite o segundo parâmetro:
    3
    O segundo parâmetro deve ser maior que o primeiro
    ```

