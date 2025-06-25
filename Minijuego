import random

def adivinanza():
    numero = random.randint(1, 10)
    intentos = 5
    puntaje = 0
    adivinado = False

    while intentos > 0:
        try:
            guess = int(input(f"Cual numero crees que va a salir?(entre 1 y 10):"))
        except ValueError:
            print("Por favor, ingresa un número válido.")
            continue

        if guess == numero:
            puntaje += 1
            print("¡Felicidades! Has adivinado el número.")
            adivinado = True
            break
        else:
            intentos -= 1
            print("No has adivinado el numero")
            if intentos > 0:
                print(f"Te quedan {intentos} intentos")
            print(f"Tu puntaje es: {puntaje} puntos")

    if not adivinado:
        print(f"No has adivinado el numero, el numero es {numero}")
        print(f"Tu puntaje es: {puntaje} puntos")

if __name__ == "__main__":
    adivinanza()
