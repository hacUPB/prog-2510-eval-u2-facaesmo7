import math

# 1. Calcular la distancia entre dos puntos
x1, y1 = map(float, input("Ingrese X1, Y1: ").split())
x2, y2 = map(float, input("Ingrese X2, Y2: ").split())
dx = x2 - x1
dy = y2 - y1
d = math.sqrt(dx**2 + dy**2)
print("La distancia entre los puntos es:", d)

# 2. Convertir metros a pulgadas
metros = float(input("Ingrese la cantidad en metros: "))
pulgadas = metros / 0.0254
print("La cantidad en pulgadas es:", pulgadas)

# 3. Calcular la hipotenusa de un triángulo rectángulo
a, b = map(float, input("Ingrese los valores de A y B: ").split())
c = math.sqrt(a**2 + b**2)
print("La hipotenusa es:", c)

# 4. Calcular la edad de una persona
dia_nac, mes_nac, ano_nac = map(int, input("Ingrese día, mes y año de nacimiento: ").split())
dia_act, mes_act, ano_act = map(int, input("Ingrese día, mes y año actual: ").split())

edad = ano_act - ano_nac
if mes_act < mes_nac or (mes_act == mes_nac and dia_act < dia_nac):
    edad -= 1
    print("Aún no ha cumplido años este año.")
elif mes_act == mes_nac and dia_act == dia_nac:
    print("¡Feliz Cumpleaños!")
else:
    print("Ya ha cumplido años este año.")
print("Su edad actual es:", edad)

# 5. Calcular el sueldo semanal basado en horas trabajadas
horas_trabajadas = float(input("Ingrese las horas trabajadas: "))
pago_por_hora = float(input("Ingrese el pago por hora: "))

if horas_trabajadas > 50:
    print("No está permitido trabajar más de 50 horas. Solo se pagará hasta 50 horas.")
    horas_trabajadas = 50

if horas_trabajadas <= 40:
    sueldo = horas_trabajadas * pago_por_hora
elif horas_trabajadas <= 45:
    sueldo = (40 * pago_por_hora) + ((horas_trabajadas - 40) * (2 * pago_por_hora))
else:
    sueldo = (40 * pago_por_hora) + (5 * 2 * pago_por_hora) + ((horas_trabajadas - 45) * (3 * pago_por_hora))

print("El sueldo semanal es:", sueldo)




El aspecto en el que siento que debo trabajar mas es en el lenguaje tecnico de python, terminus como "float" "else" "map" etc, aun asi siento que es un lenguaje de programacion facil de comprender a comparacion de otros, por lo cual agradezco que se enseñe y se evalue este jeje.