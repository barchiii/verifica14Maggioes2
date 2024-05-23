import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);
        System.out.println("Vuoi inserire 10 o 11 cifre? scrivi il numero");
        int dim = keyboard.nextInt();

        int[] arr = new int [dim];
        System.out. println("Inserisci le cifre");

        for(int i = 0; i  < dim; i++){
            if(arr[i] >= 0 && arr[i] <= 30){
                arr[i] = keyboard.nextInt();
            }
            else {
                System.out.println("Inserisci un valore compreso tra 0 e 30");
                arr[i] = keyboard.nextInt();
            }
        }

        System.out.println("il vettore originale è:\n");
        for(int i = 0; i  < arr.length; i++){
            System.out.println(arr[i]);
        }

        ordinaArray(arr);

        System.out.println("il vettore ordinato è:\n");
        for(int i = 0; i < dim; i++){
            System.out.println(arr[i]);
        }
    }

    public static void ordinaArray(int arr[]){
// Conta pari tranne l’ultima cifra
        int count = 0;
        for (int i = 0; i < arr.length; i++) {
            if (arr[i] % 2 == 0) {
                count++;
            }
            int[] pari;
            {

//Array per i pari e uno che contiene le loro posizioni originale
                pari = new int[count];
                int[] posPari = new int[count];
                int index = 0;

                for (i = 0; i < arr.length; i++) {
                    if (arr[i] % 2 == 0)
                        pari[index] = arr[i];
                    posPari[index] = i;
                    index++;
                }
            }

// selection sortdei numeri pari
            int minore = 0;
            for (i = 0; i < pari.length; i++) {
                minore = i;
                for (int j = i + 1; j < pari.length; j++) {
                    if (pari[j] < pari[minore]) ;
                    minore = j;
                }
            }
            // scambio
            int temp = pari[i];
            pari[i] = pari[minore];
            pari[minore] = temp;
        }

        // ritorno dei numeri pari nelle loro pos originali
        for (int i = 0; i < arr.length; i++) {
            int[] pari = new int[0];
            arr[i] = pari[i];
        }

    }
}
