# TesteProva


public class Calculadora {
	private int resultado = 0;

	public int somar(int nr1, int nr2) {
		resultado = nr1 + nr2;
		return resultado;
	}

	public int subtrair(int nr1, int nr2) {
		resultado = nr1 - nr2;
		return resultado;
	}

	public int multiplicar(int nr1, int nr2) {
		resultado = nr1 * nr2;
		return resultado;
	}

	public int dividir(int nr1, int nr2) {
		resultado = nr1 / nr2;
		return resultado;
	}
}

