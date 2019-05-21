# Kasa

import java.util.LinkedList;

public class Kasa {

	public static void main(String[] args) {
		
		Produkt chleb = new Produkt("chleb", 2.45, 1);
		Produkt mleko = new Produkt("mleko", 2, 2);
		Produkt maslo = new Produkt("maslo", 4.5, 1);
		
		Paragon paragon = new Paragon(new LinkedList<Produkt>());
		
		paragon.dodaj(maslo);
		paragon.dodaj(mleko);
		paragon.dodaj(chleb);
		
		paragon.drukuj();

		paragon.usun(0);
		
		paragon.drukuj();
	}

}
