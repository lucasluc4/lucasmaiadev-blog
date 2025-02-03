+++
date = '2025-02-02T18:37:04-03:00'
draft = false
title = 'Principais Conceitos da Meu Bolso'
image = 'mike-hindle-OIAIVrlH2lg-unsplash.jpg'
+++

# Sobre o que é este artigo

Esse artigo vai explicar alguns conceitos importantes usados pelo Meu Bolso para o cálculo de contabilidade. Saber isso é útil principalmente para ganhar liberdade sobre como proceder em situações não previstas no tutorial, que pode ser acessado [clicando aqui](https://lucasmaia.dev/post/meu-bolso-primeiros-passos). Se você quer um passo a passo de como usar o sistema, o artigo de tutorial é de fato mais indicado para esse fim.

# As principais entidades explicadas

Vou dividir a explicação dos principais conceitos por entidade. Em cada uma das próximas sessões, vou explicar a fundo sua principal teoria e como isso afeta o cálculo final de contabilidade.

## Contabilidade

A contabilidade é o produto final desejado ao incluir todos os patrimônios e movimentações do período. A contabilidade é dividida por período (mês e ano) e considera todas as movimentações, patrimônios e transações nos cofrinhos cadastradas para o mesmo período, assim como a contabilidade do período anterior, para o seu cálculo. Toda vez que uma contabilidade de um mês anterior é alterada, por conta da adição de uma nova movimentação, patrimônio, ou mudanças nos cofrinhos, todas as contabilidades seguintes existentes são automaticamente recalculadas. Os valores calculados na contabilidade são:

- Patrimônio total líquido: esse valor é calculado como a soma de todos os patrimônios cadastrados para esse período, menos o saldo nos cofrinhos de compra. Esse é o valor considerado para calcular a economia;
- Patrimônio total: é o valor da soma total de todos os patrimônios cadastrados;
- Patrimônio em investimento: é o valor da total total de todos os patrimônios cadastrados em contas de investimento. Esse é o valor utilizado para calcular a porcentagem de juros e dividendos do período;
- Receita sem juros: é o somatório de todas as transações cadastradas como salário ou bônus;
- Economia líquida: a economia líquida é calculada pela diferença entre o patrimônio total líquido do mês atual e do mês anterior, descontados os ganhos passivos do período;
- Juros e dividendos: é o somatório de todos os ganhos passivos calculados para todas as contas de investimento. Esses ganhos passivos são calculados conta a conta usando a diferença de saldo entre o mês atual e o anterior, considerando todas as transações realizadas. Isso é melhor explicado na sessão sobre contas de investimento. O valor em porcentagem é calculado dividindo o valor bruto dos juros e o valor total do patrimônio em investimento daquele mês;
- Total na conta de compras: valor do somatório do saldo anterior no cofrinho de compras com as transações no cofrinho do mês atual.

## Contas

Contas servem para representar qualquer coisa usada para guardar dinheiro na vida real, e que você tem interesse de rastrear. Isso inclui contas bancárias, contas em corretoras de investimento, carteiras digitais, ou mesmo algum dinheiro em papel guardado em casa. Você pode optar por acompanhar seu FGTS, também, por exemplo, mas não recomendo acompanhar contas cuja maior parte do montante vai ser usado em algum futuro breve para compra de algo. Você pode optar por criar uma conta para representar um patrimônio não-financeiro, como um imóvel, embora não exista um tipo específico para mapear esse tipo de coisa ainda na aplicação.

Cada montante de dinheiro seu deve ser cadastrado em apenas uma conta. Por exemplo, quando você investe em tesouro direto, esse saldo pode ser visualizado na conta atrelada a corretora e diretamente no site da B3. Você deve considerar cadastrar apenas uma dessas contas na aplicação, e eu fortemente sugiro cadastrar apenas o saldo da corretora. Cadastrar os dois montantes vai fazer com que esse dinheiro seja contado duas vezes durante o cálculo da contabilidade.

### Contas ativas e inativas

A habilidade de ativar ou desativar contas pode ajudar na organização da contabilidade, já que contas inativas não aparecem como opção no momento do cadastro de novas movimentações ou patrimônios. Contudo, mesmo que uma conta esteja inativa, ela vai continuar sendo usada para o cálculo de contabilidade, desde que exista algum montante registrado naquele período.

### Contas de depósito

Contas de depósito são contas que **não** possuem um rendimento passivo significativo atrelado a elas. Não é necessário cadastrar depósitos e retiradas para contas de depósito já que a diferença de valor do mês atual para o mês anterior é usado para calcular a diferença entre depósitos e retiradas que foram realizados em contas de depósito. Mesmo que uma conta possua algum tipo de rendimento, se esse rendimento não for significativo, vale considerar cadastrar essa conta como de depósito para evitar a necessidade de cadastrar todas as movimentações.

Por exemplo:

Se eu tinha uma conta com 1000 reais e fiz uma retirada de 500 reais, depois fiz um depósito de 700, no fim do mês, na aplicação eu vou cadastrar a conta com um saldo de 1200. O sistema vai calcular que foi feito um depósito de 200 reais, o que é suficiente pra todos os efeitos práticos.

### Contas de investimento

Contas de investimento são contas que possuem algum rendimento passivo. Contas em corretoras deveriam ser cadastradas como contas de investimento. Não é necessário cadastrar cada novo investimento individual realizado nessa corretora, ou cada investimento que venceu no período, desde que o dinheiro permaneça na corretora, já que o cálculo de contabilidade está mais interessado no montante final acumulado. Para que a aplicação consiga calcular corretamente o valor passivo de ganho, para essas contas é necessário registrar todas as retiradas e depósitos realizados. Com esses valores registrados e o valor de saldo no mês anterior dessa conta, conseguimos calcular o valor esperado no fim de cada mês. Qualquer diferença entre o valor esperado e o valor real é considerado uma flutuação dos investimentos e é usado para calcular o ganho passivo total da carteira.

Por exemplo:

Se eu tinha uma conta com 1000 reais, e um investimento de 200 reais venceu. Desses 200 reais, 100 eu movi para uma outra conta e 100 eu reinvesti ou mantive na corretora para reinvestir no futuro, então eu preciso cadastrar na plataforma uma retirada de 100 reais. No fim do mês, a aplicação espera que eu tenha 900 nessa conta. Se eu cadastro um valor de 950 como saldo, o sistema calcula que esses 50 reais foram um rendimento passivo.

## Patrimônio

Para cada conta cadastrada, é importante cadastrar o patrimônio associado a essa conta para cada novo período, que é basicamente o seu saldo final no mês. Se uma conta possuía um saldo no mês anterior e nenhum saldo é cadastrado para o mês corrente, então o saldo é considerado como zero. Nesse caso, pode acontecer um decréscimo significativo no patrimônio líquido e total calculados.

## Transações

Existem quatro tipo de transações que precisam ser cadastradas: salários e bônus do mês, e depósitos e retiradas em contas de investimento. Salários e bônus são associados a uma conta, mas essa associação não afeta o cálculo de contabilidade, já que o valor da receita total é calculada somando o total de transações de salário e bônus independentemente da conta, mas recomendo associar sempre a contas de depósito. O tipo de transação, seja bônus ou salário, também não afeta o cálculo final de receita.

Depósitos e retiradas em contas de investimento precisam ser cadastradas para que a aplicação calcule corretamente os juros e dividendos do mês. Sem nenhuma transação desse tipo cadastrada, o sistema vai entender que a diferença de saldo de um mês para o outro é totalmente devido a flutuações de investimentos. Caso o dinheiro não saia da conta da corretora, por exemplo, se um rendimento vence, mas o dinheiro não é retirado ou é reinvestido em outro ativo na mesma corretora, não é necessário cadastrar transações. Se você fez uma retirada e um depósito em uma conta de investimento, você pode optar por cadastrar apenas uma transação com a diferença entre os dois valores. Será uma transação de retirada se foi retirado mais dinheiro do que foi depositado, ou uma transação de depósito se foi depositado mais dinheiro do que foi retirado.

## Cofrinho de compras

Às vezes, fazemos compras grandes que precisamos guardar dinheiro por alguns meses para conseguir juntar o valor, sem afetar nossas metas de economia. Imagine o cenário que você tem uma conta com 1000 reais e tem a meta de economizar 100 reais por mês. No primeiro mês, você consegue economizar 150 reais, e o valor do saldo da sua conta vai para 1150, e você cumpre a meta, mas já que 50 reais a mais foram economizados, você quer usar esse dinheiro no futuro para comprar algo. No segundo mês, você consegue economizar novamente 150 reais, mas decide gastar os 50 reais sobressalentes junto com os 50 do mês anterior para fazer uma compra de 100 reais. No fim do mês, você vai ter um saldo de 1200 reais (1150 do mês anterior, mais 150 de economiza, menos 100 reais da compra), e o sistema vai entender que você economizou apenas 50 reais, e descumpriu a meta, apesar disso não ser verdade, já que em dois meses você economizou 200 reais.

Os cofrinhos servem para ajustar esse tipo de cenário. Se em algum mês você conseguiu economizar algum valor extra e planeja usar esse valor no futuro para uma compra maior, juntando com economias de outros meses, você deve adicionar esse valor extra no cofrinho, para que isso não afete o cálculo de economia no mês que você finalmente fizer a compra.

# Próximos passos

Caso ainda tenha dúvida em algum conceito, ler o nosso [artigo de tutorial passo a passo](https://lucasmaia.dev/post/meu-bolso-primeiros-passos) pode ajudar, mas, se mesmo assim isso não for suficiente, deixe um comentário para que eu possa pessoalmente ajudar, ou talvez a própria comunidade vá ao seu auxílio.

Se perceber algum tipo de comportamento inesperado, pode ser que isso seja uma falha da aplicação. Você pode me ajudar reportando esses problemas nos comentários para que eu possa analisar assim que possível. Nesses casos, capturas de tela podem ser muito valiosas, apesar delas não poderem ser anexadas nos comentários.

Obrigado e boas economias!

# Imagem de capa

A foto de capa é de [Mike Hindle](https://unsplash.com/@mikehindle) e está disponível no [Unsplash](https://unsplash.com/photos/a-black-and-white-photo-of-a-square-object-OIAIVrlH2lg)
