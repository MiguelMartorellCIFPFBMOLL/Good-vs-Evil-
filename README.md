# Good-vs-Evil-
 Esta es mi solución a Good vs Evil 

 ```
 public class GoodVsEvil {
  public static String battle(String goodAmounts, String evilAmounts) {
    String [] buenos = goodAmounts.split(" ");
    String [] malos = evilAmounts.split(" ");
    int sumadorbuenos = 0;
    int sumadormalos = 0;
    for (int i = 0; i < buenos.length; i++){
      switch (i){
          case 0:
          sumadorbuenos += Integer.parseInt(buenos [i]);
          break;
          case 1:
          sumadorbuenos += Integer.parseInt(buenos [i]) * 2;
          break;
           case 2:
          sumadorbuenos += Integer.parseInt(buenos [i]) * 3;
          break;
          case 3:
          sumadorbuenos += Integer.parseInt(buenos [i]) * 3;
          break;
          case 4: 
          sumadorbuenos += Integer.parseInt(buenos [i]) * 4;
          break;
          case 5:
          sumadorbuenos += Integer.parseInt(buenos [i]) * 10;
          break;          
      }
    }
    for (int j = 0; j < malos.length; j++){ // Cambiar la condición aquí
       switch (j){
          case 0:
          sumadormalos += Integer.parseInt(malos [j]);
          break;
          case 1:
          sumadormalos += Integer.parseInt(malos [j]) * 2;
          break;
          case 2:
          sumadormalos += Integer.parseInt(malos [j]) * 2;
          break;
          case 3:
          sumadormalos += Integer.parseInt(malos [j]) * 2;
          break;
          case 4:
          sumadormalos += Integer.parseInt(malos [j]) * 3;
          break;
          case 5:
          sumadormalos += Integer.parseInt(malos [j]) * 5;
          break;
          case 6:
          sumadormalos += Integer.parseInt(malos [j]) * 10;
          break;
      }
    }
    if(sumadorbuenos > sumadormalos){
     return "Battle Result: Good triumphs over Evil";
    }
    else if(sumadorbuenos < sumadormalos){
      return "Battle Result: Evil eradicates all trace of Good";
    }else{
    return "Battle Result: No victor on this battle field";
      }
  }
} ```
