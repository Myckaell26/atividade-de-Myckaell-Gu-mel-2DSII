# atividade-de-Myckaell-Gu-mel-2DSII
import java.util.Scanner;

public class CalculadoraIMC {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        // Entrada de dados
        System.out.print("Digite seu peso (kg): ");
        double peso = scanner.nextDouble();

        System.out.print("Digite sua altura (m): ");
        double altura = scanner.nextDouble();

        // Cálculo do IMC
        double imc = peso / (altura * altura);

        // Exibição do resultado
        System.out.printf("Seu IMC é: %.2f%n", imc);

        // Classificação
        if (imc < 18.5) {
            System.out.println("Classificação: Abaixo do peso");
        } else if (imc < 25) {
            System.out.println("Classificação: Peso normal");
        } else if (imc < 30) {
            System.out.println("Classificação: Sobrepeso");
        } else if (imc < 35) {
            System.out.println("Classificação: Obesidade grau 1");
        } else if (imc < 40) {
            System.out.println("Classificação: Obesidade grau 2");
        } else {
            System.out.println("Classificação: Obesidade grau 3");
        }

        scanner.close();
    }
}
