# TriBulles
package fr.gouv.finances.exo;

public class triBulles {

    public static void main(String[] args) {
	int[] monTab = { 22, 8, 6, 24, 2, 50, 7 };
	int i;
	int var;
	int j;

	for (i = 0; i < monTab.length - 1; i++) {

	    for (j = 0; j < monTab.length - 1; j++) {

		if (monTab[j] > monTab[j + 1]) {
		    var = monTab[j];
		    monTab[j] = monTab[j + 1];
		    monTab[j + 1] = var;
		}

	    }
	    for (int g : monTab) {
		System.out.print(g + " ");

	    }
	    System.out.println("");
	}
//	for (int g : monTab) {
//	    System.out.println(g);
//	}
    }
}
