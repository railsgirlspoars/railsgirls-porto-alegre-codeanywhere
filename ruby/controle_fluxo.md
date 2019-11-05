### Controle de fluxo

Até então escrevemos código que é executado sequenciamente e nesta seção
mostraremos uma forma de controlar o fluxo do programa, a partir de alguma
condição. Com isso poderemos realizar decisões durante a execução da nossa
aplicação.

Parece difícil, mas bem simples e fica mais ainda a medida que vamos praticando. Pense como uma tomada de decisão, a partir de uma sentença, escolhemos o que o programa irá fazer.

Por exemplo, vamos imprimir no método `escrever_nome` criado na seção anterior
apenas se o nome não estiver em branco.

```ruby
if nome != ''
  "Seu nome é " + nome
end
```

Outra forma de implementar seria utilizando o método `empty?`

```ruby
if !nome.empty?
  "Seu nome é " + nome
end
```

E nosso método ficaria assim:

```ruby
def escrever_nome(nome)
  if !nome.empty?
    "Seu nome é " + nome
  end
end
```
