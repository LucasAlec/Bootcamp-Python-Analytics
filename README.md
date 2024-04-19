# Formação Power BI Analyst

Neste repositório será encontrado dois projetos referentes a formação Power BI Analyst.

## Projetos

- **Relatório de Vendas Elegante**
https://app.powerbi.com/links/zMV1szD7As?ctid=a1367d4c-7379-48a6-8680-d962ed9a9b76&pbi_source=linkShare

- **Processando e Transformando Dados com Power BI**
https://app.powerbi.com/links/6DQI7eglZ4?ctid=a1367d4c-7379-48a6-8680-d962ed9a9b76&pbi_source=linkShare

### Requerimentos

- Power BI Desktop
- Excel


# Relatório de Vendas Elegante com Power BI

Neste projeto será apresentado o relatório de vendas feito com Power BI. Aqui podemos observar o poder que a ferramenta possui, nos permitindo trabalhar com um volume grande de dados ilustrados, de forma direta, clara e objetiva.



## Passo a Passo
**Criar elementos da Primeira página do relatório**

Nesta etapa foi necessário estabelecer uma estrutura inicial do relatório, criando caixas/figuras onde seriam posicionados os gráficos, títulos e cor do próprio relatório. É necessário definir o que será apresentado.

**Criar gráficos da Primeira Página do Relatório**

Foram apresentados gráficos que representam as vendas em relação ao segmento, produto e a relação de tudo isso com os países, além disso, foram criados mais de 1 tipo de gráfico para cada relação a fim de facilitar a compreensão dos dados analisados.

**Criando o segmentador e visuais alternativos**

Nesta etapa foram criados os ``indicadores`` a fim de definir que tipo de gráfico poderíamos utilizar para uma análise mais detalhada, por exemplo: Utilizar a relação Sales x Segmento através de um gráfico de barras ou gráfico de  torta.

![Relatório Elegante de Vendas pt1](1/Relatório%20Elegante%20de%20Vendas%20pt1.png)

**Criar botões dos relatórios utilizando indicadores para gravar estado do relatório**

O botões nos permite tornar o relatório mais dinâmico, neste relatório foi criado o botão ``eraser`` que restauram as alterações feitas no relatório. E botões como ``Bar chart`` e ``Tremap`` que definem o tipo de gráfico a ser utilizado na nossa análise. Além disso, foi adicionado botões que permitem a navegação entre as duas páginas do relatório.


![Relatório Elegante de Vendas pt2](1/REV%20pt2.png)



# Processando e Transformando Dados com Power BI

Este projeto tem o objetivo de configurar um setup de banco de dados na Azure, popular o servidor com script fornecido, integrar o MySQL com Power BI e elaborar um relatório no Power BI a partir do banco de dados fornecido.

![Processando e transformando dados com PowerBI](2/PTDP%20.png)

## Passo a Passo

**Criar uma instância do MySQL na Azure**

Para isso basta criar uma conta na Azure e seguir o passo a passo fornecido na interface. E por fim definir a opções de segurança do seu banco de dados.

**Explorar o Recurso - Instância MySQL**

O portal fornece uma interface gráfica para gerenciar sua instância do MySQL. Você pode acessar métricas de desempenho, configurar backups, ajustar as configurações do servidor e muito mais.

**Se conectar ao Banco de Dados com Cloud Shell**

Nesta etapa basta fornecer o `hostname`, `username` e `password` que foram definidos na criação do Banco de Dados.

**Criar Regra no Firewall na Azure para Acesso ao banco de dados**

Clique em `Adicionar Regra de Firewall` ou algo semelhante, dependendo da interface do portal. Isso abrirá um formulário onde você pode especificar os detalhes da regra.
Você precisará fornecer um nome para a regra (por exemplo, "Acesso Permitido do Meu Endereço IP"), bem como o intervalo de endereços IP que deseja permitir o acesso ao banco de dados. Você pode fornecer um único endereço IP ou um intervalo CIDR, dependendo da sua necessidade.

Após preencher os detalhes da regra, salve as configurações. Isso garantirá que apenas os endereços IP especificados tenham permissão para acessar o banco de dados MySQL na Azure.

**Integrando Power BI com MySQL**

Fornecer `hostname`, `port` e `nome do banco de dados`
No Power BI Desktop, clique na opção `Obter Dados` na barra de ferramentas ou na guia "Página Inicial". Selecione "Banco de Dados MySQL" na lista de fontes de dados disponíveis.

**Descrição do Relatório**

O Relatório apresenta o número de horas dos projetos, local onde os empregados residem, salário, departamentos e empregados sem gerente. E além disso, é possível determinar quantos colaboradores existem por gerente.