package controle;

import dominio.VendaProduto;
import java.util.Scanner;
import java.text.DecimalFormat;

public class ControleVenda {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        DecimalFormat df = new DecimalFormat("#.00");

        // Array de 5 vendas
        VendaProduto[] vendas = new VendaProduto[5];

        // Entrada de dados
        for (int i = 0; i < vendas.length; i++) {
            System.out.println("\nCadastro da venda " + (i + 1) + ":");

            System.out.print("Digite o número da venda: ");
            int numero = sc.nextInt();

            System.out.print("Digite a quantidade de produtos: ");
            int quantidade = sc.nextInt();

            System.out.print("Digite o valor unitário do produto: ");
            double valorUnitario = sc.nextDouble();

            vendas[i] = new VendaProduto(numero, quantidade, valorUnitario);
        }

        // Saída de dados
        System.out.println("\n===== LISTA DE VENDAS =====");
        for (int i = 0; i < vendas.length; i++) {
            VendaProduto venda = vendas[i];
            System.out.println("Venda " + (i + 1) + ":");
            System.out.println("Número da venda: " + venda.getNumero());
            System.out.println("Quantidade de produtos: " + venda.getQuantidade());
            System.out.println("Valor unitário: R$ " + df.format(venda.getValorUnitario()));
            System.out.println("Valor total a pagar: R$ " + df.format(venda.valorPagar()));
            System.out.println("-----------------------------");
        }

        sc.close();
    }
}

