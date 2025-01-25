package calculosalario;
import java.util.Scanner;

public class CalculoSalario {
  
      public static void main(String[] args) {
      Scanner sc = new Scanner(System.in);
        double salario = 0.0;
        double qtdhoras = 0.0;
        double qtdDias = 0.0;
        double calculo = 0.0;
        double opcao = 0.0;
       
      System.out.println("=======Calculo de salario========\n");
        
      System.out.println("======Digite a Opcao desejada========\n");
       
              /**coleta a escolha do usuario**/
        System.out.println("*****1.Calcular o valor do Salario Hora*******\n  \n******2.Calcular o Valor do salario dia*****\n");
           opcao = sc.nextDouble();
        
            /**se opcap igual a  1 **/
          if(opcao == 1 ){
         
              /**coleta o salario e o armazena na variavel "Salario"**/
              System.out.println("*****Digite o valor do salario*****\n");
              salario = sc.nextDouble();
                /**coleta a quantidade de horas trabalhadas e o armazena na variavel "qtdhoras"**/
              System.out.println("*****Digite a quanidades de horas trabalhadas*****\n");
              qtdhoras = sc.nextDouble();
              /**responsavel por realizar o calculo**/
              calculo = (salario / qtdhoras);
              System.out.println("*****o resultado da quantidade de dias trabalhados dividido pelo valor do salario e = "+calculo+ "*****\n");
          }
           if(opcao == 3 ){
         
              System.out.println("*****Digite o valor do salario*****\n");
              salario = sc.nextDouble();
              
              System.out.println("*****Digite a quanidades de Dias trabalhados*****\n");
              qtdDias = sc.nextDouble();
               
              calculo = (salario /qtdDias);
               
              System.out.println("*****o resultado da quantidade de dias trabalhados dividido pelo valor do salario e ="+calculo+ "*****\n");
          }
        
    }
    
}
