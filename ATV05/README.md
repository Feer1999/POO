<h1 align="center"> Atividade 05 </h1>

Adicione a Atv04 (sem alterar as linhas que já existem) o cálculo para a média mensal de gastos, criando uma variável mediaMensal junto com uma mensagem. Para isso, concatene a String com o valor, usando "Valor da média mensal = " + mediaMensal.

# Código comentado:

import java.util.Scanner;

public class Atv05 {

    public static void main(String[] args) {

        // Criar objeto Scanner para obter os valores de gastos mensais do usuário
        Scanner scanner = new Scanner(System.in);

        // Definir o tamanho do array com o número de meses
        System.out.print("Digite o número de meses: ");
        int numMeses = scanner.nextInt();
        double[] gastosMensais = new double[numMeses];

        // Obter os valores de gastos mensais do usuário
        for (int i = 0; i < numMeses; i++) {
            System.out.print("Digite o gasto do mês " + (i + 1) + ": ");
            gastosMensais[i] = scanner.nextDouble();
        }

        // Calcular a soma dos gastos mensais
        double somaGastos = 0;
        for (double gasto : gastosMensais) {
            somaGastos += gasto;
        }

        // Calcular a média mensal de gastos
        double mediaMensal = somaGastos / gastosMensais.length;

        // Exibir a mensagem com o valor da média mensal de gastos
        System.out.println("Valor da média mensal = " + mediaMensal);

        // Fechar o objeto Scanner
        scanner.close();
    }
}
