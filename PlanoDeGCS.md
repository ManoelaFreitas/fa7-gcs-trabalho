<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão 1.1
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|13/12/2014 | 1.0 | Versão inicial. | Thaís de Almeida |
|14/12/2014 | 1.1 | Inclusão de Seção 4. | Thaís de Almeida |
|14/12/2014 |1.2  |Inclusão das Seções 1.1 , 3.2.2 e 5.|Manoela Freitas|



1. Introdução
==============

_[A introdução do Plano de Gerenciamento de Configuração  oferece uma visão geral de todo o documento. 
Ela inclui a finalidade, o escopo, as definições, os acrônimos, as abreviações, as referências e uma visão geral deste
Plano de Gerenciamento de Configuração.]_

1.1 Finalidade
---------------
Este documento tem o objetivo de descrever o plano de Gestão de Configuração e Mudança para o estabelecimento da configuração do projeto Biblioteca.

1.2 Escopo
----------
_[Uma breve descrição do escopo deste Plano de Gerenciamento de Configuração; o modelo ao qual ele está associado e tudo o que é afetado ou influenciado por este documento.]_

1.3 Definições, Acrônimos e Abreviações
---------------------------------------
_[Esta subseção apresenta as definições de todos os termos, acrônimos e abreviações necessários para a correta interpretação do Plano de Gerenciamento de Configuração.  Essas informações podem ser fornecidas mediante referência ao Glossário do projeto.]_

1.4 Referências
---------------

Não se aplica.

1.5 Visão Geral
---------------
_[Esta subseção descreve o conteúdo restante do Plano de Gerenciamento de Configuração e explica como o documento está organizado.]_



2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------
_[Descreva quem será o responsável pela execução das diversas atividades de Gerenciamento de Configuração (CM) descritas no Processo de CM.]_

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------
_[Descreva o ambiente de computação e as ferramentas de software a serem utilizadas para desempenhar as funções de CM em todo o ciclo de vida do projeto ou produto._
_Descreva as ferramentas e os procedimentos necessários utilizados para o controle de versão dos itens de configuração gerados no ciclo de vida do projeto ou produto._
_As questões envolvidas na configuração do ambiente de CM incluem:_
* _tamanho previsto dos dados do produto_
* _distribuição da equipe do produto_
* _localização física dos servidores e clientes]_
 


3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------
_[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]_

### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|_&lt;grupo de itens de configuração&gt;_|_&lt;nome do responsável&gt;_|_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|


### 3.1.3 Baselines do Projeto

_[As baselines funcionam como um padrão oficial no qual os trabalhos subseqüentes são baseados. Somente mudanças autorizadas podem ser efetuadas nas baselines._
_Descreva em que pontos do ciclo de vida do projeto ou produto as baselines devem ser estabelecidas. As baselines mais comuns devem ser definidas ao final de cada uma das fases de Iniciação, Elaboração, Construção e Transição. Elas também podem ser geradas no final de iterações ocorridas dentro das várias fases ou com freqüência ainda maior._
_Descreva quem autoriza uma baseline e o que ela contém.]_

### 3.1.4 Estrutura do Repositório de Versões
_[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]_

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança
Seguindo os valores ágeis, mudanças são bem-vindas e aceitas até mesmo em um estado tardio do projeto. Logo, para que isso seja alcançado, o processo de mudanças deve ser simples. 

Assim que uma mudança é solicitada, o time, em uma rápida reunião com o Product Owner, analisam a solicitação de mudança, podendo ser aprovada ou não, e, sendo aprovada, decidem em que provável momento ela será feita.

O registro de solicitações de mudanças deve ser feito através do JIRA. 

O fluxo e os estados estão representados na imagem abaixo:  
 

![Fluxo de Solicitações de Mudanças](https://github.com/thaisdealmeida/fa7-gcs-trabalho/blob/Thais/Fluxo%20-%20Solicita%C3%A7%C3%A3o%20de%20Mudan%C3%A7a.png)

Os possíveis estados para uma mudança estão especificados na tabela abaixo:

| Estado | Descrição |
|-----------|-----------|
| Nova | A solicitação de mudança foi criada. |
| Em Análise | A solicitação está sendo analisada pelo time e pelo Product Owner, caso seja necessário. |
| Recusada | A solicitação foi recusada. |
| Aprovada | A solicitação foi aprovada. |
| Em Desenvolvimento | A mudança está sendo implementada pela equipe de desenvolvedores. |
| Em Teste | A mudança está na fase de testes do desenvolvedor ou da equipe de testes. |
| Desenvolvido | Os desenvolvedores terminaram de implementar a mudança e já pode passar para a equipe de testes. |
| Finalizado | A mudança já pode ser entregue ao cliente. |


### 3.2.2 Comitê de Controle de Mudança (CCB)
O CCB é responsável pela aprovação das solicitações de mudança para que sejam incorporadas ao produto através da alteração de uma baseline. Segundo a hierarquia institucional do CCB, o CCB Item será formado pelos responsáveis de cada item de configuração afetado pela solicitação de mudança. O CCB tem como participantes:

| Participantes |
|-----------|
|Coordenador do Projeto|
|Líder de Configuração|


4. Padrões e Procedimentos
==========================
Essa seção destina-se a apresentar os padrões que serão utilizados no projeto. Os padrões devem ser seguidos e qualquer melhoria deve ser informada a todo o time e partes interessadas, a saber, equipe de gerência de configuração e equipe de auditoria de processos, para que possa ser discutida e, talvez, implantada. 

4.1 Identificação de documentos do projeto
--------------------------------------

Os documentos relacionados ao projeto devem seguir um padrão, que deve ser simples. 

A descrição formal deve ser:

(NOME_DO_PROJETO)_(DESCRICAO_SUCINTA_DO_DOCUMENTO)

Ex: Isis_Documento_Visao.doc

Mais uma vez, o padrão pode ser alterado de acordo com a necessidade do projeto.

4.2 Nomenclatura de Branchs
--------------------------------------

A nomenclatura de branchs deve ser bem explícita para que seja possível uma rápida identificação da sua necessidade. Caso identifique-se a impossibilidade de nomeá-lo dessa forma, pode-se usar o código da atividade, gerado pelo JIRA, como nome. 

A descrição formal deve ser:

(MOTIVO_BRANCH)

ou

<CÓDIGO_JIRA>

Ex: mudancaDeFramework OU FM-42

4.3 Versionamento
--------------------------------------

Códigos de versionamento só devem ser usados nos documentos e códigos isolados quando necessários. A ferramenta usada para versionamento, o Git, é suficiente para guardar todo o histórico dos arquivos. Caso haja necessidade explícita de inserir códigos de versionamento nos documentos, o padrão é o que se segue:

(CodVersao).(CodMajor).(CodMinor)

CodVersao - Versão geral do sistema/documento, ditadas por grandes releases;
CodMajor - Código atualizado entre os releases, sempre que há uma nova feature, esse código é atualizado;
CodMinor - Código atualizado com bugfixes.

Os códigos de versionamento são gerados automaticamente por scripts criados pela equipe de configuração. 

Ex: Isis_Documento_Visao_3.11.1.doc

4.4 Tags
--------------------------------------

As tags devem seguir um padrão que também pode mudar caso o time e/ou equipe de configuração sinta necessidade. Tags devem ser marcas entregáveis, logo, deve-se gerar uma tag sempre que qualquer feature for implantada no cliente. Bugfixes não necessitam de tags. 

O padrão é o seguinte:

(IDENTIFICADOR)_(VERSAO)

Ex: EntregaRequisitos_1.0

5. Treinamento e Recursos
=========================

| Treinamento | Objetivo | Público Alvo |
|-----------|-----------|-----------|
| Repositório | Ensina como acessar o repositório através de uma máquina cliente, como dar os comandos principais do repositório,  como incluir novos itens dentro do repositório e também como remover do mesmo.| Toda a Equipe.|



6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
