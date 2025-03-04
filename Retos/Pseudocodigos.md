1.Inicio
    Leer X1, Y1, X2, Y2
    Dx = X2 - X1
    Dy = Y2 - Y1
    D = sqrt(Dx^2 + Dy^2)
    Escribir "La distancia entre los puntos es: ", D
Fin

2.Inicio
    Leer metros
    pulgadas = metros / 0.0254
    Escribir "La cantidad en pulgadas es: ", pulgadas
Fin

3. Inicio
    Leer A, B
    C ←=sqrt(A^2 + B^2)
    Escribir "La hipotenusa es: ", C
Fin

4. Inicio
    Leer día_nacimiento, mes_nacimiento, año_nacimiento
    Leer día_actual, mes_actual, año_actual
    
    edad ← año_actual - año_nacimiento

    Si (mes_actual < mes_nacimiento) o (mes_actual = mes_nacimiento y día_actual < día_nacimiento) Entonces
        edad ← edad - 1  
        Escribir "Aún no ha cumplido años este año."
    Sino 
        Si (mes_actual = mes_nacimiento y día_actual = día_nacimiento) Entonces
            Escribir "¡Feliz Cumpleaños!"
        Sino
            Escribir "Ya ha cumplido años este año."
        Fin Si
    Fin Si

    Escribir "Su edad actual es: ", edad
Fin
5.Inicio
    Leer horas_trabajadas, pago_por_hora

    Si horas_trabajadas > 50 Entonces
        Escribir "No está permitido trabajar más de 50 horas. Solo se pagará hasta 50 horas."
        horas_trabajadas ← 50
    Fin Si

    Si horas_trabajadas ≤ 40 Entonces
        sueldo ← horas_trabajadas * pago_por_hora
    Sino 
        Si horas_trabajadas ≤ 45 Entonces
            sueldo ← (40 * pago_por_hora) + ((horas_trabajadas - 40) * (2 * pago_por_hora))
        Sino
            sueldo ← (40 * pago_por_hora) + (5 * 2 * pago_por_hora) + ((horas_trabajadas - 45) * (3 * pago_por_hora))
        Fin Si
    Fin Si

    Escribir "El sueldo semanal es: ", sueldo
Fin

6.Inicio
    Leer N
    ceros ← 0
    negativos ← 0
    positivos ← 0

    Mientras N > 0 Hacer
        Leer numero
        Si numero = 0 Entonces
            ceros ← ceros + 1
        Sino Si numero < 0 Entonces
            negativos ← negativos + 1
        Sino
            positivos ← positivos + 1
        Fin Si
        N ← N - 1
    Fin Mientras

    Escribir "Ceros:", ceros
    Escribir "Negativos:", negativos
    Escribir "Positivos:", positivos
Fin
7.Inicio
    ahorro_diario ← 0.03  // Inicia con 3 centavos
    ahorro_total ← 0      // Acumulador del ahorro anual

    Para dia ← 1 Hasta 365 Hacer
        Escribir "Día ", dia, ": ahorró $", ahorro_diario
        ahorro_total ← ahorro_total + ahorro_diario
        ahorro_diario ← ahorro_diario * 3 // Se triplica cada día
    Fin Para

    Escribir "El ahorro total en un año es: $", ahorro_total
Fin
8.Inicio
    Leer N  // Número de artículos
    total_a_pagar = 0

    Para i = 1 Hasta N Hacer
        Leer precio
        Si precio >= 200 Entonces
            descuento = precio * 0.15
        Sino Si precio > 100 Entonces
            descuento = precio * 0.12
        Sino
            descuento = precio * 0.10
        FinSi
        
        precio_final = precio - descuento
        total_a_pagar = total_a_pagar + precio_final

        Escribir "Artículo ", i, ": Precio = ", precio, ", Descuento = ", descuento, ", Final = ", precio_final
    FinPara

    Escribir "Total a pagar: ", total_a_pagar
Fin
9.Inicio
    Leer x
    termino ← 1
    resultado ← 1
    n ← 1

    Mientras termino > 0 Hacer  
        termino ← (termino * x) / n
        resultado ← resultado + termino
        n ← n + 1
    FinMientras

    Escribir "e^", x, " ≈ ", resultado
Fin
10.