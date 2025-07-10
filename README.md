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



class Retangulo
  def initialize(modelo, cor)
    @modelo = modelo
    @cor = cor
  @ligado = false
  end

  def ligar
    puts "#{@modelo} ta ligado!"
  end
end


retangulo = Retangulo.new("Honda Civic", "Prata")


retangulo.ligar


DESAFIO FINAL
class Produto
  def initialize(nome, preco)
    @nome = nome
    @preco = preco
  end

  def aplicar_desconto(percentual)
    desconto = @preco * (percentual / 100.0)
    @preco -= desconto
    puts "Novo preço de #{@nome} após o desconto de #{percentual}%: R$#{@preco.round(2)}"
  end
end

produto = Produto.new("Camiseta", 50)
produto.aplicar_desconto(20)

```


```rb
Atividades do dia 08/07/2025
Exercício 1.1
class Livro
  def initialize(t, a)
    @titulo = t
    @autor = a
  end

  def titulo
    @titulo
  end
end

Exercício 1.3
class Livro
  attr_reader :titulo, :autor

  def initialize(t, a)
    @titulo = t
    @autor = a
  end
end

Exercício 2.1
class Aluno
  attr_accessor :nome

  def initialize(nome)
    @nome = nome
  end
end

aluno = Aluno.new("Jota")
puts "Seu nome era: #{aluno.nome}"
aluno.nome = "Miguel"
puts "Agora é: #{aluno.nome}"

Exercício 3.2 e 3.3
class Guerreiro
  attr_accessor :nome, :vida

  def initialize(n, v)
    @nome = n
    @vida = v
  end

  def receber_dano(dano)
    @vida -= dano
  end
end

guerreiro = Guerreiro.new("Thor", 100)
puts "Vida inicial: #{guerreiro.vida}"

guerreiro.receber_dano(20)
puts "Vida após dano: #{guerreiro.vida}"



class Guerreiro
  attr_accessor :nome, :pontuacao

  def initialize(n, p)
    @nome = n
    @pontuacao = p
  end

  def receber_pontos(pontos)
    @pontuacao += pontos
  end
end

guerreiro = Guerreiro.new("Buzz", 0)
puts "Pontos iniciais: #{guerreiro.pontuacao}"

guerreiro.receber_pontos(20)
puts "Pontos agora: #{guerreiro.pontuacao}"

```


```rb
Atividades do dia 09/02/2025
Desafio 1: 

  def descrever
    "O livro '#{@titulo}' de #{@autor} tem #{@numero_paginas} páginas."
  end
end

livro = Livro.new("Diário de um Banana 2", "Jeff Kinney", 224)
puts livro.descrever
Desafio 2:
class Retangulo
  def initialize(base, altura)
    @base = base
    @altura = altura
  end

  def calcular_area
    @base * @altura
  end

  def calcular_perimetro
    2 * (@base + @altura)
  end

  def formatar_maiuscula(texto)
    texto.upcase
  end
end

puts "Diga a base do retângulo"
base = gets.chomp.to_i
puts "Diga a altura do retângulo"
altura = gets.chomp.to_i

retangulo = Retangulo.new(base, altura)

area = retangulo.calcular_area
perimetro = retangulo.calcular_perimetro

puts "A área do retângulo é: #{retangulo.formatar_maiuscula(area.to_s)}"
puts "O perímetro do retângulo é: #{retangulo.formatar_maiuscula(perimetro.to_s)}"



Desafio 3: 
        class Elevador
  attr_accessor :andar_maximo, :andar_atual

  def initialize(andar_maximo)
    @andar_maximo = andar_maximo
    @andar_atual = 0  # O elevador começa no térreo
  end

  def subir
    if @andar_atual < @andar_maximo
      @andar_atual += 1
      puts "Subindo, O elevador está no andar #{@andar_atual}."
    else
      puts "Você já está no andar máximo (#{@andar_maximo})."
    end
  end

  def descer
    if @andar_atual > 0
      @andar_atual -= 1
      puts "Descendo, O elevador está no andar #{@andar_atual}."
    else
      puts "O elevador já está no térreo (andar 0)."
    end
  end

  def status
    puts "O elevador está no andar #{@andar_atual} de #{@andar_maximo}."
  end
end


Desafio 4
class ContaBancaria
 attr_reader :titular, :saldo
 def initialize(titular, saldo_inicial)
 @titular = titular
 @saldo = saldo_inicial
 @extrato = []
 end

 def depositar(valor)
    depositar +=valor
    @extrato << {tipo: "saque", valor: valor}
 end
 def saque(valor)
   if @saldo >= valor
    sacar -=valor
    @extrato << {tipo: "saque", valor: valor}
   end
end
def imprimir_extrato
    puts "Extrato: #{@titular}"
    extrato.each do |transacao|
        puts "#{transacao[:tipo].capitalize}: R$ #{'%.2f' % transacao[:valor]}"
 end
 puts "--- Saldo Final: R$ #{'%.2f' % @saldo} ---"
end
end
conta = ContaBancaria.new("Alisson", 900)
conta.depositar(400)
conta.sacar(350)
conta.imprimir_extrato
```


```rb
Atividades do dia 10/07/2025
Exercício 1
class Animal
  attr_reader :nome, :tipo

  def initialize(nome, tipo)
    @nome = nome
    @tipo = tipo
  end

  def dormir
    puts "zzzz"
  end
end
class Gato < Animal
Exercício
end
meu_gato = Gato.new("Kvaratskhelia", "Gato")
meu_gato.dormir

Exercício 2
class Funcionario
  attr_reader :nome, :salario

  def initialize(nome, salario)
    @nome = nome
    @salario = salario
  end
end

class Gerente < Funcionario
  attr_reader :bonus
  
  def initialize(nome)
    super(nome, 5000)
    @bonus = 0
  end

  def detalhes
    puts "Seu nome é #{@nome} e você tem um salário inicial de #{@salario}."
  end
end

gerente = Gerente.new("Felipinho")
gerente.detalhes
Exercício 3
class Funcionario
  attr_reader :nome, :salario

  def initialize(nome, salario)
    @nome = nome
    @salario = salario
  end
end

class Gerente < Funcionario
  attr_reader :bonus
  
  def initialize(nome)
    super(nome, 5000)
    @bonus = 0
  end

  def detalhes
    puts "Seu nome é #{@nome} e você tem um salário inicial de #{@salario}."
  end
end

gerente = Gerente.new("Felipinho")
gerente.detalhes
exercício 4
class 
    def falar
        puts "Esse animal emite um som"
    end
end
class Cachorro < Animal 
    def falar
        puts "Au Au!"
    end
end
class Gato < Animal
    def falar
        puts "Miau!"
    end
end

animal = Animal.new
animal.falar
cachorro = Cachorro.new
cachorro.falar
gato = Gato.new
gato.falar

Exercício final
class Funcionario
  attr_reader :nome, :salario

  def initialize(nome, salario_base)
    @nome = nome
    @salario = salario_base
  end

  def calcular_salario
    @salario
  end
end

class Gerente < Funcionario
  def initialize(nome, salario_base, bonus)
    super(nome, salario_base)
    @bonus = bonus
  end

  def calcular_salario
    @salario + @bonus
  end    
end

class Vendedor < Funcionario
  def initialize(nome, salario_base)
    super(nome, salario_base)
    @comissao = 0
  end

  def add_comissao(qtd)
    @comissao += qtd * 100
  end

  def calcular_salario
    @salario + @comissao
  end
end

funcionario = Funcionario.new("Carlos", 1500)
gerente = Gerente.new("Ana", 5000, 1000)
vendedor = Vendedor.new("Lucas", 2000)
vendedor.add_comissao(3)


```

