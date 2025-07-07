# atividades-do-cursoo

```rb
Atividades 04/07/2025


Atividade 1 Def
def mostrar_linha
    puts "----------------*--------------"
end

puts "Jota M"
mostrar_linha
puts "Mais conhecido como João Miguel"

Atividade 1.1 
def mostrar_menu
    puts "Login"
    puts "Configurações"
    puts "Política de Privacidade"
end

mostrar_menu

Atividade 2
puts "Diga seu nome"
nome = gets.chomp
puts "Diga sua idade"
idade = gets.chomp

def saudar(nome, idade)
  puts "Olá, #{nome}, de acordo com as suas informações você tem #{idade} anos."
end

saudar(nome, idade)


puts "Qual a sua idade?"
idade = gets.chomp.to_i

def verificar_idade(idade)
  if idade < 0
    puts "Rapaz, tá no útero é?"
  elsif idade <= 3
    puts "Quer mamadeira, pirralho!"
  elsif idade <= 13
    puts "Criança, kkk!"
  elsif idade <= 18
    puts "Adolescente brabo!"
  elsif idade <= 37
    puts "Adulto!"
  else
    puts "Velhão!"
  end
end

verificar_idade(idade)



def mostrar_tabuada(numero_da_tabuada)
  i = 1
  while i <= 10
    resultado = numero_da_tabuada * i
    puts "#{numero_da_tabuada} x #{i} = #{resultado}"
    i += 1
  end
end

puts "Digite um número para a tabuada:"
numero_do_usuario = gets.chomp.to_i

mostrar_tabuada(numero_do_usuario)
Atividade 3
puts "Diga a base do retangulo"
base = gets.chomp.to_i
puts "Diga a altura do retangulo"
altura = gets.chomp.to_i

def calcular_area_retangulo(base, altura)
  base * altura
end

area = calcular_area_retangulo(base, altura)
puts "A área do retângulo é: #{area}"

def formatar_maiuscula(texto)
    texto.upcase
end
nome_original = "JotaM"
nome_formatado = formatar_maiuscula(nome_original)

puts "O nome original é: #{nome_original}"
puts "O nome formatado é: #{nome_formatado}"    

def par(numero)
  numero % 2 == 0
end

numero_para_testar = 0

if par(numero_para_testar)
  puts "O número #{numero_para_testar} é par"
else
  puts "O número #{numero_para_testar} é ímpar"
end

DESAFIO FINAL

def calcularpfinal(preco_original, desconto_percentual)
 desconto_percentual = desconto_percentual.to_f / 100
 preco_final =  preco_original -  preco_original * desconto_percentual 
 end
 
 final = calcularpfinal(1500, 10)
 
 puts final
 
```

```rb
Atividades 07/07/2025
class Aluno
  def initialize(nome, matricula)
    @nome = nome
    @matricula = matricula
  end

  def exibir
    puts "#{@nome} - Matrícula: #{@matricula}"
  end
end

# Criando os alunos diretamente
joao = Aluno.new("João", "123")
ana = Aluno.new("Ana", "456")

# Exibindo os alunos
joao.exibir
ana.exibir


class Retangulo
  def initialize(base, altura)
    @base = base
    @altura = altura
  end

  def mostrar
    puts "Base é #{@base} e altura é #{@altura}"
  end
end


retangulo = Retangulo.new(4, 3)


retangulo.mostrar


class Retangulo
  def initialize(nome_titular, saldo_inicial)
    @titular = nome_titular
    @saldo = saldo_inicial
  end

  def mostrar
    puts "Seu nome é #{@titular} seu saldo é é #{@saldo}"
  end
end


retangulo = Retangulo.new("Joao", 300)


retangulo.mostrar

```
