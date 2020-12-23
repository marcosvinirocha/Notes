```java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.List;
import java.util.StringTokenizer;
import java.util.stream.Collectors;

public class CoracaoDasCartas {
    public static void main(String[] args) throws IOException {
        //1 / 5 - Coração das cartas
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StringTokenizer st = new StringTokenizer(br.readLine()); // Lê a linha de entrada
        Integer a= Integer.parseInt(st.nextToken());
        List<String> list= new ArrayList<>();
        List<Integer> list1,listaResultado = new ArrayList<>();
        List<List<Integer>> valoresPilha=new ArrayList<>();

        //Captura os dados e coloca na lista

        while(a!=0){
            for (var i = 1; i <= a; i++) {
                list.addAll(Arrays.stream(br.readLine().trim().split(" "))
                        .collect(Collectors.toCollection(ArrayList::new)));
                list1=list.stream().map(elem->Integer.parseInt(elem)).collect(Collectors.toList());
                valoresPilha.add(list1);
                list=new ArrayList<>();
                list1=new ArrayList<>();
            }

            boolean valor=valoresPilha.stream().allMatch(elem->elem.stream()
                    .reduce(0,(acc,val)->acc+val)%3==0);
            listaResultado.add(valor==true?1:0);
            a= Integer.parseInt(br.readLine());
        }
        listaResultado.stream().forEach(System.out::println);


    }


}
```

