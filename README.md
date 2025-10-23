# Sistema de Cadastro de Clientes

Este é um pequeno sistema para cadastrar clientes de uma loja de roupas.  
O programa cria um objeto `Cliente` com `nome` e `email` fornecidos pelo usuário e exibe uma mensagem de boas-vindas.

## Funcionalidades

- Recebe o **nome** e **email** do cliente em uma única linha.
- Armazena essas informações em um objeto da classe `Cliente`.
- Exibe uma mensagem de boas-vindas no formato:  
Cliente [nome] cadastrado com sucesso! Email: [email]

---

## Tecnologias

- Java 8 ou superior

## Estrutura do Projeto

.
├── Main.java
└── README.md

### Main.java

import java.util.Scanner;

class Cliente {
    String nome;
    String email;
    public Cliente(String nome, String email) {
        this.nome = nome;
        this.email = email;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String nome = scanner.next();
        String email = scanner.next();
        Cliente cliente = new Cliente(nome, email);
        System.out.println("Cliente " + cliente.nome + " cadastrado com sucesso! Email: " + cliente.email);
    }
}

--- 

Como Executar

1. Compile o programa:

javac Main.java

2. Execute o programa:

java Main

3. Digite o nome e email do cliente separados por espaço:

Ana ana@email.com

4. O programa exibirá:

Cliente Ana cadastrado com sucesso! Email: ana@email.com
