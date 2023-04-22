

<h1 align="center"> Atividade 04 </h1>

Atualmente os gastos mensais de uma empresa são feitos em planilhas eletrônicas. Assim, para fechar o balanço do primeiro trimestre, é necessário somar o gasto total. Sabendo que, em janeiro, foram gastos R$ 30.000,00 reais, em fevereiro, R$ 33.030,77 reais e em Março, R$ 23.899,01 reais, faça uma classe em Java que calcule e exiba o gasto total
no trimestre, seguindo os seguintes passos:

a) Crie uma classe chamada BalancoTrimestral com o método main;
b) No método principal, declare uma variável chamada gastosJaneiro e inicialize-a com o valor gasto no mês de janeiro;
c) Crie também as variáveis gastosFevereiro e gastosMarco, inicializando-as com os respectivos gastos, utilize uma linha para cada declaração;
d) Crie uma variável chamada gastosTrimestre e inicialize-a com a soma das outras variáveis;
e) Exiba a variável gastosTrimestre.


# Código comentado:

public class BalancoTrimestral {
    public static void main(String[] args) {
        // declaração e inicialização das variáveis de gastos
        double gastosJaneiro = 30000.00;
        double gastosFevereiro = 33030.77;
        double gastosMarco = 23899.01;

        // cálculo da soma dos gastos e exibição
        double gastosTrimestre = gastosJaneiro + gastosFevereiro + gastosMarco;
        System.out.println("Gastos trimestre: " + gastosTrimestre);

        // cálculo da média mensal de gastos e exibição
        double mediaMensal = gastosTrimestre / 3;
        System.out.println("Média mensal de gastos: " + mediaMensal);
        }
}    
