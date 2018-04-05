import javax.swing.*;
import java.util.Scanner;

/**public class aulaAtividades {
    public static void main(String[] args){
        //Escreva um algoritmo que calcule e imprima na tela a área de um triângulo, onde: Área = (Base x Altura) / 2.
        Double Base = Double.parseDouble(JOptionPane.showInputDialog("Digite a base referente ao triângulo: "));
        Double Altura = Double.parseDouble(JOptionPane.showInputDialog("Digite a altura referente ao triângulo: "));
        Double Area = (Base*Altura) / 2;
        Area.toString(JOptionPane.showConfirmDialog(null, Area));
        System.out.println("A área do triângulo referenciado é: "+Area);
    }
}*/

    /**public class aulaAtividades {
        public static void main(String[] args) {
            Double sexo = Double.parseDouble(JOptionPane.showInputDialog("Digite o seu sexo"));
            Double idade = Double.parseDouble(JOptionPane.showInputDialog("Digite a sua idade"));
            if ((sexo == 1) && (idade >= 21)){
                System.out.println("Sexo M e idade 21");
            } else{
                System.out.println("Deu errado");
            }
        }
    }*/
        //Algoritmo equação de segundo grau.
        /**public class aulaAtividades{
            public static void main(String[] args){
                Double coeficienteA = Double.parseDouble(JOptionPane.showInputDialog("Digite o primeiro coeficiente"));
                Double coeficienteB = Double.parseDouble(JOptionPane.showInputDialog("Digite o segundo coeficiente"));
                Double coeficienteC = Double.parseDouble(JOptionPane.showInputDialog("Digite o terceiro coeficiente"));
                Double DELTA = (coeficienteB*coeficienteB) - (4 * coeficienteA*coeficienteB);
                Double x1;
                Double x2;

                    if (DELTA > 0){
                        x1 = (-coeficienteB + Math.sqrt(DELTA) / (2 * coeficienteA));
                        System.out.println(x1);
                    } else if (DELTA == 0){
                        x1 = x2 = (-coeficienteB) / (2*coeficienteA);
                        System.out.println(x1);
                    } else{
                        System.out.println("Não existem raízes reais");
                    }
            }
        }*/

        //Menu com as opções de soma, subtração e multiplicação.
        /**public class aulaAtividades{
            public static void main(String[] args){
                Double numero1 = Double.parseDouble(JOptionPane.showInputDialog("Digite o primeiro número"));
                //numero1 = JOptionPane.showConfirmDialog(null,numero1);
                Double numero2 = Double.parseDouble(JOptionPane.showInputDialog("Digite o segundo número"));
                //numero2 = JOptionPane.showConfirmDialog(null, numero2);
                Double soma = (numero1+numero2);
                //soma.toString(JOptionPane.showConfirmDialog(null, soma));
                Double subtracao = (numero1-numero2);
                //subtracao.toString(JOptionPane.showConfirmDialog(null,subtracao));
                Double multiplicacao = (numero1*numero2);
                //multiplicacao.toString(JOptionPane.showConfirmDialog(null,multiplicacao));
                String operacaoDesejada = (JOptionPane.showInputDialog("Digite 1 para somar, 2 para subtrair ou 3 para multiplicar"));
                //operacaoDesejada.toString(JOptionPane.showConfirmDialog(null,operacaoDesejada));

                Byte NumerosRecebidos;
                switch (operacaoDesejada)
                {
                    case "1":
                        System.out.println ("A soma dos valores é: "+soma);
                        break;
                    case "2":
                        System.out.println("A subtração dos numeros recebidos é: "+subtracao);
                        break;
                    case "3":
                        System.out.println("A multiplicação dos numeros recebidos é: "+multiplicacao);
                }
            }
        }*/

        //Faça a fatoração do numero;        
        /**public class aulaAtividades{
            public static void main(String[] args){
               int fatorial = 1;
               int numeroRecebido = Integer.parseInt(JOptionPane.showInputDialog("Digite o número desejado para fatoração."));
               String resultado = "";

               if (numeroRecebido > 0){
                   while (numeroRecebido > 1){
                       fatorial = fatorial*numeroRecebido;
                       //System.out.println(fatorial);
                       resultado = resultado+numeroRecebido+ "x";
                       //System.out.println(resultado);
                       numeroRecebido = numeroRecebido - 1;
                       //System.out.println(numeroRecebido);
                   }
                   resultado = resultado+numeroRecebido;
                   JOptionPane.showMessageDialog(null,"Fatorial: "+resultado+"\nResultado: "+fatorial);
               } else if(numeroRecebido == 0){
                   JOptionPane.showMessageDialog(null,"Fatorial: "+numeroRecebido+"\nResultado: 1");
               } else{
                   JOptionPane.showMessageDialog(null,"Digite um número maior que 0");
               }
            }
        }*/
        
        //Escreva um algoritmo que calcule o valor de S, segundo a fórmula  S= 1/1...-10/100
        /**public class aulaAtividades{
            public static void main(String[] args){
            float valor = 1;
                float contador = 1;
                int indice = 1;
                String resultado = "";

                while (valor <= 10){
                    if (contador % 2 == 0){
                        valor += 1;
                        if(indice == 10) {
                            resultado += indice + "/" + indice * indice;
                        }
                        else {
                            resultado += indice + "/" + indice * indice + " + ";
                        }
                    } else{
                        valor += 1;
                        resultado += indice+"/"+indice*indice+" - ";
                    }
                    contador = contador + 1;
                    indice = indice + 1;
                }


                    JOptionPane.showMessageDialog(null, "Resultado: "+resultado);
                    System.out.println("Resultado: "+resultado);
            }
        }*/
        
        //Leia nomes e idades de uma quantidade indeterminada de pessoas;
        /*public class aulaAtividades{
            public static void main(String[] args){
              String  nomePessoa1; //= JOptionPane.showInputDialog("Digite o seu nome");
              int idadePessoa1; //= Integer.parseInt(JOptionPane.showInputDialog("Digite a sua idade");
              String nomePessoa2;
              int idadePessoa2;
              int indice = 1;

              for (indice = 1; indice <= 2; indice++ ){
                  nomePessoa1 = (JOptionPane.showInputDialog("Digite o seu nome"));
                  idadePessoa1 = Integer.parseInt(JOptionPane.showInputDialog("Digite a sua idade"));
              }
            }
        }*/
        
        //Escreva um algoritmo que imprima todos os resultados possíveis da combinação de dois dados de 6 lados;
        public class aulaAtividades{
            public static void main(String[] args){
               //Scanner ler = new Scanner(System.in);

               int numeroMaximoDado = 6;
               int dado1;
               int dado2;

               for (dado1=1; dado1<=numeroMaximoDado; dado1++){
                   for (dado2=1; dado2<=numeroMaximoDado; dado2++){
                       System.out.print("("+dado1+")");
                       System.out.println("("+dado2+")");
                   }
                   System.out.println("");
               }
            }
        }

