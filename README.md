# Media-exame
Media exame com Vetores
Algoritmo "Medias"
//
//
// Descrição   : Aqui você descreve o que o programa faz! (função)
// Autor(a)    : Nome do(a) aluno(a)
// Data atual  : 03/04/2023
const
   qtd_alunos = 10

   -
Var
   // Seção de Declarações das variáveis

   x : inteiro
   alunos: vetor [ 1..qtd_alunos] de caractere
   media_ano,media_final,exame,media,nota_exame, nota1, nota2, nota3, nota4: vetor [1..qtd_alunos] de real



Inicio

   para x de 1 ate qtd_alunos faca
      escreval("Digite o nome do aluno: ")
      leia(alunos[x])

      Escreval("Digite a primeira nota: ")
      leia(nota1[x])

      Escreval("Digite a primeira nota: ")
      leia(nota2[x])

      Escreval("Digite a primeira nota: ")
      leia(nota3[x])

      Escreval("Digite a primeira nota: ")
      leia(nota4[x])

      limpatela

      media[x] <- (nota1[x]+nota2[x]+nota3[x]+nota4[x])/4


      se media[x]>=7 entao
         escreval(alunos[x],"foi aprovado")
         escreval(media[x])
      senao
         escreval("aluno deverá fazer o exame")
         Escreval("digite a nota do exame")
         leia (nota_exame[x])
      fimse


      media_final[x] <- media[x]((nota_exame[x]*4)+(media_ano[x]*6))/10


      se media_final[x]>5 entao
         escreva (alunos[x], " aprovado " )
         escreva (media[x])
      senao
         escreval (alunos[x], "aprovado ")
         escreval (media[x])
      fimse
   fimpara
   limpatela

    escreval ( " Nome  :  N1    N2    N3   N4    MEDIA  SITUAÇÃO")
    
    para x de 1 ate qtd_alunos faca
    
    escreva (alunos[x] , "-" , nota1[x] , "-" , nota2[x] , "-" , nota3[x] , "-", nota4[x] , "-", media_final[x])
    se media_final[x]>=7 entao
    escreval(" aluno aprovado ")
    senao
    escreval(" Aluno reprovado ")
    fimse
   fimpara

Fimalgoritmo
