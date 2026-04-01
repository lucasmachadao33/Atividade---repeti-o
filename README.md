import java.util.Scanner;

public class TabuadaDeUmNumeroInteiro {
    public static void main(String[] args) {

        int numeroBase;
        char continuar;
        Scanner teclado = new Scanner(System.in);

        do {
            System.out.println("..: Tabuada de um número informado :..");
            System.out.print("Por favor, informe um número inteiro: ");
            numeroBase = teclado.nextInt();

            for (int i = 1; i < 11; i++) {
                System.out.printf("\n %3d x %2d = %3d",
                        numeroBase, i, (i * numeroBase));
            }

            System.out.print("\n\nDeseja continuar? (s/n): ");
            continuar = teclado.next().charAt(0);

        } while (continuar == 's' || continuar == 'S');

        System.out.println("\n..: Fim do programa :..");
    }
}
