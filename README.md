# Desafio Contador em Java

## 📝 Descrição

Este projeto é um simples programa de console em Java que solicita ao usuário dois números inteiros. O programa então realiza uma contagem incremental com base na diferença entre os dois números, imprimindo cada passo da iteração no console. O principal objetivo é demonstrar o uso de controle de fluxo e o tratamento de exceções personalizadas em Java.

Uma exceção customizada, `ParametrosInvalidosException`, é lançada se o segundo parâmetro for menor que o primeiro, garantindo que a lógica de contagem seja sempre válida.

## ⚙️ Principais Funcionalidades

-   Recebe dois parâmetros numéricos via terminal.
-   Valida se o segundo parâmetro é maior que o primeiro.
-   Lança uma exceção personalizada (`ParametrosInvalidosException`) caso a validação falhe.
-   Realiza um loop para imprimir os números com base na diferença entre os dois parâmetros.

## 💻 Tecnologias e Linguagens Utilizadas

-   **Linguagem:** Java
-   **Ambiente de Desenvolvimento:** IntelliJ IDEA

## 📁 Estrutura de Pastas e Arquivos

O projeto está organizado da seguinte forma:

```
/
├── .gitignore
├── .idea/
│ ├── .gitignore
│ ├── misc.xml
│ ├── modules.xml
│ └── vcs.xml
└── src/
├── Contador.java
└── ParametrosInvalidosException.java
```

-   **`src/Contador.java`**: Arquivo principal que contém a lógica para solicitar os dados ao usuário, chamar o método de contagem e tratar a exceção.
-   **`src/ParametrosInvalidosException.java`**: Classe de exceção personalizada que herda de `RuntimeException`.
-   **`.idea/`**: Pasta de configuração do ambiente de desenvolvimento IntelliJ IDEA.
-   **`.gitignore`**: Arquivo que especifica os arquivos e pastas a serem ignorados pelo Git.

## ▶️ Passo a Passo de Execução

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/desafio-contador-java.git](https://github.com/seu-usuario/desafio-contador-java.git)
    ```

2.  **Navegue até o diretório do projeto:**
    ```bash
    cd desafio-contador-java/src
    ```

3.  **Compile os arquivos Java:**
    ```bash
    javac ParametrosInvalidosException.java Contador.java
    ```

4.  **Execute a classe principal:**
    ```bash
    java Contador
    ```

## 💡 Exemplo de Uso

Ao executar o programa, você verá a seguinte saída:

**Caso de Sucesso:**
```
Digite o primeiro parâmetro:
5
Digite o segundo parâmetro:
10
Imprimindo o número: 1
Imprimindo o número: 2
Imprimindo o número: 3
Imprimindo o número: 4
Imprimindo o número: 5
```

**Caso de Falha (Exceção):**
```
Digite o primeiro parâmetro:
15
Digite o segundo parâmetro:
10
O segundo parâmetro deve ser maior que o primeiro
```
