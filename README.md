# Exercicio039.py

from datetime import date
atual = date.today().year
nasc = int(input('Digite o seu ano de nascimento: '))
idade = atual - nasc
print('Quem nasceu em {} tem {} anos em {}'. format(nasc,idade,atual))
if idade == 18:
    print('Tem que se alistar imediatamente.')
elif idade < 18:
    saldo = 18 - idade
    print('voce ainda nao tem 18 anos, ainda faltam {} anos para seu alistamento.'.format(saldo))
elif idade > 18:
    saldo = idade - 18
    print('voce deveria ter se alistado há {} anos.'.format(saldo))
