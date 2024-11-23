                           Análise de Dados sobre COVID-19 com Python, utilizando Flask e Streamlit:

____________________________________________________________________________________________________________________________________________________________________________________________

Descrição do Projeto:
O principal objetivo desse projeto é realizar análises e gerar visualizações de dados sobre a COVID-19 no Brasil, através de gráficos, abrangendo o período de julho a início de novembro de 2024. Através de um arquivo Excel contendo dados sobre casos e óbitos, o projeto proporciona uma interface interativa onde os usuários podem acessar estatísticas básicas, gerar gráficos e explorar um pouco do impacto dessa pandemia no Brasil.

Funcionalidades:

API Flask: Oferece duas rotas principais:

•	/api/statistics: Retorna as estatísticas básicas (média, mediana, desvio padrão) dos dados mais recentes.

•	/api/data: Retorna os dados mais atualizados em formato JSON.

1.	Visualização de Dados com Streamlit:
o	Interface de visualização interativa utilizando o Streamlit para gráficos e tabelas.
o	Permite gerar e visualizar os seguintes gráficos: 
•	Gráfico de Área: Comparação entre os casos novos e óbitos novos.
•	Gráfico de Linhas: Evolução dos casos acumulados ao longo do tempo.
•	Gráfico de Linhas: Evolução dos óbitos acumulados ao longo do tempo.
o	Exibição de uma tabela formatada com os dados mais recentes, com valores numéricos e datas no formato brasileiro.

2.	Estatísticas Básicas:
o	Média, mediana e desvio padrão das variáveis numéricas, como casos acumulados, casos novos, óbitos acumulados e óbitos novos.
Pré-Requisitos:
Antes de executar o script, é preciso que as bibliotecas necessárias estejam devidamente instaladas. Comando de instalação das dependências:
pip install pandas matplotlib seaborn flask streamlit requests openpyxl

Além disso, o projeto depende de um arquivo Excel (Indexado no arquivo do script) com o seguinte formato de colunas:

•	Data: Data dos registros.

•	casosAcumulados: Total de casos acumulados.

•	casosNovos: Total de casos novos.

•	obitosAcumulados: Total de óbitos acumulados.

•	obitosNovos: Total de óbitos novos.

•	País: País do qual os dados são referentes.

O arquivo Excel deve ser especificado no código, em file_path, com o nome COVID_19_2024.xlsx.

Execução Local:
1.	Iniciar o Flask API: O servidor Flask fornece as rotas de API para dados e estatísticas. Ele será iniciado em segundo plano. Execute o script Python da seguinte maneira:

2.	Acessar a Interface Streamlit: O Streamlit irá exibir uma interface gráfica para visualização dos dados. A interface será exibida automaticamente após o Flask iniciar.
o	Acesse a interface Streamlit no seu navegador, geralmente em http://localhost:8501.
o	Comando para rodar o Streamlit no terminal: streamlit run main.py

4.	Interação com a Aplicação:
o	A página inicial mostrará informações sobre o projeto, autores e dados sobre a COVID-19.
o	O Gráfico de Área - exibirá uma comparação entre os casos novos e óbitos novos.
o	O Gráfico de Linhas - comparará a evolução de casos acumulados e óbitos ao longo do tempo.
o	A tabela de dados será apresentada com valores formatados para facilitar a leitura.

Endpoints da API:

•	GET /api/statistics: Retorna as estatísticas básicas (média, mediana e desvio padrão) dos dados mais recentes.

•	GET/api/data: Retorna os dados mais recentes em formato JSON.

Estrutura:

•	COVID_19_2024.xlsx: Arquivo Excel com os dados de COVID-19.

•	main.py: Arquivo Python principal com a implementação de Flask e Streamlit.

•	requirements.txt: Arquivo de dependências, caso necessário para instalação.

Projeto Desenvolvido por:

•	Rayane Sant'Anna: Matrícula: 2024.0502.8821 |	Email: raymscs@hotmail.com

•	Naiá Duhau:	Matrícula: 2024.0500.0791 | Email: naiaduhau@gmail.com

Informações Adicionais:
•	Disciplina: Linguagem Python | Professor: Raphael Mauricio Sanches de Jesus

•	Pós-Graduação | Data de Entrega: 23/11/2024

Considerações finais:
Este projeto tem como objetivo proporcionar uma análise interativa e visual dos dados relacionados à pandemia de COVID-19, com ênfase na evolução dos casos e óbitos no Brasil entre julho e novembro de 2024.
