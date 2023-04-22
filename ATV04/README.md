

<h1 align="center"> Atividade 04 </h1>

# Código comentado:

public class BalancoTrimestral {
    public static void main(String[] args) {
        // declaração e inicialização das variáveis de gastos
        double gastosJaneiro = 1500.0;
        double gastosFevereiro = 2000.0;
        double gastosMarco = 1800.0;

        // cálculo da soma dos gastos e exibição
        double gastosTrimestre = gastosJaneiro + gastosFevereiro + gastosMarco;
        System.out.println("Gastos trimestre: " + gastosTrimestre);

        // cálculo da média mensal de gastos e exibição
        double mediaMensal = gastosTrimestre / 3;
        System.out.println("Média mensal de gastos: " + mediaMensal);
    }
}
