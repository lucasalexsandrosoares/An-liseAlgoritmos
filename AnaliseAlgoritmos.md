# AnáliseAlgoritmos

#### 1 Problema
Quais são as duas caracterısticas mais comuns para analisar algoritmos? 

R: Tempo e consumo de memória.

#### 2 Problema 
Por que a medida de tempo em segundos não representa qualificadamente o tempo de execução de um algoritmo? 

R: A medição de tempo em segundos não é uma medida estável e de qualidade.

#### 3 Problema 
A medida de tempo de um algoritmo é realizada através de qual informação? O que pode afetá-la? 

R: A medição de tempo é feita através da quantidade de passos que o algoritmo precisa finalizar a execução. O tempo de execução de um algoritmo é afetado pelo ambiente do hardware (compilador, processador, Sistema operacional da linguagem de programação, etc) e tamanho de entrada.

#### 4 Problema 
Na análise de algoritmos, qual é o valor da base da função logarıtmica e exponencial? Por que é escolhido este valor?

R: Base 2, por causa das operações binárias.

#### 5 Problema 
O que é complexidade de tempo? 

R: É o tempo que o algoritmo leva para executar a função.

#### 6 Problema 
Dado dois algoritmos A e B com as complexidades de tempo respectivamente f1 e f2, qual é o melhor algoritmo? O que indica qual é o melhor algoritmo?

R: O tempo de execução e o número de iterações. 

#### 7 Problema 
Em uma função de complexidade, o que representa o termo n? 

R: Tamanho  da entrada. 

#### 8 Problema 
Quais são as operações primitivas de um algoritmo?

R: 
Atribuição de valores a variáveis 
Chamadas de métodos 
Operações aritméticas (por exemplo, adição de dois números) 
Comparação de dois números 
Acesso a um arranjo 
Seguimento de uma referência para um objeto 
Retorno de um método
 
#### 9 Problema 
Qual é o valor de uma operação primitiva de um algoritmo? 

R: Se atribui o valor 1.

#### 10 Problema 
Desenvolva o pseudocódigo do algoritmo SOMA, que realiza a soma de dois números inteiros recebidos por parâmetro e tem como saída a resultado da operação. Identifique a sua função de complexidade de tempo. 

```python
funcao soma (a, b){
	s = a + b
retorna s 
}
``` 

f(n) = 2


#### 11 Problema 
Desenvolva o pseudocódigo do algoritmo SOMA VETOR, que realiza a soma de todos os elementos de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo. 

```
funcao somavetor(v){
para i em alcance(v){
s += v[i]	
}
retorna s
} 
```

f(n) = n + n + 1

f(n) =  2n + 1

#### 12 Problema 
Desenvolva o pseudocódigo do algoritmo CONTAGEM ÍMPARES, que realiza a contagem de números ímpares de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo. 

```
funcao contaimpares(v){
para i em alcance(v){
se v[i] % 2  == 0{
 c += 1
}
	}
retorna c
}
```
f(n) =  n + n + n + 1

f(n) =  3n + 1

#### 13 Problema 
Desenvolva o pseudocódigo do algoritmo SOMA MATRIZ, que realiza a soma de todos os elementos de uma matriz. O algoritmo recebe a matriz M e tem como saída o resultado. Identifique a sua função de complexidade de tempo. 

```
funcao somamatriz(v){
	para i em alcance(v){
		para j em alcance(i) {
			s += v[i][j]
			j += 1		
		}
	i += 1
	}	
retorna s
}
```
f(n) =  n + n*n + n*n + n*n + n + 1

f(n) =  3n² + 2n + 1


#### 14 Problema 
Desenvolva o pseudocódigo do algoritmo BUSCA MATRIZ, que identifica posição x e y de um elemento em uma matriz. O algoritmo recebe a matriz M e o valor V e tem como saída a posição x e y . Identifique a sua função de complexidade de tempo. 

```
funcao buscamatriz (m,v){
para i = 1 até comprimento(m){
	para j = 1 até comprimento(v){
		se m[i][j] = v{
			retorna m[i][j]
		}
	j += 1
	}
i += 1
}
retorna m
}
```
f(n) = n + n*n + n*n+ n*n +n + 1 + 1

f(n) = 3n² + 2n + 2

#### 15 Problema 
O que é análise assintótica? Qual é o seu objetivo? 

R: É uma estimativa de tempo que o algoritmo leva para calcular. Objetivo de compreender o tempo de execução para grandes entradas.

#### 16 Problema 
Qual é o processo da análise assintótica? Crie um exemplo. 

R: f(n) = 4n4 + 2n2 + 10n + 5 -> Identificar o componente de maior ordem 4n4  -> Ignorar os coeficiente -> n4

#### 17 Problema 
O que é a notação assintótica? 

R:  É uma notação para descrever uma fórmula matemática que se importa apenas com o maior componente da fórmula e ignora os fatores menores ou constantes.

#### 18 Problema 
O que é a notação O-Grande ou Big-Oh?

R: Uma função é menor que ou igual a outra função g(n). F é limitada superiormente por g assintoticamente

#### 19 Problema 
Qual é a definição formal da notação  O-Grande? 

R: Sejam f e g funções f,g: N → R+. Digamos que f(n) = O(g(n)) se existem inteiros positivos c e n0 tais que para todo inteiro n ≥ n0 f(n) ≤ cg(n). Quando f(n) = O(g(n)) dizemos que g(n) é o limite superior para f(n) ou, mais precisamente, que g(n) é um limitante assintótico para f(n), para enfatizar que estamos suprimento fatores constantes.

#### 20 Problema 
Crie um gráfico explicando a notação O-grande. Utilize f(n) = 2n + 4. Qual é um valor possível para n0? 

n0 = 1 

constante = 6

![O-grande](https://user-images.githubusercontent.com/40281699/56991682-a3c9d980-6b6e-11e9-8672-6e290ec6f30e.PNG)

#### 21 Problema 
O que é a notação o-pequeno ou Little-Oh? 

R: Uma é função é menor que a outra função g(n). F é denominado de g assintoticamente.

#### 22 Problema 
Qual é a definição formal da notação  o-pequeno? 

R: Sejam f e g funções f,g: N → R+. Digamos que f(n) = o(g(n)) se Em outras palavras, f(n) = O(g(n)) significa que, para qualquer número real c > 0, existe um número n0, onde f(n) < cg(n) para todo n ≥ n0.

#### 23 Problema 
Crie um gráfico explicando a notação o-pequeno. 

![O-pequeno](https://user-images.githubusercontent.com/40281699/56991557-56e60300-6b6e-11e9-82d5-7701d8e1a29b.PNG)


#### 24 Problema 
Passe a notação O-grande e o-pequeno as funções abaixo: 

#### A F(n) = n + 1 

O (n)

o(n logn)

#### B F(n) = 8 

O (1)

o (1)

#### C F(n) = 2n 2 − 1 

O(n2)

o(2^n)

#### D F(n) = nlogn

O (nlogn)

o(n^2)

#### E F(n) = 3n! + 2n

O (n!)

o(n.n!) 

#### F F(n) = 3n 3 + 2n 2 + 4n + 6 

O (n3)

o(n!)

#### G F(n) = 5^n + 11 

O (n)

o (n logn)

#### H F(n) = 3logn 

O (n)

o(n)

#### 25 Problema 
Identifique o O-Grande dos algoritmos desenvolvidos nos Problemas 10 até 14.

#### 10) f(n) = 2  

O(1)

#### 11) f(n) =  2n + 1 

O(n)

#### 12) f(n) =  3n + 1 

O(n)

#### 13)f(n) =  3n² + 2n + 1 

O(n2)

#### 14) f(n) = 3n² + 2n + 2 

O(n2)
