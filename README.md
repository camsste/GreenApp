# Infrações Ambientais do Recife
Este é um projeto em React Native que utiliza a API do Dados Recife para exibir locais que sofreram infrações ambientais e mostra a localização atual do usuário em coordenadas.

# Descrição
Este aplicativo exibe uma lista de locais que sofreram infrações ambientais na cidade do Recife, utilizando dados fornecidos pela API do Dados Recife. Também mostra a localização atual do usuário em coordenadas geográficas.

# API Utilizada
A API utilizada neste projeto é fornecida pelo portal de dados abertos da Prefeitura do Recife. A URL da API é:  http://dados.recife.pe.gov.br/api/3/action/datastore_search?resource_id=41dda42a-2a09-47ed-8667-123b024e1546

Esta API fornece dados de infrações registradas na cidade do Recife. Abaixo estão os principais campos que são retornados pela API:

- **cnpj**: O CNPJ da entidade registrada.
- **data**: A data em que a vistoria foi realizada.
- **endereco**: O endereço onde a infração foi registrada.
- **id**: Um identificador único para o registro.
- **infracoes**: As infrações cometidas, conforme o artigo da legislação.
- **latitude**: A latitude da localização da infração.
- **longitude**: A longitude da localização da infração.
- **nomeFantasia**: O nome fantasia da entidade registrada.
- **numeroAuto**: O número do auto de infração.
- **razaoSocial**: A razão social da entidade registrada.

# Funcionalidades
- Listar locais com infrações ambientais.
- Exibir detalhes sobre as infrações.
- Mostrar a localização atual do usuário em coordenadas geográficas.

# Tecnologias Utilizadas
- React Native
- Expo
- API do Dados Recife
  
# Requisitos
- Node.js
- Expo CLI
- Conta no Expo

# Instalação
1. Clone o repositório:
```
git clone https://github.com/seu-usuario/infrações-ambientais-recife.git
cd infrações-ambientais-recife
```
2. Instale as dependências:
```
npm install
```

4. Inicie o projeto com Expo:
```
npx expo start
```
# Como Executar
1. Certifique-se de que você tem o Expo Go instalado no seu dispositivo móvel.

2. Após iniciar o projeto, um QR code será exibido no terminal ou na página web aberta pelo Expo.

3. Escaneie o QR code com o aplicativo Expo Go para visualizar o projeto no seu dispositivo.

# Estrutura do Projeto
```
greenapp/
├── assets/                                           # Diretório para imagens, fontes e outros recursos estáticos
│   ├── images/                                       # Subdiretório para imagens
│   │   ├── danger.png                                # Exemplo de imagem
│   │   ├── imageMap.png                                # Exemplo de imagem
│   │   └── splash.png                                 # Exemplo de imagem
│   └── fonts/                                        # Subdiretório para fontes
│       └── roboto-font.ttf                           # Exemplo de fonte
├── components/                                         # Diretório para componentes React
│   ├── layout/                                        # Diretório para componentes React de layout
│   │   └── sheet.tsx                                  # Componente React de layout para as telas do aplicativo
│   └── outrosComponentes.tsx                             # Outros componentes React reutilizáveis do projeto
├── constants/                                          # Diretório para constantes do aplicativo
│   └── Colors.ts                                       # Arquivo de constantes para cores do aplicativo
├── screens/                                            # Diretório para telas React do aplicativo
│   ├── HomeScreen.tsx                                # Tela inicial do aplicativo
│   ├── DetailsScreen.tsx                              # Tela de detalhes do aplicativo
│   └── outrosArquivosDeTela.tsx                          # Outros arquivos de telas React do aplicativo
├── Service/                                            # Diretório para classes de serviço do projeto
│   └── Endpoints.ts                                   # Classe de serviço para endpoints da API
├── App.js                                             # Arquivo principal do aplicativo React
├── app.json                                             # Arquivo de configuração do Expo
├── babel.config.js                                       # Arquivo de configuração do Babel
├── package.json                                         # Arquivo de metadados do projeto
└── tsconfig.json                                        # Arquivo de configuração do TypeScript

```

# Licença
Feito por Camile Stefany.
