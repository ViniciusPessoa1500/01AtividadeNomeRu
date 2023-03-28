# 01AtividadeNomeRu
Atividade nome + nota + Ru
inserirDados = int(input('Iniciar programa: 0-não   1-sim: '))
##primeiramente declaramos uma variável inserir dados do tipo inteiro, imputando a frase opção sim e não.
novamente = 1
##quando for verdadeiro declaramos novamente com a opção 1.
while (novamente == 1):
##aqui no while fazemos amarração do novamente trazendo a diferença entre o-não e 1-sim com ==.
    if inserirDados == 1:
        nomeAluno = str(input('digite o nome do aluno: '))
##neste if    sendo sim verdadeiro prosegue com o nome aluno.
    if inserirDados == 1:
        notaFinal = float(input('digite o valor da nota: '))
        notaStr = str(notaFinal)
##em seguida o if traz o float converte um número armazenado em uma string ou inteiro em um número de ponto flutuante,
##ou um número com um ponto decimal. sendo assim o valor nota final.
    if ((notaFinal <0) or ( notaFinal>10)):
        print("Nota invalida!")
        novamente = int(input('Iniciar programa novamente: 0-não   1-sim: '))
##trazendo a nota, se for falso ou inválida retorna novamente o menu.
    elif notaFinal <= 2.9:
        print( " o aluno "+ nomeAluno + " tirou a nota "+ notaStr+ " se enquadra no conceito E")
    elif ((notaFinal >= 3.0) and (notaFinal <= 4.9)):
        print(" o aluno " + nomeAluno + " tirou a nota " + notaStr+" se enquadra no conceito D")
    elif ((notaFinal >= 5.0) and (notaFinal <= 6.9)):
        print("o aluno " + nomeAluno + " tirou a nota " + notaStr+ " se enquadra no conceito C")
    elif ((notaFinal >= 7.0) and (notaFinal <= 8.9)):
        print(" o aluno " + nomeAluno + " tirou a nota " + notaStr+ " se enquadra no conceito B")
    else:
        print(" o aluno " + nomeAluno + " tirou a nota " + notaStr+  " se enquadra no conceito A")
    novamente = int(input('Iniciar programa novamente: 0-não   1-sim: '))
    if novamente != 1:
        break
##no elif esta declarada todas a notas segundo o exercício, quando for falso ela le a proxima nota, se for verdadeiro
##ela traz a nota para o print, enquadrando no conceito declarado.
##noif novamente se for != pede para retornar ao menu ou finalizar o programa.
##break serve para parar de rodar.

