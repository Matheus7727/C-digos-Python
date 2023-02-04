# Python-colab


print("Olá, bem vindo ao mundo da programação Python")

mensagem = "Olá, bem vindo ao mundo da programação Python... :)"
print(mensagem)

mensagem = input("Por favor, digite um texto qualquer: ")
print("Você digitou: "+mensagem)

mensagem = "Olá, bem vindo ao mundo da programação Python... :)"
print(mensagem.lower())

mensagem = "Olá, bem vindo ao mundo da programação Python... :)"
print(mensagem.title())

mensagem = "Olá, bem vindo ao mundo da programação Python... :)"
print(mensagem.upper())

nome = input("Digite seu nome: ")
telefone = input("Digite se número de telefone: ")
email = input("Digite seu melhor e-mail: ")
print("Nome: "+nome+" - Telefone: "+telefone+" - email: "+email)

primeironome = input("Digite seu nome: ")
telefone = input("Digite se número de telefone: ")
email = input("Digite seu melhor e-mail: ")
textoDigitado = "Nome: %s - Telefone: %s - e-mail: %s" % (primeironome, telefone, email)
print(textoDigitado)

help("keywords")

valorA = 10
valorB = int(20.55)
valorC = int(valorA + valorB)
print(valorA,valorB, valorC)
print(type(valorA), type(valorB), type(valorC))

# Operações Aritméticas
A = 10
B = 20
# Adição
c = A + B
print(c)
# Subtração
d = A - B
print(d) 
# Multiplicação
e = A * B
print(e)
# Divisão
f = A / B
print(f)
# Exponenciação
g = A ** B
print(g)

a = 10.37
b = 7.75
c = a * b
print(c)
resultado = "Resultado: {:7.4f} ".format(c)
print(resultado)

a = 2+4j
b = 6+3j

c = a ** b

print(c)

a = -10.85
b = 2
c = 4

print(int(a))
print(complex(b))
print(pow(b,c))
print(int(abs(a)))

# hex 16
# 0123456789abcdef

# oct 8

# 255 = ff  

print(oct(10))
print(hex(255))


a = 12.5678985
print(round(a,6))


# Operadores lógicos
# and - or - not
a = 21
b = 24
c = not((not a))
print(c)

# saldo é R$ 100,00
# pode sacar qualquer valor até R$ 100,00
# sacar R$ 80,00 - ok saldo restante R$ 20,00
# sacar R$ 10,00 - ok saldo restante R$ 10,00
# sacar R$ 25,00 - negado sem saldo
# IF ELSE
saldo = 100

if saldo>=0: print(" Seu Saldo Atual é R$ %d " % (saldo))

if saldo<0: print(" Seu Saldo Atual é (negativo) R$ %d " % (saldo))

valorSaque = 80

if saldo-valorSaque>=0: print("Saque efetuado - R$ %d " % (valorSaque))

saldo = saldo - valorSaque

if saldo>=0: print(" Seu Saldo Atual é R$ %d " % (saldo))

valorSaque = 10

if saldo-valorSaque>=0: print("Saque efetuado - R$ %d " % (valorSaque))

saldo = saldo - valorSaque

if saldo>=0: print(" Seu Saldo Atual é R$ %d " % (saldo))

valorSaque = 25

if saldo-valorSaque<0: 
  print("Saque não efetuado no valor de R$ %d " % (valorSaque))

if saldo>=0: print(" Seu Saldo Atual é R$ %d " % (saldo))



# saldo é R$ 100,00
# pode sacar qualquer valor até R$ 100,00
# sacar R$ 80,00 - ok saldo restante R$ 20,00
# sacar R$ 10,00 - ok saldo restante R$ 10,00
# sacar R$ 25,00 - negado sem saldo
# IF ELSE IF

saldo = 100

if saldo>=0:
   print(" Seu Saldo Atual é R$ %d " % (saldo))
else:
   print(" Seu Saldo Atual é (negativo) R$ %d " % (saldo))

valorSaque = 80

if (saldo-valorSaque)>=0: 
  print("Saque efetuado - R$ %d " % (valorSaque))
  saldo = saldo - valorSaque
  print(" Seu Saldo Atual é R$ %d " % (saldo))
else:
  print(" Seu Saldo Atual é R$ %d " % (saldo))
  print(" Saque não efetuado no valor de R$ %d " % (valorSaque))


valorSaque = 10

if (saldo-valorSaque)>=0: 
  print("Saque efetuado - R$ %d " % (valorSaque))
  saldo = saldo - valorSaque
  print(" Seu Saldo Atual é R$ %d " % (saldo))
else:
  print(" Seu Saldo Atual é R$ %d " % (saldo))
  print(" Saque não efetuado no valor de R$ %d " % (valorSaque))


valorSaque = 25

if (saldo-valorSaque)>=0: 
  print("Saque efetuado - R$ %d " % (valorSaque))
  saldo = saldo - valorSaque
  print(" Seu Saldo Atual é R$ %d " % (saldo))
else:  
  print(" Saque não efetuado no valor de R$ %d " % (valorSaque))


# saldo é R$ 100,00
# limite especial R$ 200,00
# 
# if elif else

saldo = 0
limite = 0

if (saldo>0):
  print("Saldo atual sem limite é: R$ %d " % (saldo))
elif (limite>0):
  print("Saldo no limite é: R$ %d " % (limite))
else:
  print("Saldo atual sem limite é: R$ %d " % (saldo))
  print("Saldo do limite é: R$ %d " % (limite))

# while 
# for

numero = 0

while numero <10:
  print("Número %d " % (numero))
  numero = numero + 1 
print("Fim do processamento com o Loop While")

# coleta de dados valor sempre positivo
# quantidade de vendas - contador
# valor médio das vendas
# valor total das vendas

# enquanto o número -1

dadoVenda = 0
contador = 0
valorMedioDasVendas = 0
valorTotalDasVendas = 0

while dadoVenda>=0:
   dadoVenda = int(input("Digite o valor da venda, ou -1 para finalizar.\n"))
   if dadoVenda>=0:
    contador = contador + 1
    valorTotalDasVendas = valorTotalDasVendas + dadoVenda
valorMedioDasVendas = valorTotalDasVendas / contador
print("Total das Vendas: %d " % (valorTotalDasVendas))
print("Média das Vendas: %d " % (valorMedioDasVendas))
print("Quantida de vendas: %d " % (contador))

# laço for simples
# sequencia = [10,12,13,14,15,16]
# for x in sequencia:
     # codigo
     # codigo
     # codigo

sequencia = [10,11,12,13,14,15,16]
for x in sequencia:
    print("Número: %d " % (x))

# laço for simples com tuplas
# tupla = [10,"Laranja",13]
# for x in sequencia:
     # codigo
     # codigo
     # codigo

tupla = [10,"Laranja",13,"Carro",2+4j,0xff, 0o22, "Marco Maddo"]
for x in tupla:
    print("Registro: ",x)
