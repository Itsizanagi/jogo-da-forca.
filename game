import random
import time
palavra = ('destiny', 'polazi', 'carro')
palavra_secreta = random.choice(palavra)
letras_escolhidas_pela_pessoa = []
underline1= ["_", "_", "_", "_","_","_","_"]
underline2 = ["_", "_", "_", "_", "_","_"]
underline3 = ["_", "_", "_", "_", "_",]
tentativas = 2
acertos = 0

print('='*20)
print("-運命jogo da forca!運命-")
print('='*20)
print("Ola, me chamo izanagi. vamos jogar?")
jogar = str(input("Sim ou Não: ")).strip().upper()

if jogar in 'SIM':
    print("Voce tem 2 chances para acertar a palavra!")
    print("\033[31mPensando aguarde.")
    time.sleep(3)
    print("\033[30mPalavra escolhida com sucesso!")
    print(" A palavra tem {} letras".format(len(palavra_secreta)))
    print("_"*len(palavra_secreta))
else:
    print("Ate a proxima!")
    exit()

while True:
    print("Qual letra voce acha que a palavra tem?? ")
    letra = str(input("Letra:"))
    letras_escolhidas_pela_pessoa.append(letra)
    print('letras tentadas: {}'.format(letras_escolhidas_pela_pessoa))

    if palavra_secreta == 'destiny':
        if letra in palavra_secreta:
            print("Voce acertou uma letra na {} posição!".format(palavra_secreta.index(letra)))
            underline1[palavra_secreta.index(letra)] = (letra)
            print(underline1)
            acertos += 1
        else:
            print("poxa, voce errou uma letra. Tente novamente")
            tentativas -= 1
            print("Agora você tem {} chances".format(tentativas))
            if tentativas <= 0:
                print("derrota :(")
                break
        if acertos == 4:
            print('Parabens!')
            break

    if palavra_secreta == 'polazi':
        if letra in palavra_secreta:
            print("Voce acertou uma letra na {} posição!".format(palavra_secreta.index(letra)))
            underline2[palavra_secreta.index(letra)] = (letra)
            print(underline2)
            acertos += 1
        else:
            print("poxa, voce errou uma letra. Tente novamente")
            tentativas -= 1
            print("Agora você tem {} chances".format(tentativas))
            if tentativas <= 0:
                print("derrota :(")
                break
        if acertos == 5:
            print('Parabens!')
            break

    if palavra_secreta == 'carro':
        if letra in palavra_secreta:
            print("Voce acertou uma letra na {} posição!".format(palavra_secreta.index(letra)))
            underline3[palavra_secreta.index(letra)] = (letra)
            print(underline3)
            acertos += 1
        else:
            print("poxa, voce errou uma letra. Tente novamente")
            tentativas -= 1
            print("Agora você tem {} chances".format(tentativas))
        if tentativas <= 0:
            print("derrota :(")
            break
        if acertos == 6:
            print('Boa Campeao!')
            break

print("Ate a proxima")
