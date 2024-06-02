palavra =input("Digite a palavra tema: ")
letras_palavra = []
chances = 6
ganhou = False

def venceu():
    print(f"Parabéns você venceu! A palavra era: {palavra}")

def perdeu():
    print(f"Que pena... você perdeu o jogo. A palavra era: {palavra}")

while True:
    for letra in palavra:
        if letra in letras_palavra:
            print(letra, end="  ")
        else:
            print("_", end="  ")
    
    print("")
    tentativa = input("Digite uma letra: ")
    letras_palavra.append(tentativa)
    
    if tentativa not in palavra:
        chances -=1

    ganhou = True
    for letra in palavra:
        if letra not in letras_palavra:
            ganhou = False
    
    if chances ==0 or ganhou:
        break

if ganhou:
    venceu()

else:
    perdeu()
