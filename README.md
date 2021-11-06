<h2 align="center">Java function created by me to capitalize each first letter of a String </h2>

>Status: Completed ✔️

>Language used: Java 🖥️

#### Used normally in projects that need to read a name of user and return or store this name in back-end or front-end code

To make this simple function, I basically created a vector of each word in the String, then read the size of this vector and based on that I did a loop loop that replaces each first letter of each vector with an equivalent but in capital format. Finally, the function returns to us the correctly formatted String.

Full code (as i am from Brazil, the code variables are in portuguese):
~~~java
public class Capitalize {

	public static void main(String[] args) {
		String nome = "your name";
		System.out.println(letraMaiuscula(nome, ""));

	}

	public static String letraMaiuscula(String nome, String nomeCompleto) {
		nomeCompleto = "";
		String[] vetorNome = nome.split(" ");
		int tamVetor = vetorNome.length;

		for (int i = 0; i < tamVetor; i++) {
			String nomeSeparado = vetorNome[i];
			nome = nomeSeparado.substring(0, 1).toUpperCase().concat(nomeSeparado.substring(1));
			nomeCompleto += nome.concat(" ");
		}
		return (nomeCompleto);

	}

}
~
