# Desafio de Controle de Fluxo em Java

## 📜 Descrição

Este projeto é um simples programa de console em Java desenvolvido para demonstrar conceitos fundamentais de controle de fluxo. O programa solicita ao usuário dois números inteiros, valida se o segundo número é maior que o primeiro e, em caso afirmativo, imprime no console uma contagem baseada na diferença entre eles. O principal objetivo é praticar o uso de laços de repetição (`for`), condicionais (`if`) e o tratamento de exceções customizadas.

## ✨ Funcionalidades Principais

* **Entrada de Dados:** Recebe dois parâmetros numéricos inteiros via terminal.
* **Validação de Parâmetros:** Verifica se o segundo parâmetro é estritamente maior que o primeiro.
* **Tratamento de Exceção:** Lança uma exceção customizada (`ParametrosInvalidosException`) caso a validação falhe.
* **Lógica de Contagem:** Itera e imprime uma sequência de números com base na diferença entre os parâmetros fornecidos.

## 🚀 Tecnologias Utilizadas

* **Java:** Linguagem principal do projeto.
* **IDE:** Desenvolvido utilizando IntelliJ IDEA.

## 📂 Estrutura do Projeto

O projeto está organizado da seguinte forma:

```

/
├── .gitignore
├── desafio.iml
├── src/
│   ├── Contador.java                   \# Classe principal com a lógica do programa
│   └── ParametrosInvalidosException.java   \# Classe de exceção customizada
└── ...

````

## ⚙️ Instruções de Execução

Para executar o projeto localmente, siga os passos abaixo.

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/desafio-controle-fluxo-java.git](https://github.com/seu-usuario/desafio-controle-fluxo-java.git)
    ```

2.  **Navegue até o diretório do código-fonte:**
    ```bash
    cd desafio-controle-fluxo-java/src
    ```

3.  **Compile os arquivos Java:**
    ```bash
    javac Contador.java ParametrosInvalidosException.java
    ```

4.  **Execute a classe principal:**
    ```bash
    java Contador
    ```

5.  O terminal solicitará que você insira os dois parâmetros para iniciar a contagem.

##  Exemplo de Uso

### Execução com sucesso

Ao inserir um segundo parâmetro maior que o primeiro:

````

Digite o primeiro parâmetro:
5
Digite o segundo parâmetro:
8
Imprimindo o número: 1
Imprimindo o número: 2
Imprimindo o número: 3

```

### Execução com erro

Ao inserir o segundo parâmetro menor ou igual ao primeiro, a exceção é tratada:

```

Digite o primeiro parâmetro:
10
Digite o segundo parâmetro:
3
O segundo parâmetro deve ser maior que o primeiro

```

```
