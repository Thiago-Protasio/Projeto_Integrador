# Gerenciamento de Inventário
Status: *Em desenvolvimento*

## Tecnologias
**Banco de dados**: SQL  
**Front-end**: HTML, CSS, JavaScript  
**Back-end**: Java  
**Desktop**: Java  

## Desenvolvedores
Thiago Protasio

## Objetivo
Esse sistema tem como objetivo gerenciar todo o estoque de peças de uma empresa. Isso 
inclui peças e componentes de máquinas de produção e ferramentas e maquinário da manutenção.  
Haverá dois tipos de usuários no sistema:  
- O **gestor** da oficina deve ser responsável por adicionar novos itens e novos funcionários ao sistema.   
- O **funcionário** deve ser capaz de buscar por itens do inventário e dar baixa caso a quantidade de 
um item seja removida ou adicionada à oficina.

## Funcionalidades (Requisitos Funcionais)
- **RF01** - Login  
**Ator**: Funcionário e gestor  
**Descrição**: O usuário poderá realizar o login informando o username e senha.
- **RF02** - Adicionar ou remover usuários  
**Ator**: Gestor  
**Descrição**: O gestor poderá visualizar uma lista de usuários e escolher adicionar novos usuários ou 
remover. Para cadastrar um novo usuário o gestor deverá preencher os campos de nome, username, 
senha, setor e registro da empresa.
- **RF03** - Dar ou remover permissões de usuário  
**Ator**: Gestor  
**Descrição**: O gestor poderá gerenciar as permissões de um usuário. As permissões definem quais 
ações um usuário poderá realizar dentro do sistema.
- **RF04** - Pesquisa e listagem de itens  
**Ator**: Gestor e funcionário  
**Descrição**: O usuário deve conseguir pesquisar e listar todos os itens do inventario sejam peças, 
ferramentas ou máquinas. Deve ser possível digitar o nome ou código de um item no campo de 
busca e obter os resultados compatíveis com a pesquisa.
- **RF05** - Criação de item  
**Ator**: Gestor  
**Descrição**: O gestor deve ser capaz de adicionar um novo item ao inventario. O cadastro deve conter 
os campos de nome (obrigatório), código de identificação (obrigatório), quantidade (obrigatório, e 
descrição (opcional).
- **RF06** - Atualizar quantidade  
**Ator**: Gestor e funcionário  
**Descrição**: O usuário deve conseguir selecionar um item desejado e atualizar sua quantidade. No 
caso de quantidade maiores ele pode escrevê-las no campo ou no caso de quantidades menores 
usar setas para aumentar ou diminuir uma unidade por vez.
- **RF07** - Alterar status  
**Ator**: Gestor e funcionário  
**Descrição**: o usuário deve poder selecionar um item e alterar seu status para ‘em uso’ se houver 
disponíveis ou alterar para ‘disponível’ se houver itens em uso. O status deve mostrar 
separadamente a quantidade de itens em uso e a quantidade de itens disponíveis.

## Requisitos não Funcionais
- **RNF01** - Banco de dados Relacional  
O sistema deve ser construído utilizando um banco de dados relacional SQL. Preferencialmente 
MySQL já que essa será uma aplicação interna com poucos usuários e não haverá um grande tráfego 
de dados
- **RNF02** - Backup do baco de dados  
Um backup do banco de dados deve ser realizado todos os dias automaticamente, para evitar perdas 
e inconsistências de dados.
