# Retos-sesi-n-1
#######################################RETO 1####################################################
public class Paciente {
    // Atributos
    String nombre;
    int edad;
    String numerodeExpediente;


    // Métodos
    public void mostrarInformacion() {
        System.out.print("Paciente: " + nombre);
        System.out.print("Edad:" + edad);
        System.out.print("Número de expediente: " + numerodeExpediente);
    }

}

import java.util.Scanner;

public class Principal {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Crear un objeto de tipo Paciente
        Paciente paciente1 = new Paciente();

        // Solicitar datos al usuario
        System.out.print("Ingrese el nombre del paciente: ");
        paciente1.nombre = scanner.nextLine();

        System.out.print("Ingrese la edad del paciente: ");
        paciente1.edad = scanner.nextInt();
        scanner.nextLine(); // Limpiar el buffer

        System.out.print("Ingrese el número de expediente: ");
        paciente1.numerodeExpediente = scanner.nextLine();

        // Mostrar la información del paciente
        System.out.println("\nInformación del paciente:");
        paciente1.mostrarInformacion();

        scanner.close();
    }
}


################################ RETO 2  ######################################################

public class Entrada {
    // Atributos
    String NombreEvento;
    double PrecioEntrada;

    //Constructor
    public Entrada (String NombreEvento, double PrecioEntrada) {
        this.NombreEvento = NombreEvento;
        this.PrecioEntrada = PrecioEntrada;
    }

    // Métodos
    public void mostrarInformacion() {
        System.out.print("Evento:" + NombreEvento + "| Precio:" + PrecioEntrada);
    }
}


public class Principal2 {
    public static void main(String[] args) {
        //Objetos
        Entrada entrada1 = new Entrada("Obra de Teatro", 100.0);
        Entrada entrada2 = new Entrada("Tamborileros de Tabasco", 300.0);
        Entrada entrada3 = new Entrada( "Rivera Maya", 350);

        // Resultados
        entrada1.mostrarInformacion();
        entrada2.mostrarInformacion();
        entrada3.mostrarInformacion();
    }
}




