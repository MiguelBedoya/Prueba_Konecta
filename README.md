# PRUEBA KONECTA
## MIGUEL ANGEL BEDOYA GALEANO

1 | SELECT id_fabricante, id_producto, descripción, precio, precio*1.10 AS precio_iva FROM productos

2 	
	1| SELECT Apellidos FROM EMPLEADOS

	2| SELECT DISTINCT Apellidos FROM EMPLEADOS

	3| SELECT * FROM EMPLEADOS WHERE Apellidos ='lopez' OR Apellidos = 'perez'

	4| SELECT SUM (Presupuesto) FROM DEPARTAMENTOS

	5| SELECT Departamento, COUNT(*) FROM EMPLEADOS GROUP BY Departamento

	6| SELECT Nombre, Apellidos FROM EMPLEADOS WHERE Departamento IN

	(SELECT Codigo FROM DEPARTAMENTOS WHERE Presupuesto > 60000)

	7| UPDATE EMPLEADOS SET Departamento = 14 WHERE Departamento = 77

	8| DELETE FROM EMPLEADOS WHERE Departamento = 14

3

import java.text.ParseException;

import java.util.Calendar;

public class Fecha {

    public static void fechaHabil(Calendar fecha, int dias) throws ParseException{

         int dia =fecha.get(Calendar.DAY_OF_MONTH) ;
         if (validarFecha(fecha)) {
            for (int i = 0; i < dias; i++) {
            }
        }else{
             System.out.println("la fecha no puede ser menor a la actual");
         }
         System.out.println(dia);
    }
    public static boolean validarFecha(Calendar fecha){
        Calendar fechaActual = Calendar.getInstance();
        if (fechaActual.before(fecha)) {
            return true;
        }
        return false;
    }
    public static void main(String[] args) {
         try {
            Calendar c1 = Calendar.getInstance();
        c1.set(2020, 2, 10);
            fechaHabil(c1, 2);
        } catch (Exception e) {
            System.out.println(e.getMessage());
        }
    }
}

4  | Especificación o levantamiento de requisitos.

   | Se procede a realizar un diseño del software

   | Se empieza a construir el sistema

   | Integración 

   | Pruebas o validaciones

   | Despliegue

   | Mantenimiento

5
## PREGUNTAS
¿Cómo podría reconocer a un cliente nuevo?

¿Cómo saber si la persona está inscrita?

¿Cómo puedo inscribir a un cliente nuevo?

5 | C  >> Es un modelo o plantilla a partir de la cual creamos objetos

6 | C >> Crear un objeto a partir de la clase

7 | B >> Sus atributos y sus métodos

8|
Polimorfismo: Significa “varias formas diferente” esta característica permite definir distintos comportamientos para un método dependiendo de la clase sobre la que se realice la implementación.

Herencia: Es el mecanismo que me permite tomar los atributos y métodos de una clase padre,  y crear nuevos objetos a partir de este; esto me favorece para la reutilización de código.

Encapsulamiento: El concepto de encapsulamiento es proteger los datos internos, al definir atributos  como privados.

Abstracción: Es la capacidad de concentrar las propiedad y comportamientos necesarios para la correcta representación del objeto dentro del sistema.