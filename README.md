# TRABALHO 01: iMenu - The interactive menu
Trabalho desenvolvido durante a disciplina de Banco de Dados do Integrado

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
Lucas Vinício Alves Almeida: lucasportugal2002@gmail.com<br>
Ricardo Meireles Trindade Pereira: ricarynwa8@gmail.com<br>
[e-mail do grupo: intermenu8@gmail.com]

### 2.INTRODUÇÃO E MOTIVAÇAO<br>

> Nós visamos melhorar a experiência dos clientes nos restaurantes. Sabendo da insatisfação constante dos clientes em alguns estabelecimentos, nosso sistema busca agilizar os pedidos e acelerar o atendimento, evitar erros no pedido dos clientes e promover uma melhor experiência aos fregueses. 
 

### 3.MINI-MUNDO Novo<br>

> O cliente, ao frequentar o restaurante, terá a sua disposição o sistema “iMenu” em um dispositivo Mobile provido pelo próprio restaurante. Ao acessar o sistema, o cliente poderá escolher o tipo de refeição (carnes, massas, sobremesas, etc…). As categorias serão definidas pelo próprio restaurante através do gerente. Depois de escolher o tipo de refeição, o cliente fará seu pedido dado os pratos disponíveis podendo fazer observações sobre o mesmo. Os pedidos serão adicionados a uma lista onde o cliente poderá observar o tempo de preparo ou até mesmo cancelar o seu pedido. Após o cliente enviar o pedido, os cozinheiros terão acesso ao mesmo e irão servi-los. No final, o cliente poderá avaliar o atendimento e o restaurante através de um sistema de notas. 


### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser desenvolvidas. O princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas e/ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/intermenu8/trabalhomdbd/blob/master/imagens/imenumock.PNG "Title")
![Arquivo PDF do Protótipo Balsamiq feito para IMenu: The Interactive Menu](https://github.com/intermenu8/trabalhomdbd/blob/master/arquivos/Mockup.pdf "Empresa Devcom")


#### 4.1 TABELA DE DADOS DO SISTEMA:
![Alt text](https://github.com/intermenu8/trabalhomdbd/blob/master/arquivos/imenutests.xlsx "Tabela exemplo")
    
    
#### 4.2 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
   Quantos clientes gastam menos de R$100,00 em um pedido?
   Quais os 3 clientes que gastam menos nos pedidos?
   Quantos clientes costumam fazer observações nos pedidos?
   Quais os pratos mais caros?
   Qual o foi o valor total arrecadado com esses 10 pedidos?
   Quais os 3 pratos mais caros?(dentre esses)
   Quais as 3 categorias mais caras?(dentre essas)
   Qual o preço médio dos pratos?
   Quantos os clientes gastam por pedido em média?
   Quantos clientes gastam um valor acima da média?
    
>## Marco de Entrega 01 em: (24/03/2018)<br>

### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
![Alt text](https://github.com/intermenu8/trabalhomdbd/blob/master/imagens/Capturar.PNG "Modelo Conceitual")
    
## Marco de Entrega 01 em: (20/04/2018)<br>
#### 5.3 DESCRIÇÃO DOS DADOS 
    CLIENTE: Tabela que armazena as informações relativas ao cliente<br>
    numero: número que identifica o cliente
    nome: nome do cliente, para melhor atendimento
    gasto: soma dos valores dos pedidos do cliente
    COZINHEIRO: Tabela que armazena as informações relativas ao cozinheiro<br>
    id: identificação do cozinheiro
    nome: nome do cozinheiro
    PEDIDO: Tabela que armazena as informações relativas ao pedidobr>
    valor: soma dos valores dos pratos do pedido
    id:identificação do pedido
    observações: observações que o cliente pode fazer em relação ao seu pedido(exemplo: sem azeitona;)
    GERENTE: Tabela que armazena as informações relativas ao gerente<br>
    senha: senha para o gerente ter acesso ao sistema como gerente
    CATEGORIA: Tabela que armazena as informações relativas à categoria<br>
    id: identificação da categoria
    nome: nome da categoria
    PRATO: Tabela que armazena as informações relativas ao prato<br>
    id: identificação do prato
    nome: nome do prato
    preço: preço do prato
    INGREDIENTE: Tabela que armazena as informações relativas ao ingrediente<br>
    id: identificação do ingrediente
    nome: nome do ingrediente
    <br>

>## Marco de Entrega 01 em: (12/05/2018)<br>
### 6	MODELO LÓGICO<br>
![Alt text](https://github.com/intermenu8/trabalhomdbd/blob/master/imagens/mdbdIMenu.PNG "Modelo Lógico")
       
      
### 7	MODELO FÍSICO<br>
        a) inclusão das instruções de criacão das estruturas DDL 
        (criação de tabelas, alterações, etc..)          
        
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físic
        b) formato .SQL

#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script 
        (create para tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script 
        (Drop table + Create de tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.


    
#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>


#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        

## Marco de Entrega 02 em: (16/06/2018)<br>
### ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO SEMESTRAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (30/06/2018)
<br>

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

#### 9.11	LISTA DE CODIGOS DAS FUNÇÕES E TRIGGERS<br>
        Detalhamento sobre funcionalidade de cada código.
        a) Objetivo
        b) Código do objeto (função/trigger)
        c) exemplo de dados para aplicação
        d) resultados em forma de tabela/imagem
<br>


#### 9.12	GERACAO DE DADOS (MÍNIMO DE 100 MIL REGISTROS PARA PRINCIPAL RELAÇAO)<br>
        a) principal tabela do sistema deve ter no mínimo 100 mil registros
        b) tabelas diretamente relacionadas a tabela principal 10 mil registros
        c) tabelas auxiliares de relacao multivalorada mínimo de 10 registros
        d) registrar o tempo de inserção em cada uma das tabelas do banco de dados
        e) especificar a quantidade de registros inseridos em cada tabela
        Para melhor compreensão verifiquem o exemplo na base de testes:<br>
        https://github.com/discipbd2/base-de-testes-locadora
        

#### 9.13	Backup do Banco de Dados<br>
        Detalhamento do backup.
        a) Tempo
        b) Tamanho
        c) Teste de restauração (backup)
        d) Tempo para restauração
        e) Teste de restauração (script sql)
        f) Tempo para restauração (script sql)
<br>

Data de Entrega: (Data a ser definida)
<br>

#### 9.14	APLICAÇAO DE ÍNDICES E TESTES DE PERFORMANCE<br>
    a) Lista de índices, tipos de índices com explicação de porque foram implementados nas consultas 
    b) Performance esperada VS Resultados obtidos
    c) Tabela de resultados comparando velocidades antes e depois da aplicação dos índices (constando velocidade esperada com planejamento, sem indice e com índice Vs velocidade de execucao real com índice e sem índice).
    d) Escolher as consultas mais complexas para serem analisadas (consultas com menos de 2 joins não serão aceitas)
    e) As imagens do Explain devem ser inclusas no trabalho, bem como explicações sobre os resultados obtidos.
    f) Inclusão de tabela mostrando as 10 execuções, excluindo-se o maior e menor tempos para cada consulta e 
    obtendo-se a media dos outros valores como resultado médio final.
<br>
    Data de Entrega: (Data a ser definida)
<br>   

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 11 Backup completo do banco de dados postgres 
    a) deve ser realizado no formato "backup" 
        (Em Dump Options #1 Habilitar opções Don't Save Owner e Privilege)
    b) antes de postar o arquivo no git o mesmo deve ser testado/restaurado por outro grupo de alunos/dupla
    c) informar aqui o grupo de alunos/dupla que realizou o teste.

    
### 12	TUTORIAL COMPLETO DE PASSOS PARA RESTAURACAO DO BANCO E EXECUCAO DE PROCEDIMENTOS ENVOLVIDOS NO TRABALHO PARA OBTENÇÃO DOS RESULTADOS<br>
        a) Outros grupos deverão ser capazes de restaurar o banco 
        b) executar todas as consultas presentes no trabalho
        c) executar códigos que tenham sido construídos para o trabalho 
        d) realizar qualquer procedimento executado pelo grupo que desenvolveu o trabalho

### 13	DIFICULDADES ENCONTRADAS PELO GRUPO<br>  

    
>## Marco de Entrega 04/Entrega Final em: (Data definida no cronograma)<br>

       
### 14  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
   
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/

#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. Caso existam arquivos com conteúdos sigilosos, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário deste GIT, para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://sis4.com/brModelo/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


        
        


    





