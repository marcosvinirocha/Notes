***ArraysList***

documentação

https://www.javatpoint.com/collections-in-java

```java
List<String> nomes = new ArrayList<>();
//ou
List<String> nomes = new Vector<>();

nomes.add("carlos");// adiciona o nome

System.out.println(nome);

Collections.short(nomes); // ordena na ordem desejada
System.out.println(nome);

nomes.set(2,"larissa")// realiza um update na lista  

nomes.remove(4,"maria"); //remove da lista 
nomes.remove("marcos");

String nome = nomes.get(1); // retorna o valor para a variavel
int tamanho = nomes.size(); // retorna a quantidade de elementos na lista

nomes.contains("marieta") // verifica se possui o elemento na lista retornando um valor 								boleano.

nome.isEmpty(); // retorna um valor boleano se a lista tiver vazia ou não;
nome.clear(); // limpa a lista;

int posicao = nomes.indexOf(""); //retorna um inteiro com a posicao da lista

// declara uma variavel que não esta usando mais a variavel que deseja usar
for(String nomedalinha: nomes){ 
    
    // imprimir a lista
}

 Iterator<Carro> carrosAsIterator = carros.iterator();
         while (carrosAsIterator.hasNext()){
                Carro it = carrosAsIterator.next();
/*A idéia do Iterator é realmente percorrer uma coleção, porém vc pode utilizar Iterators diferentes para percorrer uma coleção de forma diferente…se vc usar um Iterator ao invés de implementar na própria lista o código pra percorrê-la como vc quer, vc evita carregar a interface da lista com coisas que não pertencem a ela…
*/
             
  
 Set<Double> notaslunos = new Hashset<>();
  // segue o mesmo exemplo de cima de lista
 LinkedHashSet<Integer> sequencia de numeros = new LinkedHashSet<>();
  // segue o mesmo exemplo de cima de lista
 TreeSet<String> treeCapitais = new TreeSet<>();
    // segue o mesmo exemplo de cima de lista
             
             
  
             
```



***Queue***

https://www.javatpoint.com/java-priorityqueue

```java
Queue<String> filaDeBanco = new linkedList<>();
filaDeBanco.add("");

String cliente1 = filaDeBanco.poll(); // exibe o valor e remove da fila

String cliente2 = filaDeBanco.peek(); // exibe o valor mas não remove da fila e retorna null se estiver vazia.

String cleinte3 = filaDeBanco.element(); // execulta o mesmo processo do peek, mas se a lista tiver vazia podera ocorrer erro.





```



***Map***

https://www.javatpoint.com/java-map

```java
import java.util.*;  
public class HashMapExample1{  
 public static void main(String args[]){  
   HashMap<Integer,String> map=new HashMap<Integer,String>();//Creating HashMap    
   map.put(1,"Mango");  //Put elements in Map  
   map.put(2,"Apple");    
   map.put(3,"Banana");   
   map.put(4,"Grapes");   
       
   System.out.println("Iterating Hashmap...");  
   for(Map.Entry m : map.entrySet()){    
    System.out.println(m.getKey()+" "+m.getValue());    
   }  
}  
}  
```



***Comparators***

1. usados para ordenação de listas

https://www.javatpoint.com/Comparable-interface-in-collection-framework

https://www.javatpoint.com/Comparator-interface-in-collection-framework



***Options***

https://www.javatpoint.com/java-8-optional



***Stream API***

https://www.javatpoint.com/java-8-stream