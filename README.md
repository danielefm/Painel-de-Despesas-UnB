# Painel-de-Despesas-UnB

**Este projeto ainda está em desenvolvimento**

## 1. Sobre o projeto

Este projeto surgiu como uma *sidetask* da minha atuação profissional na Universidade de Brasília. Atualmente, sou servidora da Universidade, trabalhando no setor de Infraestrutura, Obras e Licitações. Parte das atribuições do meu setor envolvem a definição de quais as obras prioritárias para serem executadas em determinado ano fiscal. Entretanto, essas decisões são quase completamente subjetivas, e nem sempre atendem às reais necessidades da Universidade.

Com o objetivo de orientar a dados a tomada de decisão sobre investimento público, comecei a desenvolver esse painel de despesas da Universidade de Brasília. Meus objetivos específicos incluem:

1. Identificar quais os principais gastos da UnB, tanto em um ano 'padrão' (2019), quanto em um ano afetado pela pandemia '2020'
2. Planejar investimentos em Infraestrutura que potencialmente reduziriam esses gastos principais (ex.: se eu identificar que o gasto com energia elétrica é significativo, posso verificar a viabilidade de investimentos em projetos de eficiência energética, como instalação de placas solares)

## 2. Conclusões parciais

### 2.1 Obtenção de dados

Verifiquei que existiam duas formas para obter os dados do Portal da Transparência: acessando a [API de Dados](http://www.portaldatransparencia.gov.br/api-de-dados) ou fazendo o download de arquivos CSV no [site](http://www.portaldatransparencia.gov.br/despesas/lista-consultas) disponibilizado pelo Governo Federal.

Entretanto, percebi que os dados obtidos por cada uma dessas vias eram diferentes. No notebook [comparacao-API-csv.ipynb](https://github.com/danielefm/Painel-de-Despesas-UnB/blob/main/comparacao-API-csv.ipynb) eu faço essa comparação e verifico que os dados obtidos pela API têm classificações genéricas, como ação governamental 'Múltipla', destino 'Múltiplo', além de várias informações faltantes. Já os dados obtidos pelo download de CSVs são mais consolidados e não têm dados faltantes, o que me faz concluir que sejam melhores para a avaliação que quero fazer.

Um roteiro de como os dados foram obtidos via API consta no notebook [obtencao-de-dados-API.ipynb](https://github.com/danielefm/Painel-de-Despesas-UnB/blob/main/obtencao-de-dados-API.ipynb).