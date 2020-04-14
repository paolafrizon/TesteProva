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



# Classe do Junit



import org.junit.jupiter.api.Test;

import junit.framework.TestCase;

public class CalculadoraTest extends TestCase {
	@Test
	public void testeSomar() {
		int nro1 = 5;
		int nro2 = 5;
		Calculadora calc = new Calculadora();
		int resultadoEsperado = 10;
		int resultadoReal = calc.somar(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	}

	@Test
	public void testeSubtrair() {
		int nro1 = 5;
		int nro2 = 3;
		Calculadora calc = new Calculadora();
		int resultadoEsperado = 2;
		int resultadoReal = calc.subtrair(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	}

	@Test
	public void testeMultiplicar() {
		int nro1 = 3;
		int nro2 = 3;
		Calculadora calc = new Calculadora();
		int resultadoEsperado = 9;
		int resultadoReal = calc.multiplicar(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	}

	@Test
	public void testeDividir() {
		int nro1 = 10;
		int nro2 = 2;
		Calculadora calc = new Calculadora();
		int resultadoEsperado = 5;
		int resultadoReal = calc.dividir(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	}
}
