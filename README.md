# Tecnicas-de-Prog.-3er-Parc
Programa Menu 3er Parcialpackage examenjava;
import java.util.Scanner;
public class parcial {

　
	    static Scanner scanner = new Scanner(System.in); //Sirve para recoger texto por consola
	    static int select = -1; //opción elegida del usuario
	    static int num1 = 0, num2 = 0; //Variables

	    public static void main(String[] args) {

	        //Mientras la opción elegida sea 0, preguntamos al usuario
	        while(select != 0){
	            //Try catch para evitar que el programa termine si hay un error
	            try{
	                System.out.println("Elige opción:\n1.- Validar Edad (IF)" +
	                        "\n2.- Ingresar Nombre (FOR)\n" +
	                        "3.- Matriz\n" +
	                        "4.- Vectores\n" +
	                        "0.- Salir");
	                //Recoger una variable por consola
	                select = Integer.parseInt(scanner.nextLine()); 

	                //Ejemplo de switch case en Java
	                switch(select){
	                case 1: 
	                    Scanner scanner = new Scanner(System.in);
	                    System.out.print("Ingresa tu edad");
	                    int edad = scanner.nextInt();
	                    if (edad >= 18) {
	                        System.out.println("Puedes ingresar a beber");
	                    } else {
	                        System.out.println("No puedes ingresar al bar");
	                    }
	                    System.out.print("mostrar la edad: ");
	                    System.out.println(edad);

　
	                    break;
	                case 2: 
	                    //Creo una variable tipo String con nombre: "nombre" 
	                    String nombre; 

	                    // Creo mi Scanner con nombre: "T" 
	                    Scanner T = new Scanner (System.in); 

	                    //Inicio mi for con una variable "i" comenzada en 0 ( cero), hasta que i sea mener que 4 e "i" valla aumnetado en 1 
	                    for (int i = 0 ; i<4 ; i++){ 
	                    //Comienza contenido del for 
	                    System.out.print("Ingrese nombre N° "+(i+1)+": " ); 
	                    nombre = T.nextLine(); 

	                    System.out.println("=============Bienvenido=============" ); 
	                    System.out.println("Bienvenido "+ nombre); 
	                    System.out.println("====================================" ); 
	                    //finaliza contenido del for 
	                    } 

	                    System.out.println("Todos los nombres fueron ingresados exitosamente." ); 

　
　
	                    break;
	                case 3: 
	                    Scanner reader = new Scanner(System.in);

	                    int uno, dos, tres, cuatro, cinco, seis, siete, ocho, nueve, diez;

	                    System.out.println("Creación de una matriz con dos filas y cinco columnas: ");

	                    System.out.print("Ingresa el primer valor de la columna uno: ");
	                    uno = reader.nextInt();
	                    System.out.print("Ingresa el segundo valor de la columna uno: ");
	                    dos = reader.nextInt();
	                    System.out.print("Ingresa el primer valor de la columna dos: ");
	                    tres = reader.nextInt();
	                    System.out.print("Ingresa el segundo valor de la columna dos: ");
	                    cuatro = reader.nextInt();
	                    System.out.print("Ingresa el primer valor de la columna tres: ");
	                    cinco = reader.nextInt();
	                    System.out.print("Ingresa el segundo valor de la columna tres: ");
	                    seis = reader.nextInt();
	                    System.out.print("Ingresa el primer valor de la columna cuatro: ");
	                    siete = reader.nextInt();
	                    System.out.print("Ingresa el segundo valor de la columna cuatro: ");
	                    ocho = reader.nextInt();
	                    System.out.print("Ingresa el primer valor de la columna cinco: ");
	                    nueve = reader.nextInt();
	                    System.out.println("Ingresa el segundo valor de la columna cinco: ");
	                    diez = reader.nextInt();

	                    System.out.println(uno + " " + tres + " " + cinco + " " + siete + " " + nueve);
	                    System.out.println(dos + " " + cuatro + " " + seis + " " + ocho + " " + diez);

	                    break;
	                case 4: 
	                    Scanner reader1 = new Scanner(System.in);

	                    int nElementos, i, suma = 0 ;

	                    System.out.print("Ingresa la cantidad de elementos que deseas que tenga el vector: ");
	                    nElementos = reader1.nextInt();
	                    int Arreglo[] = new int [nElementos];

	                    for(i=0;i<Arreglo.length;i++){
	                    System.out.println("Ingresa el valor" + " " + i +":");
	                    Arreglo[i] = reader1.nextInt();
	                    }

	                    System.out.println("Arreglo");

	                    for(i=0;i<Arreglo.length;i++){
	                    System.out.println(Arreglo[i]);
	                    }

	                    for(int j=0;j<Arreglo.length;j++){

	                    suma+=Arreglo[j];
	                    }

	                    System.out.println("La suma de todos los elementos es: " + suma);

　
	                    break;
	                case 0: 
	                    System.out.println("Adios!");
	                    break;
	                default:
	                    System.out.println("Número no reconocido");break;
	                }

	                System.out.println("\n"); //Mostrar un salto de línea en Java

	            }catch(Exception e){
	                System.out.println("Error! Error!");
	            }
	        }

	    }

	    //Método para recoger variables por consola
	    public static void pideNumeros(){
	        System.out.println("Introduce número 1:");
	        num1 = Integer.parseInt(scanner.nextLine());

	        System.out.println("Introduce número 2:");
	        num2 = Integer.parseInt(scanner.nextLine());

	        //Mostrar un salto de línea en Java
	        System.out.println("\n"); 
	    }

	}
