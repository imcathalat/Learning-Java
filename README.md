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

´´´

      private void btnCalculatorActionPerformed (java.awt.event.ActionEvent evt) 
      {
         int ano = (Integer) spnAno.getValue(); 

         /*** o usuário digita no spinner o ano que nasceu e a variável ano armazena esse valor (getValue();), não é necessária a conversão de string para inteiro, visto que spinner só recebe valores numéricos, além disso, e necessário o uso de typecast (n sei pq) ***/

         int idade = (int) (2023-ano);

         lblIdade.setText(Integer.toString(idade)); 
         /* A label chamada lblIdade exibe (set.Text) um valor inteiro que foi convertido para String (Integer.toString) que tinha sido armazenado na variável idade */
   }
´´´
