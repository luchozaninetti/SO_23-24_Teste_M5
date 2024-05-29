# Teste de Sistemas Operativos - Módulo 5

Faz *fork* do repositório para teres a tua cópia.

Preenche o ficheiro README diretamente no GitHub. A partir da página principal do repositório, clica em "Edit File" (ícone representando um lápis).

Escreve as respostas dentro dos blocos correspondentes. Substitui as reticências pelo que é pedido em cada pergunta. Não desformates o documento.

Quando acabares, carrega no botão "Commit Changes".

## Informação do aluno

    Nome: Luis Fernando Zaninetti

## P1 - Para as seguintes questões, assinala a opção correta: (2.5v)

  1. Que comando é usado para definir permissões de execução num script Bash?

    A) chmod +x script.sh
    B) chmod -x script.sh
    C) chmod +r script.sh
    D) chmod -r script.sh
    
    Resposta: A

  2. Como se define um comentário num script Bash?

    A) // comentário
    B) /* comentário */
    C) # comentário
    D) -- comentário
    
    Resposta: C
   
  3. Que comando é usado para adicionar uma linha de texto ao final de um arquivo em Bash?

    A) echo "texto" > arquivo
    B) echo "texto" < arquivo
    C) echo "texto" | arquivo
    D) echo "texto" >> arquivo
    
    Resposta: D

  4. Qual é o comando usado para ler a entrada do utilizador num script Bash?

    A) read
    B) input
    C) get
    D) scan
    
    Resposta: A

  5. Que símbolo é usado para denotar uma variável em Bash?

    A) %
    B) $
    C) &
    D) #
    
    Resposta: B

## P2 - Escreve scripts em Bash para realizar as seguintes instruções: (7.5v)

  1. Exibir a mensagem "Olá, Mundo!" no terminal.

    Resposta:
    #!/bin/bash
    echo "Olá, Mundo!"
    
  2. Receber dois números como entrada, e exibir a soma dos dois.
     
    Resposta:
    #!/bin/bash
    Echo "Introduza um número"
    read num1
    Echo "Intruduza outro numero"
    read num2
    soma=$((num1 + num2))
    echo "A soma de $num1 e $num2 é: $soma"



  3. Ler um valor numérico e imprimir uma mensagem a informar se o mesmo é par ou ímpar.

    Resposta:
    #!/bin/bash
    Echo "Introduza um número"
    read num
    if [ $((num % 2)) -eq 0 ]; then
    echo "O número $numero é par."
    else
    echo "O número $numero é ímpar."
    fi

## P3 - Indica o que é realizado pelas seguintes instruções: (6v)

  1. 
    
    echo "scale=2;22/7" | bc

    Resposta:
    Defini o número de casas decimais no resultado
     
  2. 
    
    #!/bin/bash
    sum=0
    for i in {1..5}
    do
      sum=$((sum + i))
    done
    echo "A soma dos números de 1 a 5 é $sum."


    Resposta:
    Realiza a soma dos números de 1 a 5 e imprime o resultado

  3. 
    
    #!/bin/bash
    num=10
    while [ $num -gt 0 ]
    do
      echo "Número: $num"
      ((num--))
    done

    Resposta:
    Esse script faz um ciclo que a cada volta o numero é subtraido 1 e envia o numero para fora, esse ciclo continua até que o numero (10) chegue a 0

## P4 - Realiza os seguintes exercícios, com respostas detalhadas: (4v)

  1. O que é um **shebang** (#!) e qual é a sua função num script?

    Resposta:
    Um shebang é uma sequência de dois caracteres usada em scripts para indicar qual interpretador de comandos deve ser usado para executar o script. Essa linha deve aparecer na             primeira linha de um script.

  2. Como se utiliza a instrução 'if-else' num script Bash? Escreve um exemplo simples.

    Resposta:
    
    A instrução if-else em um script Bash é usada para executar diferentes blocos de código dependendo se uma condição é verdadeira ou falsa
    #!/bin/bash
    idade=20
    if [ $idade -ge 18 ]; then
    echo "Você é maior de idade."
    else
    echo "Você é menor de idade."
    fi

