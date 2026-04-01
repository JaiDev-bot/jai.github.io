---
title: "Buzz Lightyear não quer mais escalar até a nuvem: sobre a repatriação de dados."
date: 2026-01-20 08:00:00 -0300
categories: [Cloud]
tags: [Azure,Cloud,AWS,GCP,Data-Repatriation]
---



![Buzz Lightyear](/assets/imagens/20-01-2026-Buzz.jpg)


# Análise: repatriação de dados

**Referência:** Baseado nos artigos ["Why we are leaving the cloud"](https://world.hey.com/dhh/why-we-are-leaving-the-cloud-60434b27) e ["Cloud Exit"](https://basecamp.com/cloud-exit), de **David Heinemeier Hansson (DHH)**, criador do Ruby on Rails e CTO da 37signals.

> "We left the cloud. 
> 
> They promised the cloud would be cheaper, faster, and easier. For us, the savings never materialized and the team never shrunk."



### 1. A promessa vs. realidade

A computação em nuvem foi vendida como serviços de computação sob demanda, com capacidades exorbitantes de agilidade, disponibilidade e redução de custos; algo que inicialmente foi uma inovação para a sociedade, algo que resolveria problemas e mudaria nossa forma de enxergar a tecnologia e a internet. Os provedores de nuvem vendem, principalmente, a ideia de que a nuvem é mais barata em comparação ao **on-premise**, tendo até ferramentas de cálculo para analisar a diferença de custos entre ter sua própria infraestrutura na empresa e ter um servidor alugado na nuvem. Mas será mesmo que essas ferramentas servem para mostrar a diferença de custo total ou focam apenas em pontos específicos para o cliente se maravilhar e, por consequência, entrar em uma teia de Vendor Lock-in? Mas não nos limitemos a tão somente custos, a pergunta também pode emergir do espectro técnico e das necessidades de negócio. 

### 2. A Armadilha do OpEx


O marketing da nuvem foca no baixo custo de entrada, mas omite a inflação do crescimento. Para a 37signals, a conta não fechava mais: pagar um "aluguel" perpétuo por recursos que rodam 24/7 tornou-se financeiramente irracional. Quando a carga de trabalho é previsível e estável, o modelo de serviços sob demanda deixa de ser uma vantagem e passa a ser um imposto sobre a escala.

A análise técnica de DHH revela que a promessa de "times menores" é uma falácia. Gerenciar a complexidade de arquiteturas cloud-native exige especialistas tão caros e numerosos quanto os que gerenciam hardware físico, com a desvantagem de que, na nuvem, você gasta energia lutando contra a infraestrutura de terceiros para otimizar faturas.

### 3. Eficiência arquitetural
A decisão de DHH não foi um saudosismo ao hardware, mas uma análise de eficiência de throughput. Na nuvem, camadas de abstração e virtualização (Hypervisors) introduzem uma latência inerente e o risco de contenção de recursos por "noisy neighbors". Ao repatriar para o Bare Metal, a 37signals eliminou essas camadas, garantindo acesso direto aos ciclos de CPU e barramentos NVMe.

### 4. Conclusão
A computação em nuvem continua sendo uma ferramenta excepcional para startups e projetos de escala incerta. No entanto, o movimento de saída liderado pela 37signals serve como um alerta para a maturidade técnica: a nuvem deve ser um meio, não um destino final obrigatório.

Para empresas com tráfego consolidado e previsível, a repatriação de dados representa a retomada do controle financeiro e tecnológico. No fim do dia, a pergunta não é se a nuvem é melhor, mas sim em qual momento o custo da conveniência supera o valor da sua independência.



**Afinal, a sua empresa realmente precisa da nuvem?**


