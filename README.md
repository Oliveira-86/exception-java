# Excepction-java

- Uma exceção é qualquer condição de erro ou comportamento
inesperado encontrado por um programa em execução;
- Quando lançada, uma exceção é propagada na pilha de chamadas de
métodos em execução, até que seja capturada (tratada) ou o
programa seja encerrado;
- O modelo de tratamento de exceções permite que erros sejam
tratados de forma consistente e flexível, usando boas práticas.

### Estrutura try-catch

#### • Bloco try
	Contém o código que representa a execução normal do trecho de código que pode acarretar em uma exceção.
#### • Bloco catch
	Contém o código a ser executado caso uma exceção ocorra. Deve ser especificado o tipo da exceção a ser tratada (upcasting é permitido).
	
##### Exemplo:
	try {
      acc.withdraw(amount);
      System.out.println("New balance: " + String.format("%.2f", acc.getBalance()));
		}
    catch (DoimanException e) {
      System.out.println("Withdraw error: " + e.getMessage());
		}
		
