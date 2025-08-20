---
aliases:
  - Klassen
---
# Klasse
Eine Klasse in Java ist eine Art Schablone für [[Objekt|Objekte]].
Dabei ist jedes [[Objekt]], das von dieser Klasse erstellt wird, zunächst gleich, bis auf die UUID und spezifisch bei der Objekterstellung angegebene Parameter.

## Aufbau
Eine Klasse ist folgendermaßen aufgebaut: 
1. Import-Anweisungen
2. Klassendefinition
3. Attribute (Exemplarvariablen)
4. [[Konstruktor]]
5. [[Methode|Methoden]]

>[!Example]
>Eine einfache Beispielklasse könnte folgendermaßen aussehen:
>```
>import java.util.Random; // Beispiel-Import
>
>public class Auto {
>
>	// Attribut
>	private String marke;
>	
>	// Konstruktor
>	public Auto(String marke) {
>		this.marke = marke;
>	}
>	
>	// Eine einzige Methode
>	public void hupen() {
>	    System.out.println(marke + " hupt!");
>	   }
>}
>```



