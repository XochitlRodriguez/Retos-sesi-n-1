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





