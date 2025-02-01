+++
date = '2025-01-26T17:54:56-03:00'
draft = false
title = 'A Aplicação Meu Bolso'
+++

Em 2024, eu decidi lançar minha aplicação financeira pessoal de maneira pública, mas por ter sido um ano bem atribulado, principalmente do ponto de vista financeiro, acabei fazendo o lançamento apenas em 2025, depois de ter me dedicado a finalizar uma série de ajustes no código. Lancei faltando terminar alguns, ainda, mas só divulguei depois que fiquei satisfeito com uma versão zero, inicial. A aplicação, com sua versão atual, pode ser acessada em https://meubolso.lucasmaia.dev, e espero que ela possa ajudar você, leitor, assim como tem me ajudado nesses últimos anos.

À medida que eu for lançando novas versões com novas funcionalidades, vou criando novos posts para divulgar e explicar como tudo funciona; e vou adicionar links aqui mesmo, neste artigo, para que isso funcione como um índice para consulta de usuários precisando de ajuda.

# Porque decidi criar uma aplicação?

Até 2018, eu não me preocupava em me organizar financeiramente. Não que eu gastasse de maneira desordenada, mas eu apenas me preocupava se eu não estava gastando mais do que ganhava. Isso porque no geral eu ganhava mais ou menos o suficiente para me manter, e na época meu foco era mais em evoluir na carreira do que economizar dinheiro. Esse cenário mudou em 2018, com um novo emprego e uma remuneração substancialmente maior, e criar metas de economia começou a fazer bastante sentido.

As aplicações de gestão financeira pessoal nunca me satisfizeram, basicamente porque seu foco é geralmente controlar o seu gasto mensal dividido por categoria, para que você possa tomar decisões de corte em despesas. Algumas dessas aplicações inclusive conectam com aplicações bancárias para monitorar seu cartão de crédito e sua conta. Esse não era muito meu foco, porque meu objetivo era basicamente controlar o quanto mensalmente eu estava conseguindo economizar. Eu estabeleci uma meta de quantia de dinheiro que eu planejava guardar mês a mês, e no fim de cada período eu precisava saber se eu tinha atingido o objetivo, ou não. Simples.

O que eu montei na época foi uma planilha no excel com alguns cálculos incorporados, onde eu incluía o valor que eu possuía em cada uma das minhas contas bancárias ou contas de investimento, no fim de cada mês. Essa planilha fazia uma soma e comparava com o somatório do mês anterior, e no final dava o quanto foi essa variação. Esse sistema foi suficiente por bastante tempo, mas tinha um defeito quando falamos de controlar contas de investimento: às vezes eu economizava bastante dinheiro, mas, se as flutuações do valor das minhas aplicações fossem negativas durante o mês, o somatório era puxado para baixo e eu acabava não cumprindo a meta. Ou o contrário: às vezes eu não economizava o suficiente, mas as flutuações positivas dos investimentos faziam com que eu batesse a meta. Isso fez com que eu começasse a pensar em alternativas para fazer um cálculo mais rebuscado. Uma planilha melhorada provavelmente seria suficiente, mas o excel possui uma filosofia muito espacial com suas células, e me faltava conhecimento para fazer algo muito mais elaborado.

Minha segunda alternativa foi o Notion, mas suas base de dados automáticas tem limitações sobre relações, e muita coisa precisa ser feita de maneira manual para funcionar corretamente. O Coda é uma aplicação parecida que dá mais possibilidade de automações, mas o plano grátis possui limitação de linhas que podem ser incluídas. Embora essa limitação ainda fosse bastante permissiva, eu preferi criar as automações de tal maneira que não me deixasse sujeito a uma plataforma paga. No fim, decidi finalmente criar minha própria aplicação, que em suas primeiras versões rodava diretamente no meu computador e exportava algumas informações para o Notion. Utilizei esse programa dessa forma por 2 anos, até que decidi publicá-lo para facilitar a usabilidade e para que outras pessoas pudessem usar, o que me motivaria provavelmente a trabalhar mais fielmente em sua melhoria.

# Para quem essa aplicação pode ser útil?

Se você tem interesse de, de fato, categorizar os seus gastos, para de alguma forma conseguir colocar limites por categoria, existem outras aplicações que são específicas para fazer isso. Eu não tentei ir por esse caminho, pois esse nível de controle nunca foi recompensador para mim. Ao mesmo tempo, se você quiser controlar seus investimentos, para identificar a eficiência da sua carteira, para otimizar retornos, provavelmente também existem aplicações bastante especializadas nesse tipo de coisa. Eu não sou um investidor assíduo, e no geral busco aplicações sem muito risco ou flutuações, então não preciso tanto desse nível de acompanhamento. Sinto que o Meu Bolso tenta resolver problemas mais simples e mais primordiais do que esses.

Essa minha aplicação serve principalmente para três casos:

- Se você tem um plano a longo prazo de aumento de patrimônio e tem interesse em estabelecer uma meta mensal de economia, para garantir seus objetivos estão sendo cumpridos; ou
- Se você quer descobrir quanto seus investimentos tem contribuído, de maneira bruta, para o aumento do seu patrimônio, mês a mês; ou
- Se você possui uma meta de economia mensal para algum objetivo de curto prazo, como uma viagem, ou outra compra pontual, sem perder o rastro do seu patrimônio.

Ter uma meta mensal fácil de calcular me incentivou nos anos passados a economizar mais e a evitar gastos mais supérfluos em busca dessa meta, já que eu me sentia recompensado por isso, o que fez com que meu patrimônio crescesse substancialmente e eu pudesse me organizar financeiramente para alcançar objetivos que antes me pareciam irreais. Ter um tato sobre quanto seu dinheiro tem rendido passivamente também ajuda a investir cada vez mais.

Sinto que controlar gastos, economia e rendimento de maneira mais macro é uma forma muito mais recompensadora, do que micro-gerenciar essas coisas. E suficiente para, por exemplo, começar a calcular um plano de aposentadoria. No fim, o Meu Bolso é sobre recompensar esse esforço de economia e isso nos coloca num ciclo virtuoso para que continuemos seguindo o plano.

# Como o Meu Bolso funciona

 O Meu Bolso funciona de maneira relativamente simples. No fim de cada mês (ou em alguma outra data que ache pertinente, desde que seja sempre no mesmo dia), você precisa visitar cada uma das suas contas bancárias, ou contas em agências financeiras, e incluir na plataforma os valores dos saldos. Você também precisa incluir as suas receitas principais - como o salário. Não é necessário incluir receitas como rendimento de investimentos, já que com o saldo a aplicação já consegue calcular isso automaticamente, mas é necessário incluir as movimentações nessas contas, como novos investimentos ou retiradas. Parece bastante trabalho, mas não é. Mesmo com umas 7 contas a atualizar, eu não demoro mais do que 15 minutos por mês nesse processo.

Cada conta em uma agência dessas precisa ser mapeada para uma conta dentro da plataforma, então é necessário uma configuração inicial que reflita o seu contexto atual. Essas contas cadastradas possuem tipos que ajudam a aplicação a calcular os gastos e rendimentos mais facilmente.

Por fim, você tem acesso a cofrinhos, que servem para reservar parte do dinheiro para alguns objetivos de curto ou médio prazo, como uma viagem, ou uma compra maior que você precisa economizar durante vários meses para conseguir o valor necessário. Esses cofrinhos funcionam como um “pré-gasto”, para que o mês que de fato você realize essa compra não tenha o objetivo sendo erroneamente sobre-impactado, mesmo que esse gasto tenha sido planejado.

Com todas essas inclusões, a ferramenta consegue calcular:

- o seu patrimônio total;
- o quanto seu patrimônio evoluiu de um mês para o outro;
- o quanto dessa evolução foi devido a ganhos passivos e o quanto tem rendido no total sua carteira de investimentos;
- a sua receita total;
- o quanto das suas receitas você conseguiu economizar, em valores absolutos e em porcentagem;
- o quanto você tem reservado em cofrinhos para poder gastar em compras maiores;

Esses valores calculados ficam armazenados em um histórico, e você tem uma idéia de como anda a sua evolução patrimonial mensalmente.

No futuro breve, queremos incluir maneiras de exportar essas informações em formato .csv e para o Notion, para que você possa processar essas informações da forma que quiser.

# Próximos passos

Eu planejo escrever uma série de artigos para explicar o funcionamento da aplicação como um todo, e alguns guias e tutorias de ajuda. Vou adicionar os endereços aqui à medida que conseguir concluí-los.

Por enquanto, o próximo passo é acessar a começar a utilizar a aplicação Meu Bolso disponível em https://meubolso.lucasmaia.dev.