import java.util.Scanner;

public class ProvaUmUna {
    public static void main(String[] args) {

        // Entrada de dados do sitema
        Scanner scanner = new Scanner(System.in);

        System.out.println("Digite a placa do veículo:");
        String placaVeiculo = scanner.nextLine();

        System.out.println("Digite o valor do combustivel:");
        double valorCombustivel = scanner.nextDouble();

        System.out.println("Digite a quantidade de quilômetros rodados a 60 KM/H");
        double kmh60 = scanner.nextDouble();

        System.out.println("Digite a quantidade de quilômetros rodados a 80 KM/H");
        double kmh80 = scanner.nextDouble();

        System.out.println("Digite a quantidade de quilômetros rodados a 100 KM/H");
        double kmh100 = scanner.nextDouble();

        System.out.println("Digite a quantidade de quilômetros rodados a 120 KM/H");
        double kmh120 = scanner.nextDouble();

        System.out.println("Digite a quantidade de quilômetros rodados a 140 KM/H");
        double kmh140 = scanner.nextDouble();

        // Cálculo da quantidade utilizada de combustível para cada trecho
        double litros60 = (10.0 / 307) * kmh60;
        double litros80 = (10.0 / 268) * kmh80;
        double litros100 = (10.0 / 224) * kmh100;
        double litros120 = (10.0 / 181) * kmh120;
        double litros140 = (10.0 / 145) * kmh140;

        // Cálculo da quantidade total de combustível
        double totaldelitros = litros60 + litros80 + litros100 + litros120 + litros140;

        // Cálculo da velocidade média ponderada da viagem
        double tempo60 = kmh60 / 60, tempo80 = kmh80 / 80,
                tempo100 = kmh100 / 100, tempo120 = kmh120 / 120,
                tempo140 = kmh140 / 140;

        double velocidadeMediaPonderada = ((60 * tempo60) + (80 * tempo80) + (100 * tempo100) + (120 * tempo120)
                + (140 * tempo140)) / (tempo60 + tempo80 + tempo100 + tempo120 + tempo140);

        // Cálculo do custo total da viagem
        double custoTotalViagem = ((kmh60 / 30.7) + (kmh80 / 26.8) + (kmh100 / 22.4) + (kmh120 / 18.1)
                + (kmh140 / 14.5)) * valorCombustivel;

        // O custo total da viagem.
        System.out.println("Placa do veículo: " + placaVeiculo);
        System.out.println(String.format("Consumo total: %.4f litros", totaldelitros));
        System.out.println(String.format("Valor total: R$%.2f", custoTotalViagem));
        System.out.println(String.format("Velocidade média ponderada: %.4fkm/h", velocidadeMediaPonderada));
        scanner.close();
    }
}
