# Segunda-Feira

## Fala galera, aqui centralizaremos as atividades trabalhadas nas suas segundas, exercícios e demais arquivos que são perntinente as assuntos trabalhados.

### Operadores artméticos

```
Operador	Significado
+		adição
-		subtração
*		multiplicação
/		divisão
%		mod (resto da divisão)
```

Precedência
```
1 → * / %
2 → + -
```
#### Exemplos
```
2 * 6 / 3 = 4
3 + 2 * 4 = 11
(3 + 2) * 4 = 20
60 / (3+2) * 4 = 48
60 * ((3.067 + 1.2) / 2) 

6 % 2 = 0
6 % 4 = 2
19 % 5 = 4
14 % 3 = 2
```
### Nome de variáveis
```
int 3 séries de 10 repetições;
int _3 séries de 10 repetições;
int _3 series de 10 repeticoes;
int _3seriesdenaoentendinada10repeticoes;
int  SeriesDeNaoEntendiNadaComAlgumasRepeticoesSemNumeroNaFrente;
double melhorAindaEhSemNumeroNaFrente;
boolean mas_tem_gente_que_prefere_snake_case;
String everInEnglishPlease = ‘If seu English not is much good, só try!’
```
### Declaração de variáveis
```
<tipo> <nomeDaVariavel> = <valor inicial>;
char intEhONumeroDaVida = ‘42’;
double sempreEstejaComSuasToalhas = 3.1415
```

### Tipos primitivos
```
Números inteiros: byte, short, int, long
Números com ponto flutuante: float, double
Valor verdade: boolean
Um caractere Unicode: char

Cadeia de caracteres: String (não é primitivo)

Exemplo: 'a' = '\u0061'
```
### Operações básicas de programação
```
Entrada de dados: teclado (mouse só em .net)
É feita através de adição de valores as variáveis.

Processamento de dados: Processador
É quando o programa realiza os cálculos.

Saída de dados: Monitor
É quando o programa mostra os dados tratados.
```

### Saída de Dados

#### Escrever na tela
```
Sem quebra de linha ao final:
System.out.print(“Não pula linha!”);

Com quebra de linha ao final:
System.out.println(“Se seu primeiro código não foi: “);
System.out.println(“System.out.print(“Hello World! ”);”
System.out.print(“Você está amaldiçõado… Boa sorte!”);

Com variável:
System.out.print(r);

Com controle de casas decimais:
System.out.print(“%.2f”, x);

Para considerar o separador de decimais como ponto (como é no USA), ANTES da declaração do Scanner set a localidade para US.

Locale.setDefault(Locale.US);

Concatenar elementos:
System.out.print(s + “ séries de “ + r + “ repetições!”);
ou
System.out.print(“%n tigres tristes comem %n pratos de trigo”, numTigers, numDishs);
System.out.print(“it’s-a me, %s! Woo-hoo! Let’s-a go play N%d”, mariosName, nintendo64);

%f = ponto flutuante
%d = inteiro
%s = texto
%n = quebra de linha
```

#### Calculando
```
A variável sempre receberá a expressão.
<variavel> = <expressao>

int r, m;

r = 21;
m = 9 + r;

double force, mass, aceleration;

mass = 4.0;
aceleration = 2250.0

force = mass * aceleration;

System.out.println(“It’s over %.2f!”);

caso use float é uma boa pratica usar f.

float forca, massa, aceleracao;

massa = 4f;
aceleracao = 2000f;

forca = massa * aceleracao;

System.out.println(“É de mais de %f!”);
```

### Casting
```
É a conversão explícita de um tipo para outro.
Utilizado para converter o resultado de um tipo para outro.

int goku = 1, vejita = 1;
double gojita = 0.0;

gojita = (double) goku + vejita;
```

### Entrada de Dados
```
Para fazer entrada de dados, é preciso criar um objeto do tipo “Scanner”.

Scanner sc = new Scanner(System.in);

Para ler texto (sem espaços)

String word = sc.next();

Para ler inteiro

int x = sc.nextInt();

Para ler double

double y = sc.nextDouble();

Para ler um caractere

char c = sc.next().charAt(0);

Funções extras para String

Formatar: toLowerCase(), toUpperCase(), trim()
Recortar: substring(inicio), substring(inicio, fim)
Substituir: replace(char, char), replace(string, string)
Buscar: indexOf(), lastIndexOf()
```

### Função Matemática
```
Raiz quadrada
r = Math.sqrt(x);

Exponencial
r = Math.pow(x, y);

Valor Absoluto
r = Math.abs(x);

Modo de uso
double delta, a, b, c, x1, x2;

delta = Math.pow(b, 2.0) – 4*a*c;
x1 = (-b + Math.sqrt(delta)) / (2.0 * a);
x2 = (-b – Math.sqrt(delta)) / (2.0 * a);
```

### Expressões comparativas

### Operadores comparativos
```
Operador	Significado
>			maior
<			menor
>=			meior ou igual
<=			menor ou igual
==			igual
!=			diferente

Supondo que x = 7
x > 0  Resultado: True
x == 3 Resultado: False
10 <= 30 Resultado: True
x != 2 Resultado: True
7 >= x Resultado: True
```

### Operadores lógicos
```
Operador	Significado
&&			E
||			OU
!			NÃO
```
#### Exemplos do operador “E” → Todas as condições verdadeiras
```
LoL é melhor que Dota E CS é melhor que Calófiduti Resultado: True

iPhone é melhor que Android E GeForce é melhor que AMD Resultado: false

x > 0 && x == 7 Resultado: True

x < 8 && x <= 6 && x > 5 Resultado: false
```

#### Exemplos do operador “OU” → Pelo menos uma das condições verdadeiras
```
Supra mk4 é melhor que Skyline GT-R R34 OU One Piece é melhor que Naruto Resultado: True

x > 0 || x == 7 Resultado: True

x > 8 || x != 7 || x >= 3 Resultado: True
```

#### Exemplo Misto → Precedência vem primeiro E depois OU
```
x > 6 || x != 7 && x >= 8 Resultado: True
```

#### Exemplo de Não → Nega
```
!(x > 6 || x != 7 && x > 8) Resultado: False
```

### Estrutura condicional → Controle dependente de condição

#### Estrutura condiciona simples
```
Se ( expressão verdade ) {
	Bloco de código caso seja verdade
} 
```
#### Estrutura condiciona composta
```
Se ( expressão verdade ) {
	Bloco de código caso seja verdade
} ou então {
	Bloco de código caso seja falso
}
```

#### Estrutura condiciona encadeada
```
Se ( expressão verdade ) {
	Bloco de código caso seja verdade
} ou então {
	se (expressão verdade) {
		Bloco de código caso seja verdade a segunda expressão
	} ou então {
		Bloco de código caso seja falso a primeira e a segunda expressão
	}
}

if (x != 7) {
	System.out.print(“X diferente de 7”);
} else if (x <= 6) {
		System.out.print(“X menor que 7”);
	} else if (x >= 8) {
			System.out.print(“X maior que 7”);	
		} else {
			System.out.print(“X igual a 7”);
		}
}
```

### Operadores de atribuição cumulativa
```
Operador	Equivalência
a += b;		a = a + b;
a -= b;		a = a – b;
a *= b;		a = a * b;
a /= b;		a = a / b;
a %= b;		a = a % b;
```
### Estrutura opcional → Controle dependente de uma dentre várias opções
```
switch (x) {
	case 1: //valor de x igual 1
		System.out.print(“x vale 1”);
		break;
	case 2: //valor de x igual 2
		System.out.print(“x vale 2”);
		break;
	case 2: //valor de x igual 2
		System.out.print(“x vale 2”);
		break;
	case 3: //valor de x igual 3
		System.out.print(“x vale 3”);
		break;
	case 4: //valor de x igual 4
		System.out.print(“x vale 4”);
		break;
	default:
		System.out.print(“x tem outro valor”);
		break;
}
```
### Expressão condincional ternária → Um opcional ao if-else
```
( expressão ) ? seVerdadeiro : seFalso

( Digimon melhor que Pokemon) ? 1 : 2

( x != 7 ) ? “Agumon” : “Pikachu”
```

### Estrutura de repetição

#### Estrutura while (enquanto) → Serve para repetir um bloco de comandos enquanto a condição for verdadeira
```
x = 4;
while ( x != 7 ) {
	++x;
}
```
#### Estrutura for (para) → Serve para repetir um bloco de comands por um certo intervalo de tempo
```
for ( início ; condição ; incremento) {
	bloco de códigos
}

for ( int i=0; i<5; i++) {
	System.out.println(“Valor de I: “ + I);
}

Regressivo
for ( int i=4; i>=0; i--) {
	System.out.println(“Valor de I: “ + I);
}
```
#### Estrutura do while (faça enquanto) → Executa no mínimo uma vez.
```
do {
	Bloco de código
} while ( condição );

int x = 4;
do {
	System.out.println(“Valor de X: “ + x);
	++x;
} while ( x <= 7 )
```

### Retirado do curso do Professor Nelio Alves
[Curso da Udemy](https://www.udemy.com/course/java-curso-completo/)<br />
[GitHub do Professor](https://github.com/acenelio)

### Tip of the day

> Para percorrer uma lista no java e fazer uma operação com cada elemento da lista, temos uma estrutura pronta: **ForEach**

#### Exemplo para somar 1 e imprimir cada elemento de uma lista de inteiros:

`for(int numero: numeros){   
     numero = numero + 1;    
     System.out.println(numero);    
 }`
