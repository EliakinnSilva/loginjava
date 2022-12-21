# loginjava
Estudo de java

import java.util.Scanner;

public class Login {
  public static void main(String[] args) {
    // Define as variáveis de nome de usuário, senha e resultado
    String username = "";
    String password = "";
    String result = "";

    // Cria um objeto Scanner para ler a entrada do usuário
    Scanner input = new Scanner(System.in);

    // Lê o nome de usuário e a senha do usuário
    System.out.print("Insira o nome de usuário: ");
    username = input.nextLine();
    System.out.print("Insira a senha: ");
    password = input.nextLine();

    // Verifica se o nome de usuário e a senha são válidos
    if (username.equals("silva") && password.equals("1234")) {
      result = "login bem-sucedido";
      System.out.println("Bem-vindo, " + username + "!");
    } else {
      result = "login falhou";
      System.out.println("Nome de usuário ou senha incorretos. Tente novamente.");
    }
  }
}
