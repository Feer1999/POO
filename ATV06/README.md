<h1 align="center"> Atividade 06 </h1>

Dados os valores de um depósito fixo mensal e um montante desejado, crie uma classe para determinar quantos meses serão necessários para acumular o montante desejado, considerando juros mensais de 0,5%.

# Código comentado:

import java.util.Scanner; // Importa a classe Scanner, para receber entrada de dados do usuário

public class Atv06 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); // Cria um objeto Scanner para receber entrada de dados do usuário

        System.out.print("Digite o valor do depósito fixo mensal: "); // Exibe uma mensagem para o usuário
        double depositoMensal = scanner.nextDouble(); // Lê o valor do depósito fixo mensal informado pelo usuário

        System.out.print("Digite o valor do montante desejado: "); // Exibe uma mensagem para o usuário
        double montanteDesejado = scanner.nextDouble(); // Lê o valor do montante desejado informado pelo usuário

        double jurosMensais = 1.005; // Define o valor da taxa de juros mensais como 0,5%
        double montanteAtual = 0; // Inicializa o montante atual como zero
        int meses = 0; // Inicializa o contador de meses como zero
        while (montanteAtual < montanteDesejado) { // Enquanto o montante atual for menor que o montante desejado
            montanteAtual += depositoMensal; // Adiciona o depósito fixo mensal ao montante atual
            montanteAtual *= jurosMensais; // Multiplica o montante atual pela taxa de juros mensais
            meses++; // Incrementa o contador de meses
        }
        // Exibe a mensagem informando o número de meses necessários para acumular o montante
        System.out.println("Serão necessários " + meses + " meses para acumular o montante desejado.");  

        scanner.close();  // Fecha o objeto Scanner
    }
}


