
<h1 align="center"> Atividade 01 </h1>

Crie uma classe em Java que seja capaz de apresentar a soma de todos os argumentos inteiros ou reais recebidos. Argumentos inválidos devem ser desconsiderados sem provocar a exibição de erros ou exceções.

# Código comentado:

import java.util.Scanner;

public class atv01 {
    public static void main(String[] args) {
        // cria um objeto Scanner para ler a entrada do usuário a partir do console
        Scanner scanner = new Scanner(System.in);
        
        // pede ao usuário para digitar os números separados por espaço
        System.out.print("Digite os números separados por espaço: ");
        
        // lê a entrada do usuário como uma string
        String input = scanner.nextLine();
        
        // divide a string em um array de strings usando o espaço como separador
        String[] valores = input.split(" ");
        
        // inicializa a variável "soma" com o valor zero
        double soma = 0;
        
        // itera sobre cada valor do array "valores"
        for (String valor : valores) {
            // verifica se o valor atual não é nulo e não está vazio após remover os espaços em branco da string
            if (valor != null && !valor.trim().isEmpty()) {
                try {
                    // tenta converter o valor atual para um número em ponto flutuante (double) e adicioná-lo à variável "soma"
                    soma += Double.parseDouble(valor);
                } catch (NumberFormatException e) {
                    // ignora o valor inválido
                }
            }
        }
        
        // imprime a soma dos números lidos do usuário
        System.out.println("A soma dos números informados é: " + soma);
    }
}
