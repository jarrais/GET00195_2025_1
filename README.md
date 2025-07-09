# Apresentação

Este repositório apresenta a implementação de um conjunto de **indicadores educacionais** elaborados a partir dos microdados do **Censo Escolar 2024**, com foco nos **municípios do Estado do Rio de Janeiro**.

O objetivo central deste trabalho é oferecer uma visão detalhada da realidade educacional nos municípios fluminenses, contribuindo para o **monitoramento**, **avaliação** e **planejamento de políticas públicas** voltadas à educação básica.

# Visão Geral

O projeto foi desenvolvido no âmbito da disciplina **GET00195 – Prática Estatística I**, no semestre **2025/1**, da **Universidade Federal Fluminense (UFF)**, sob a orientação do professor **Jony Arrais**.

Os dados utilizados são oriundos do [Censo Escolar 2024 - INEP](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/censo-escolar), organizado pelo **Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (INEP)**.

A construção dos indicadores envolveu duas etapas principais:

1. **Definição metodológica** — com a formalização dos indicadores por meio de expressões matemáticas;
2. **Implementação computacional** — com a aplicação de scripts em **R** sobre os microdados originais.

Foram consideradas **apenas as escolas situadas no estado do Rio de Janeiro**, em funcionamento e com pelo menos uma matrícula na educação básica.

# Indicadores Produzidos

Ao todo, foram construídos **41 indicadores**, calculados por município, abordando os seguintes aspectos:

- **Acessibilidade**: banheiros acessíveis para pessoas com necessidades especiais, salas adaptadas, sinalização visual, etc.;
- **Infraestrutura**: biblioteca, quadra esportiva, laboratório, climatização, saneamento;
- **Inclusão**: salas para atendimento educacional especializado, profissionais de saúde, psicólogos(as), nutricionistas;
- **Tecnologia**: internet, computadores, banda larga;
- **Organização escolar**: grêmio estudantil, alimentação, reciclagem;
- **Tipologia das escolas**: públicas/privadas, zona urbana/rural, entre outras.

Os indicadores foram calculados por município, sendo alguns segmentados por **dependência administrativa** (federal, estadual, municipal e privada).

Para detalhes técnicos e fórmulas matemáticas, consulte o documento:

Texto_Final_Indicadores_Educacionais_2025_1.pdf

# Estrutura do Repositório

O repositório contém os seguintes arquivos principais:

- `script_indicadores.R` — script completo em R com a limpeza, filtragem e cálculo dos indicadores;
- `base_final.xlsx` — planilha final contendo os indicadores agregados por município;
- `Texto_Final_Indicadores_Educacionais_2025_1.pdf` — documentação com as fórmulas e explicações técnicas;
- `microdados_censo_2024.csv` — base de dados original (recomenda-se baixar direto do INEP, devido ao tamanho).

# Ferramentas Utilizadas

O projeto foi desenvolvido inteiramente em **linguagem R**, com uso dos seguintes pacotes:

- dplyr
- readr
- tidyr
- naniar
- writexl

# Participantes

Este projeto foi realizado por estudantes da disciplina **GET00195 – Prática Estatística I** do curso de **Estatística da Universidade Federal Fluminense (UFF)**, turma 2025/1:

- ANA LUIZA KOCH PORTO
- ANDRE MORENO RIBEIRO GOMES
- BEATRIZ FRANCO DE FREITAS
- BRUNO OLIVEIRA ALVES DOS SANTOS
- DANIEL MARTINS DE FARIA
- DAVI LUCAS DE JESUS CAETANO
- EDERSON MACEDO DE CARVALHO MORAES
- FELIPE MAIA RODRIGUES DE MIRANDA
- FERNANDA ALEXANDRINA DOS SANTOS
- FERNANDO LUCAS SANTOS DE OLIVEIRA
- FILIPE DE CARVALHO SANT ANNA
- GABRIEL LUIS ALVES GONCALVES DE SOUZA
- GABRIEL VIEIRA RABELO
- GUSTAVO DE SANSON KOVACS
- GUSTAVO MEDEIROS MARINHO DE LIMA
- ILIDIO DO NASCIMENTO ALVES JUNIOR
- JOAO PEDRO SANTOS MACHADO
- JOAO VITOR NEVES PEREIRA
- JOAO VITOR PIMENTEL HANNIG
- KIANE SASSAKI MENEZES
- LORENA NEIVA TORRES
- LUCAS GOMES CRUD
- LUCAS RODRIGO DE MOURA ARAGÃO
- MARCELO RIBEIRO DE CASTRO ROCHA
- MATHEUS DE SOUZA DA SILVA
- MILENA BRANCO LABRE DE OLIVEIRA RODRIGUES
- OLGA GUIMARAES GRICHTCHOUK
- PAOLLA PINHEIRO PACHECO
- PATRICK DOS REIS DIAS
- PAULO HENRIQUE MARTINEZ MACHADO
- PAULO VICTOR ZAVA PEREIRA
- PEDRO AUGUSTO MENEZES ROCHA
- PEDRO TRUPPEL DUARTE XAVIER
- RENATO GUIMARAES GUERREIRO
- RICARDO AUGUSTO FIGUEIREDO DE OLIVEIRA
- THAIS NASCIMENTO DE OLIVEIRA RABELLO
- THIAGO DE OLIVEIRA SENRA
  

Orientação: **Prof. Jony Arrais**


# Como Reproduzir os Resultados

Para gerar os indicadores a partir dos microdados do Censo Escolar 2024, siga os passos abaixo:

1. **Baixe os microdados** diretamente do site do INEP:  
   [Download do Censo Escolar 2024 (INEP)](https://download.inep.gov.br/dados_abertos/microdados_censo_escolar_2024.zip)

2. **Extraia os arquivos** `.csv` do ZIP e salve no mesmo diretório onde está o script `script_indicadores.R`.

3. **Abra o RStudio** (ou outro ambiente compatível com R).

4. Execute o script `script_indicadores.R` para processar os dados.

5. Ao final, será gerada a planilha `base_final.xlsx` com os indicadores agregados por município para o Estado do Rio de Janeiro.

