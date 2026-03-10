# BETA1.py
# REALIZAREMOS UN PROGRAMA QUE NOS EVALUE NUESTRO PROMEDIO EN RIWI

#Inicialiazamos y limpiamos las variables que vamos a usar
nota1 = 0
nota2 = 0
nota3 = 0
promedio = 0

#Ingreso de las 3 notas
nota1 = float (input("Ingrese su nota de INGLES  "))
nota2= float (input("Ingrese su nota de DESARROLLO  "))
nota3=float (input("Ingrese su nota de SICOCIAL  "))

#validamos que el usuario no nos ingrese una nota fuera del rango
if (nota1 < 1 or nota1 > 5) or (nota2< 1 or nota2> 5) or  (nota3< 1 or nota3 >5):
    print ("Error al digitar su nota, POR FAVOR DIGITE UNA NOTA VALIDA!")
else:
    #calculamos el promedio
    promedio = (nota1 * 0.60) + (nota2 * 0.20) + (nota3 * 0.20)
    print ("El promedio del estudiantes es:  ", promedio)

    #Clasificamos el promedio segun los estandares de riwi
    if promedio < 3:
        print ("NOTA BAJA")
    elif promedio == 3:
        print ("NOTA REGULAR")
    elif promedio > 3 and promedio < 4:
        print ("NOTA BUENA")
    elif promedio >=4:
        print("NOTA EXCELENTE")
