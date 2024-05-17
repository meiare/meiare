Algoritmo CalcularCostoColas
    Definir cantidadColas, costoBase, costoTotalSinIVA, iva, totalAPagar Como Real
	
    Escribir "Ingrese la cantidad de colas compradas:"
    Leer cantidadColas
	
    Si cantidadColas > 23 Entonces
        costoBase = 0.50
    Sino
        costoBase = 1.20
    FinSi
	
    costoTotalSinIVA = cantidadColas * costoBase
    iva = 0.12 * costoTotalSinIVA
    totalAPagar = costoTotalSinIVA + iva
	
    Escribir "Cantidad comprada:", cantidadColas
    Escribir "Costo por unidad: $", costoBase
    Escribir "Total sin IVA: $", costoTotalSinIVA
    Escribir "IVA (12%): $", iva
    Escribir "Total a pagar: $", totalAPagar
FinAlgoritmo
