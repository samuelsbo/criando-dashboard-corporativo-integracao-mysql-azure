# criando-dashboard-corporativo-integracao-mysql-azure

# Dashboard Corporativo - Integração Power BI, MySQL e Azure

Este projeto contém um **dashboard corporativo** desenvolvido no Power BI, que integra dados de um banco de dados **MySQL** hospedado na **Azure**. O objetivo principal do dashboard é fornecer insights detalhados sobre horas trabalhadas, custos de mão de obra (MO) e o desempenho de projetos por departamento, localização e funcionário.

## Sumário

- [Descrição do Projeto](#descrição-do-projeto)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Base de Dados](#base-de-dados)
- [Integração MySQL e Power BI](#integração-mysql-e-power-bi)
- [Cálculos e Medidas](#cálculos-e-medidas)
- [Principais Insights](#principais-insights)
- [Conclusões](#conclusões)
- [Autor](#autor)

## Descrição do Projeto

Este dashboard foi criado para monitorar e analisar as horas trabalhadas e os custos de mão de obra (MO) em diversos projetos e departamentos dentro da empresa. Ele integra dados do MySQL, utilizando o Power BI para processar e visualizar essas informações. O tratamento dos dados foi realizado por meio do Power Query, permitindo uma análise precisa do desempenho dos projetos.

## Tecnologias Utilizadas

- **MySQL**: Para armazenamento e gerenciamento de dados.
- **Azure**: Hospedagem do banco de dados MySQL.
- **Power BI Desktop**: Para conexão ao banco de dados, tratamento dos dados e criação dos dashboards.

## Base de Dados

As tabelas do banco de dados foram criadas via MySQL e são estruturadas conforme o seguinte esquema:

- **employee**: Armazena os dados dos funcionários, como nome, sobrenome, SSN, data de nascimento, endereço, sexo, salário, entre outros.
- **departament**: Contém informações sobre os departamentos, como nome, número, e o gerente responsável.
- **dept_locations**: Localizações dos departamentos.
- **project**: Detalhes sobre os projetos, incluindo nome, número e localização.
- **works_on**: Relaciona os funcionários aos projetos e registra as horas trabalhadas em cada projeto.
- **dependent**: Informações sobre os dependentes dos funcionários.

## Integração MySQL e Power BI

O banco de dados MySQL foi hospedado no **Azure**, e a integração foi realizada por meio do **Power BI Desktop**, que se conectou diretamente ao banco para importar e tratar os dados. Após a conexão, os dados foram preparados utilizando o **Power Query** e visualizados em dashboards interativos no Power BI.

## Cálculos e Medidas

Para realizar os cálculos utilizados nos visuais, foram aplicadas as seguintes funções DAX no Power BI:

- **SUM**: Utilizada para calcular o total de horas trabalhadas e custos de mão de obra.
- **COUNT**: Contagem do número total de funcionários e projetos.
- **DISTINCTCOUNT**: Para contar o número de funcionários únicos por projeto e departamento.

## Principais Insights

1. **Custos de MO por Departamento**:
   - Pesquisa foi o departamento com maior custo de mão de obra, com valor superior a $21 mil.

2. **Custos de MO por Localização**:
   - As unidades em **Administração-Stafford** e **Pesquisa-Houston** registraram os maiores custos de MO.

3. **Custos de MO por Projeto**:
   - **Product Z** e **Newbenefits** foram os projetos mais custosos, com valores superiores a $7 mil.

4. **Horas Trabalhadas por Departamento**:
   - O departamento de **Pesquisa** registrou o maior número de horas trabalhadas, seguido de perto pelo departamento de **Administração**.

5. **Horas Trabalhadas por Projeto**:
   - Os projetos **Computerization** e **Newbenefits** lideraram em horas trabalhadas, ambos com 55 horas cada.

## Conclusões

O dashboard permite uma análise detalhada dos custos de mão de obra e horas trabalhadas por projeto e departamento. Ele fornece uma visão clara sobre onde os maiores investimentos de tempo e recursos estão ocorrendo dentro da empresa, ajudando na alocação eficiente de recursos e na tomada de decisões estratégicas.

## Autor

Este projeto foi desenvolvido por Samuel Batista, baseado nas orientações da tutora Juliana Mascarenhas (@julianazanelatto). Sinta-se à vontade para entrar em contato ou contribuir com melhorias!
