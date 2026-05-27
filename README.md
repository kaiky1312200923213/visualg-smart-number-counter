# criando-contador-numero-inteligente-com-visualg
Algoritmo "calculaNumeros"
Var
   numero, soma, cont, nulo, divPor5 : inteiro
   media : real

Inicio
   soma     <- 0
   nulo     <- 0
   divPor5  <- 0

   para cont de 1 ate 5 faca
      escreva("Digite o ", cont, "º número: ")
      leia(numero)

      soma <- soma + numero

      se numero = 0 entao
         nulo <- nulo + 1
      fimse

      se numero mod 5 = 0 entao
         divPor5 <- divPor5 + 1
         escreval(">>> O número ", numero, " é divisível por 5!")
      fimse

   fimpara

   media <- soma / 5

   escreval("----------------------------")
   escreval("Soma dos números  : ", soma)
   escreval("Média dos números : ", media:0:2)
   escreval("Quantidade de zeros   : ", nulo)
   escreval("Divisíveis por 5  : ", divPor5)
   escreval("----------------------------")

Fimalgoritmo
