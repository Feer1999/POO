
<h1 align="center"> Atividade 3 </h1>

Usando a classe JOptionPane para entrada de dados, crie uma classe que receba a nota de
duas provas e de um trabalho. Calcule e mostre a média.

# Código comentado:

Comentários adicionados no código:

```
import javax.swing.JOptionPane;

public class atv03 {
    public static void main(String[] args) {
        // Solicita a nota da primeira prova
        String nota1 = JOptionPane.showInputDialog("Digite a nota da primeira prova:");
        double prova1 = Double.parseDouble(nota1); // converte a nota em string para double

        // Solicita a nota da segunda prova
        String nota2 = JOptionPane.showInputDialog("Digite a nota da segunda prova:");
        double prova2 = Double.parseDouble(nota2); // converte a nota em string para double

        // Solicita a nota do trabalho
        String notaTrabalho = JOptionPane.showInputDialog("Digite a nota do trabalho:");
        double trabalho = Double.parseDouble(notaTrabalho); // converte a nota em string para double

        // Calcula a média das notas
        double media = (prova1 + prova2 + trabalho) / 3; // realiza o cálculo da média

        // Exibe a média em uma caixa de diálogo
        JOptionPane.showMessageDialog(null, "A média das notas é: " + media); // exibe o resultado em uma caixa de diálogo
    }
}

