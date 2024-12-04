# **Diariamente**

![Logo do Projeto Diariamente](images/logo diariamente.jpg)


O Diariamente é um diário para registro de pensamentos e acontecimentos com foco em escrita expressiva, reflexão e percepção das emoções.

---
## **Índice**
1. [Sobre o Projeto](#sobre-o-projeto)
2. [Funcionalidades](#funcionalidades)
3. [Histórias de Usuário](#histórias-de-usuário)
3. [Tecnologias Utilizadas](#tecnologias-utilizadas)
4. [Pré-requisitos](#pré-requisitos)
5. [Instruções de Instalação](#instruções-de-instalação)
6. [Estrutura do Projeto](#estrutura-do-projeto)
7. [Licença](#licença)
8. [Contato](#contato)
---

## **Sobre o Projeto**
O Diariamente é uma aplicação criada para facilitar o registro de pensamentos e emoções, visando trazer aos usuários os 
benefícios já comprovados da escrita em diários. O Diariamente foi desenvolvido para seguir a simplicidade do registro em
diários como já conhecemos porém com as facilidades que a tecnologia nos proporciona. O software segue o padrão de arquitetura 
Model-View-Controller (MVC) visando permitir uma maior escalabilidade no código.

---
## **Funcionalidades**

- Criar novos registros para expressar sentimentos e acontecimentos.
- Atribuir a cada registro uma emoção primária e diversas emoções secundárias.
- Exibir todos os registros criados com título, conteúdo, data e hora de criação, emoção primária e secundárias.
- Filtrar registros emoção primária.
- Buscar por termos específicos ou palavras-chave em todos os registros salvos.
- Editar e excluir registros existentes.

---

## **Histórias de Usuário**

1. #### **Registro de Sentimentos e Acontecimentos:**
- **Como** usuário, **gostaria** de registrar meus sentimentos e acontecimentos do dia de forma livre, **pois assim** eu posso desabafar e refletir sobre o que estou vivendo.
- **Como** usuário, **gostaria** de acrescentar reflexões em registros passados, **pois assim** poderei atualizar sentimentos e acontecimentos após refletir mais sobre eles.
- **Como** usuário, **gostaria** de poder excluir registros passados, **pois assim** manterei em meu diário somente registros com os quais ainda me identifico e obtendo uma experiência mais personalizada.

2. #### **Seleção Manual de Sentimentos:**
- **Como** usuário, **gostaria** de escolher manualmente o sentimento relacionado ao meu registro, **pois assim** eu poderei ter uma compreensão mais clara do que estou sentindo.
- **Como** usuário, **gostaria** de selecionar múltiplos sentimentos (sendo um principal e outros secundários) em um único registro, **pois assim** eu poderei representar melhor a complexidade das minhas emoções em determinadas situações.

3. #### **Visualização de Histórico:**
- **Como** usuário, **gostaria** de visualizar meu histórico de registros categorizados por data, **pois assim** eu poderei facilmente relembrar e acessar entradas anteriores.


4. #### **Filtro por Tipos de Sentimento:**
- **Como** usuário, **gostaria** de escolher manualmente o sentimento relacionado ao meu registro, **pois assim** eu poderei ter uma compreensão mais clara do que estou sentindo.
- **Como** usuário, **gostaria** de selecionar múltiplos sentimentos (sendo um principal e outros secundários) em um único registro, **pois assim** eu poderei representar melhor a complexidade das minhas emoções em determinadas situações.
---


## **Tecnologias Utilizadas**

- **Linguagem**: Java
- **Framework**: Maven
- **Banco de Dados**: MySQL

---

## **Pré-requisitos**

Antes de instalar e executar o projeto, certifique-se de ter os seguintes itens instalados:

- **Java Development Kit (JDK) 17 ou superior**
- **Maven** (para gerenciamento de dependências)
- **MySQL** (execução do script SQL para criação e configuração do banco)
- **IDE** recomendada: IntelliJ ou Eclipse

---

## **Instruções de Instalação**

1. **Clone o Repositório:**

   ```bash
   git clone https://github.com/seu-usuario/diariamente.git
   cd diariamente 
   
2. **Configure o Banco de Dados:**
- Execute o arquivo diariamente_DB.sql contendo o script de criação e configuração do banco.
- Atualize as configurações de conexão no arquivo DatabaseConnection.java no pacote util para garantir que o usuario e senha descritos no método de conexão sejam equivalentes aos utilizados para acessar o banco de dados no gerenciador do banco.

3. **Instale as depêndencias:**
    ```bash
   mvn clean install
## **Estrutura do Projeto**
- `src/` : Código fonte da aplicação
  - `controller/` : Classes controller para realizar a comunicação entre os DAO's e as classes view
  - `model/` : Classes model onde é definida a estrutura das classes principais do projeto 
  - `repository/` : Classes DAO para realizar as operações no banco de dados
  - `util/` : Classe DatabaseConnection responsável por instanciar e retornar a conexão com o banco
  - `view/` : Classes view responsáveis por coletar e exibir dados ao usuário
- `database/` : Arquivo diariamente_DP.sql contendo o script para criação e configuração do banco


## **Licença**
Este projeto está licenciado sob a Licença MIT - veja o arquivo para mais detalhes.

## **Contato**
- **Nome:** João Victor Santos
- **e-mail:** joaovictorsantos10@hotmail.com.br
