Weather Location Tracker (Integração Google Sheets + Open-Meteo API)
Este projeto foi desenvolvido para automatizar o processo de coleta e consulta meteorológica de múltiplos locais. Ele lê coordenadas geográficas diretamente de uma planilha do Google Sheets (preenchida via formulário) e realiza consultas em tempo real na API pública de previsão do tempo Open-Meteo utilizando Python.

🚀 Funcionalidades
Integração Dinâmica: Conexão e leitura direta de dados públicos do Google Sheets em formato CSV.
Geolocalização Automatizada: Iteração automatizada sobre registros de localizações enviadas com Latitude e Longitude.
Consulta de Clima em Tempo Real: Requisições ágeis utilizando a biblioteca requests para obter a temperatura atualizada via Open-Meteo API.
🛠️ Tecnologias Utilizadas
Python: Linguagem base do projeto.
Pandas: Manipulação de dados e leitura eficiente da planilha.
Requests: Comunicação com a API HTTP REST do Open-Meteo.
Google Sheets: Banco de dados estruturado para cadastro das localizações.
📋 Como Funciona
O usuário cadastra locais através de um formulário que popula a planilha do Google.
O script Python faz a leitura da planilha exportada em tempo real.
O script varre cada linha, extraindo o nome do local, latitude e longitude.
Para cada ponto geográfico, é disparada uma chamada de API para obter os dados climáticos instantâneos, exibindo os resultados consolidados em formato amigável no console.
