# Escolha_Sua_Trilha
Protótipo de um ChatBot para ajudar pessoas a encontrarem trilha de longo curso no Brasil e ajudar no planejamento dessa aventura.
O Brasil possui muitas trilhas e esse projeto visa melhorar divulgação dessas trilhas, utlizando como base os documentos do
Ministério da Turismo sobre as trilha de Longo Curso.

A utilização é bem simples, basta iniciar o Chat que irá te guiar no processo de escolher e planejar uma aventura.

Por mais que ele já esteja funcional, ainda é um protótipo e bem uma base de dados ainda limitada, mas que pode ser
incrementada no futuro, para conseguir ter também dados de mundo todo, sendo uma ferramenta ótima para os trilheiros
e montanhistas que buscam uma aventura ou até mesmo para uma Agência de Viagens especializada em aventuras.

# Como configurar o ChatBot
## Colocar sua API do Google Gemini
Para colocar a API do Google de forma segura, precisamos configurar um chave secreta.
![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/72e93501-f16a-468c-b778-cb805fb3d4e0)

No exemplo, utilizo o nome de API_KEY. Para configurar, clique no ícone da Chave no lado esquerdo do Colab:

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/4e970447-eb9b-4ed0-9591-177c55ead1fe)

Basta deixa o Notebook access habilitado, em NAME colocar o nome API_KEY e em VALUE copiar o valor da sua API.


## Baixar os PDFs e colocar no Google Drive
Antes de mais nada, você precisa baixar os dois arquivos PDFs (manual_estruturacao.pdf e trilhas_do_brasil.pdf) e adionar eles
no seu Google Drive, para que o Notebook do Colab consiga acessar eles para fazer a extração.
Com os arquivos no Drive, rode a segunda linha do Notebook, para fazer a conexão:

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/264fe085-0222-4093-a0fc-1d89e782b2a1)

Depois de feita a conexão, clique no ícone da PASTA no menu da esquerda, lá terá a pasta DRIVE.
Navege por ela até chegar nos arquivos PDFs:

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/fff648ac-9d99-49cd-b2ef-f58fa4074bfc)

Em cada um dos arquivos, quando você coloca o mouse em cima do arquivo, aparecem ... no final dele. Clique neles e escolha
a opção de COPY PATH:

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/2af568b7-8cab-4cc7-8c0c-90ddf3be6a9b)

Com o PATH copiado, vá até o ponto onde ocorre a extração dos PDFs e cole esse PATH dentro das aspas para os dois arquivos:

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/bdbe7aa5-6560-4ae9-b756-99c446bd7a2d)

Pronto! Agora o Notebook está configurado.

# Rodando o ChatBot
Para rodar o ChatBot, depois da configaração da API e dos arquivos PDFs, basta ir em RUNTIME -> RUN ALL

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/dd27a573-fece-4be5-9eac-660431501df8)

E ir até o final do Notebook e aguardar o Chat ser iniciado. Depois, basta interagir com ele para descobrir
uma aventura perto de você:

![image](https://github.com/marcelodaros/Escolha_Sua_Trilha/assets/44591098/29ba933b-2e6f-4245-98db-0017cff2d9e6)
