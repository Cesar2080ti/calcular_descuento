# CalculoDescuentoPython.py

def calcular_descuento(monto_total, porcentaje_descuento=10):
    """
    Calcula el monto del descuento basado en el monto total de la compra
    y un porcentaje de descuento dado.

    Parámetros:
    monto_total (float): El monto total de la compra.
    porcentaje_descuento (float, opcional): El porcentaje de descuento a aplicar. Por defecto es 10.

    Retorna:
    float: El monto del descuento calculado.
    """
    descuento = (monto_total * porcentaje_descuento) / 100
    return descuento

def main():
    # Primer ejemplo: solo monto total
    monto1 = 150.0
    descuento1 = calcular_descuento(monto1)
    monto_final1 = monto1 - descuento1
    print(f"Monto total: ${monto1:.2f}, Descuento: ${descuento1:.2f}, Monto a pagar: ${monto_final1:.2f}")

    # Segundo ejemplo: monto total y porcentaje de descuento
    monto2 = 200.0
    porcentaje2 = 15
    descuento2 = calcular_descuento(monto2, porcentaje2)
    monto_final2 = monto2 - descuento2
    print(f"Monto total: ${monto2:.2f}, Descuento: ${descuento2:.2f}, Monto a pagar: ${monto_final2:.2f}")

if __name__ == "__main__":
    main()
