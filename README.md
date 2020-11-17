# Nauka
public class Zad33 {

    /* 1. Napisz program, który:
● utworzy dwuwymiarowa 10 x 10 tablice liczb całkowitych,
● wypełni ja tabliczka mnożenia,
● wypisze elementy na ekran (wypisany ma być ładny
kwadrat). */

    public static void main(String[] args) {

        int [][] tabMnozenia = new int[10][10];

        for (int i = 0; i < tabMnozenia.length; i++) {
            for (int j = 0; j < tabMnozenia.length; j++) {

                tabMnozenia[0][j] = j + 1;
                tabMnozenia[i][0] = i + 1;
                tabMnozenia[i][j] = tabMnozenia[0][j] * tabMnozenia[i][0];

                System.out.printf("%3s", tabMnozenia[i][j] + " ");
            }
            System.out.println();
        }
    }
}
