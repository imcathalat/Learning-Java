# Learning-Java

- sout: System.out.print ();
- psvm: public static void main (String[] args) {}

### Regas CamelCase

1. primeira letra maiuscula: **classe** ou **interface**;
2. primeira letra minuscula, outras letras em CamelCase: **atributo**, **variável** ou **método**;
   1. nomeAluno, mediaPrimeiroBimestre, lancarNota;
3. somente letras minúsculas: **pacote**;
4. somente letras maiúsculas: **constante**;

### Hello World!

``` 
package primeiroprograma;
public  class PrimeiroPrograma {
   public static void main (String[] args) {
        System.out.print("Hello World!");
        }
    }
```

- **import**: para importar classes.
por padrão vem com o pacote **java.lang**

### Algumas conversões

#### Integer.parseInt(); -> String para inteiro
#### Integer.toString(); -> Inteiro para String

get.Text e setText: necessário a conversão

- get: pegar a informação (receber o dado)
- set: mostra a informação na tela depois de compilada

## Calculator Code in actionPerformed:

```
      private void btnCalculatorActionPerformed (java.awt.event.ActionEvent evt) 
      {
         int ano = (Integer) spnAno.getValue(); 
         
         getValue(); = pegar o que foi escrito no spinner.
         typecast também é um conversor de tipos de variável

         /*** o usuário digita no spinner o ano que nasceu e a variável ano armazena esse valor (getValue();), não é necessária a conversão de string para inteiro, visto que spinner só recebe valores numéricos, além disso, e necessário o uso de typecast (n sei pq) ***/

         int idade = (int) (2023-ano);

         lblIdade.setText(Integer.toString(idade)); 
         /* A label chamada lblIdade exibe (set.Text) um valor inteiro que foi convertido para String (Integer.toString) que tinha sido armazenado na variável idade */ 
         } 
         
  ```
  
 ### ! Operadores Unários !   
 
 ### Pré-incremento ≠ Pós-incremento
- Pré incremento: 

```
         int numero = 5;
         int valor = 5 + ++numero; 
         significa que 5 vai ser somado ao número que foi somado mais um antes de realizar a soma 5 + numero.
 ```
 - Pós incremento:
 ```
         int numero = 5;
         int valor = 5 + numero++;
         significa que 5 vai ser somado a numero (5) e depois dessa soma, numero vai receber um. Ou seja, realiza a soma de 5 + numero e depois a variável numero muda de 5              para 6, pois recebeu mais 1.
 ```
 - O pré e o pós decremento funcionam da mesma forma, porém ao invés de adicionando uma unidade, se subtrai uma unidade.
 
 ### Operadores de Atribuição 
 - símbolo primeiro e depois o sinal de atribuição (=) -> -= ou /= ou *= e assim por diante.
 ```
   a+=b -> a = a + b;
   a-=b -> a = a -b;
   a*=b -> a = a * b;
   a/=b -> a = a/b;
   a%=b -> a =a % b;
   
 ```
 
 ## Classe Math

![math-java-2](https://user-images.githubusercontent.com/82779734/234941866-f5875462-0ea6-42a7-b649-ccb31fe01594.png)

### Arredondamentos

![arredondamentos-classe-math](https://user-images.githubusercontent.com/82779734/234943655-0deb9cf0-bdfb-4e79-81d1-f4ffe9a13075.png)

### Gerador de Número

**Math.random();** : gera número entra 0 e 1.

**Gerar número aléatório entre uma faixa de números que eu escolhi**
```
   menor numero + Math.random() * (maior numero - menor numero)
   
   double ale = Math.random();
   int ale2 = (int) 5 + ale*(10-5);
   vai gerar um número aleatório entre 5 e 10
```


   
