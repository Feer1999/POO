
<h1 align="center"> Atividade 02 </h1>

Crie uma classe em Java que realize cada uma das seguintes tarefas:

a) Exibir a mensagem "Informe um inteiro: ", deixando o cursor na mesma linha;
b) Atribuir o produto de variáveis b e c para a variável a;
c) Utilizar um comentário para afirmar que um programa executa um cálculo de exemplo de folha de pagamento.

# Código comentado:

import java.util.Scanner;

public class atv02 {
    public static void main(String[] args) {

        // a) Exibir a mensagem "Informe um inteiro: ", deixando o cursor na mesma linha;
        System.out.print("Informe um inteiro: ");
        
        // criar um objeto Scanner para ler a entrada do usuário a partir do console
        Scanner scanner = new Scanner(System.in);
        
        // ler um número inteiro do usuário e armazená-lo na variável "numero"
        int numero = scanner.nextInt();

        // b) Atribuir o produto de variáveis b e c informados pelo usuário para a variável a;
        System.out.print("Informe o valor de b: ");
        int b = scanner.nextInt();

        System.out.print("Informe o valor de c: ");
        int c = scanner.nextInt();

        // calcular o produto de b e c e armazená-lo na variável "a"
        int a = b * c;

        // c) Demonstrar a execução do cálculo e utilizar um comentário para afirmar que é um programa de exemplo de folha de pagamento.
        System.out.println("O produto de " + b + " e " + c + " é " + a + ".");
        // Este é um programa de exemplo de cálculo de folha de pagamento.
    }
}

