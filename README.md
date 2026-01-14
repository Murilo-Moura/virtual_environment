# Web Application: Análise de Anúncios de Vendas de Carros

## Descrição do Projeto
Este projeto foi desenvolvido com o foco em praticar tarefas fundamentais de engenharia de software aplicadas à ciência de dados. O objetivo principal foi criar um ambiente de desenvolvimento robusto, gerenciar dependências, construir um painel interativo (dashboard) para exploração de dados e realizar a implantação (deploy) em um serviço de nuvem, tornando os resultados acessíveis via web.

## Ferramentas e Bibliotecas Utilizadas
- **Python**: Linguagem de programação base.
- **Streamlit**: Framework utilizado para a criação da interface do aplicativo web.
- **Pandas**: Manipulação e tratamento dos dados brutos.
- **Plotly Express**: Criação de gráficos dinâmicos e interativos.
- **Render**: Plataforma de nuvem utilizada para o deploy da aplicação.
- **Git/GitHub**: Controle de versão e gestão de repositório.

## Tabela (Dicionário de Dados)
O conjunto de dados `vehicles.csv` contém informações sobre anúncios de carros e possui os seguintes campos:

| Campo | Descrição |
| :--- | :--- |
| **price** | Preço de venda do veículo |
| **model_year** | Ano do modelo do carro |
| **model** | Modelo do veículo |
| **condition** | Condição de conservação (excelente, boa, etc.) |
| **cylinders** | Número de cilindros do motor |
| **fuel** | Tipo de combustível utilizado |
| **odometer** | Quilometragem registrada no odômetro |
| **transmission** | Tipo de transmissão (automática, manual) |
| **type** | Tipo de carroceria (SUV, sedan, etc.) |
| **paint_color** | Cor do veículo |
| **is_4wd** | Indica se o veículo possui tração 4x4 (Booleano) |
| **date_posted** | Data em que o anúncio foi publicado |
| **days_listed** | Quantidade de dias que o anúncio ficou ativo |

## Metodologia
**1. Configuração do Ambiente**
- Criação e gerenciamento de um ambiente virtual Python para isolar dependências.
- Configuração do ficheiro `requirements.txt` para garantir a replicabilidade do projeto.

**2. Pré-processamento e Limpeza**
- Conversão de tipos de dados (ex: `date_posted` para datetime).
- Tratamento de valores ausentes em colunas críticas como `model_year`, `cylinders`, `odometer` e `is_4wd`.
- Preenchimento de valores nulos na cor do veículo como "unknown".

**3. Desenvolvimento da Aplicação Web**
- Construção de uma interface com Streamlit contendo cabeçalhos e botões de comando.
- Implementação de lógica para geração de visualizações sob demanda (Histogramas e Gráficos de Dispersão).

**4. Deploy em Nuvem**
- Configuração do repositório no GitHub para integração contínua com o **Render**.
- Disponibilização da aplicação através de um link público.

## Resultados
O resultado final é um aplicativo web funcional onde o usuário pode interagir com os dados de vendas de carros. Através de cliques em botões, é possível visualizar a distribuição da quilometragem (odômetro) e analisar a relação entre preço e ano do modelo ou condição do veículo.

A aplicação está disponível publicamente em: [Meu Projeto no Render](https://my-first-project-o4ah.onrender.com)



## Aprendizados
- **Engenharia de Software**: Domínio do ciclo de vida de uma aplicação, desde a criação do ambiente até a entrega final ao usuário.
- **Desenvolvimento Web com Python**: Uso do Streamlit para transformar scripts de análise em ferramentas interativas de fácil consumo.
- **Gestão de Dependências**: Importância de controlar versões de bibliotecas para evitar erros em ambientes de produção.
- **Implantação em Nuvem**: Experiência prática em hospedar projetos reais em servidores externos (Cloud Services).
- **Controle de Versão**: Uso de `.gitignore` e boas práticas de commits para manter um repositório profissional.

