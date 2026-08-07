<h1>Cálculo Estrutural e de Concreto — MVP Funcional</h1>

Este repositório armazena o código-fonte e a documentação do projeto acadêmico de Cálculo Estrutural e Dosagem de Concreto, desenvolvido como um MVP Funcional de suporte à engenharia civil e construção sustentável.

A aplicação permite a modelagem paramétrica básica de elementos de concreto armado, cálculo automático de volumes teóricos e cubagem de insumos construtivos por traços de dosagem regulamentados pelas normas técnicas.

<h3>🛠️ Identificação e Metadados do Projeto</h3>

<b>Desenvolvedora:</b> Eduarda Pereira de Lima

Natureza do Projeto: Documentação Técnica Ilustrada (MVP Funcional)

Sistema Alvo da Pesquisa Primária: Sistema inteligente integrado para cálculo e descrição de calorias baseado em fotografia de comida via Inteligência Artificial.

Aplicação Colateral de Validação (MVP): Calculadora e Dimensionadora Estrutural de Concreto com persistência de dados e download estruturado em formato de planilha Excel (.xlsx).

Data de Emissão: Junho de 2026

Contexto Acadêmico: Curso de Inteligência Artificial Aplicada

<b>Orientador:</b> Prof. Djones Braz de Araujo Costa

Instituição: FAETEC-RJ — Unidade de Cachoeiras de Macacu

<h3>🏗️ O MVP e Conexão de Pesquisa</h3>

A aplicação interativa disponibilizada neste repositório representa o MVP Funcional de validação de fluxo de dados.

O projeto maior estuda a modelagem e estimativa volumétrica de objetos tridimensionais a partir de fotografias bidimensionais (visão computacional). No escopo deste MVP, aplicamos a lógica matemática de determinação tridimensional para a cubicagem de elementos estruturais da construção civil (lajes, sapatas, vigas e pilares), gerando a cubagem quantitativa exata de materiais de construção necessária para o seu preenchimento homogêneo.

Funções Ativas na Aplicação Web:

Seleção do Elemento Estrutural: Customização automática de termos e fórmulas para Lajes, Vigas/Pilares ou Sapatas.

Dimensionamento Dinâmico: Inserção de Comprimento ($L$), Largura ($W$) e Espessura/Altura ($H$) em metros ($m$).

Dosagem de Traços Normatizados: Escolha rápida de traços usuais com fatores água/cimento regulamentados.

Cálculo Físico-Químico de Insumos:

Estimativa de Cimento (kg e número de sacos de 50 kg).

Estimativa de Areia Média/Fina ($m^3$).

Estimativa de Brita 1 ou 2 ($m^3$).

Cálculo exato da água de amassamento (L).

Relatório Acumulado e Notas Técnicas: Adição de descrições e histórico de elementos que acumulam o volume final.

Exportação Direta em Excel (.xlsx): Geração dinâmica e automatizada através de biblioteca em JavaScript (SheetJS) sem necessidade de processamento no servidor (Serverless).

<h3>🚀 Como Executar e Implantar no GitHub Pages</h3>

O projeto foi totalmente projetado de maneira monolítica unificada (HTML, CSS e JS integrados em um único arquivo de distribuição rápida), o que o torna ideal para publicação no GitHub Pages.

Passos para colocar o projeto no ar:

Crie um novo repositório no seu GitHub (ex: calculo-concreto-faetec).

Faça o upload do arquivo index.html e deste README.md na raiz (/) do repositório.

No GitHub, acesse as configurações do repositório (Settings).

No menu lateral esquerdo, clique na seção Pages.

Em Build and deployment, selecione a branch main (ou master) e a pasta raiz / (root).

Clique em Save.

Aguarde alguns instantes e sua aplicação estará online no endereço padrão:
https://<seu-usuario>.github.io/<nome-do-repositorio>/

<h3>🧮 Modelagem Matemática e Teórica de Engenharia</h3>

O cálculo dinâmico da aplicação utiliza o Método IPT de dosagem experimental e rendimento volumétrico. A quantidade de material seco por metro cúbico de concreto é deduzida com base na densidade aparente dos agregados:

$$V_{concreto} = L \cdot W \cdot H$$

Seja a proporção em massa/volume $1 : a : b : \frac{a}{c}$, o volume aparente de mistura seca é dado por:

$$V_{mistura} = \left( 1 + a + b \right)$$

O consumo de cimento por metro cúbico real ($C$) de concreto acabado é modelado aplicando-se o coeficiente de adensamento empírico $k \approx 0.68$:

$$C = \frac{\rho_{cimento} \cdot 1}{k \cdot (1 + a + b)}$$

Onde $\rho_{cimento} = 1400\,kg/m^3$. Acrescenta-se à estimativa final um coeficiente de segurança de perda técnica por transporte e adensamento de $1.10$ ($+10\%$).

<h3>📄 Licença e Uso de Comunidade</h3>

Este projeto é disponibilizado publicamente com propósitos exclusivamente acadêmicos e educacionais. Alunos, professores e pesquisadores da área de Inteligência Artificial, Engenharia Civil e TI estão autorizados a realizar fork, modificação e uso do motor de cálculo de exportação em planilha.

FAETEC-RJ - Unidade de Cachoeiras de Macacu - Junho de 2026.
