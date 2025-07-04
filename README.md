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
    
```
