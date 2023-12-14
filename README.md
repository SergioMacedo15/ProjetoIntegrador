
# Sequencia lógica do Projeto


# Escolha das Tecnologias

## Backend
No desenvolvimento do backend, a escolha recaiu sobre [Node.js](https://nodejs.org/) com o framework [Express](https://expressjs.com/). A combinação destas tecnologias proporciona um ambiente altamente eficiente para a construção de servidores web robustos e escaláveis. Além disso, a integração perfeita do Node.js com o Express simplifica a criação de APIs e o gerenciamento de rotas.

Para armazenamento de dados, adotamos o [MongoDB](https://www.mongodb.com/) como banco de dados. O MongoDB, um banco de dados NoSQL, oferece flexibilidade e escalabilidade, tornando-o uma escolha ideal para aplicações que demandam um modelo de dados dinâmico.

**Estrutura do Projeto:**
```plaintext
backend/
│
├── controllers/
│   └── [Controladores]
│
├── models/
│   └── [Modelos MongoDB]
│
├── routes/
│   └── [Rotas Express]
│
├── config/
│   └── [Configurações]
│
├── middleware/
│   └── [Middlewares Personalizados]
│
├── .env
├── server.js
└── ...
```
Certifique-se de configurar o ambiente e as variáveis de ambiente necessárias para a conexão com o MongoDB. Configurações como link de acesso seja ele local ou provido pela própria plataforma e a autorização de acesso a rede que esta sendo utilizada.

**Instalação:**
```plaintext
# Backend: Instalação das dependências do Node.js e do MongoDB
cd backend
npm install express mongoose dotenv
# express: Framework web para Node.js
# mongoose: ODM (Object Data Modeling) para MongoDB
# dotenv: Carrega variáveis de ambiente a partir de um arquivo .env
Certifique-se de configurar o ambiente e as variáveis de ambiente necessárias para a conexão com o MongoDB.
```

A estrutura do projeto facilita a manutenção e escalabilidade, com os controladores (controllers) responsáveis por manipular as requisições, os modelos (models) definindo a estrutura dos dados no MongoDB, as rotas (routes) gerenciando o fluxo da aplicação, configurações específicas no diretório config, e middlewares personalizados no diretório middleware. O arquivo server.js atua como ponto de entrada da aplicação.

#### Dependências do Backend:

- [bcrypt](https://www.npmjs.com/package/bcrypt): ^5.1.1
  - **Propósito:** Utilizado para criptografia de senhas.
  - **Justificativa:** A criptografia de senhas é essencial para garantir a segurança das credenciais dos usuários armazenadas no banco de dados.

- [body-parser](https://www.npmjs.com/package/body-parser): ^1.20.2
  - **Propósito:** Analisa o corpo das requisições HTTP.
  - **Justificativa:** Facilita a extração de dados do corpo das requisições, tornando o manuseio de dados mais eficiente.

- [express](https://www.npmjs.com/package/express): ^4.18.2
  - **Propósito:** Framework web para Node.js.
  - **Justificativa:** Simplifica o desenvolvimento de aplicativos web e APIs, proporcionando uma estrutura robusta e flexível.

- [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken): ^9.0.2
  - **Propósito:** Geração e verificação de tokens de autenticação.
  - **Justificativa:** Essencial para implementar a autenticação baseada em tokens, garantindo a segurança das comunicações.

- [mongodb](https://www.npmjs.com/package/mongodb): ^6.3.0
  - **Propósito:** Driver oficial do MongoDB para Node.js.
  - **Justificativa:** Possibilita a interação eficiente com o banco de dados MongoDB, utilizado para armazenar dados da aplicação.

- [mongoose](https://www.npmjs.com/package/mongoose): ^8.0.2
  - **Propósito:** Modelagem de objetos MongoDB.
  - **Justificativa:** Simplifica a interação com o MongoDB ao fornecer uma camada de abstração, permitindo a definição de modelos de dados de forma mais intuitiva.

- [nodemon](https://www.npmjs.com/package/nodemon): ^3.0.2
  - **Propósito:** Monitora alterações nos arquivos e reinicia automaticamente o servidor.
  - **Justificativa:** Facilita o desenvolvimento, eliminando a necessidade de reinicialização manual do servidor a cada alteração no código.

- [socket.io](https://www.npmjs.com/package/socket.io): ^4.7.2
  - **Propósito:** Habilita comunicação em tempo real via WebSocket.
  - **Justificativa:** Essencial para implementar funcionalidades de chat em tempo real, proporcionando uma experiência interativa aos usuários.

- [uuid](https://www.npmjs.com/package/uuid): ^9.0.1
  - **Propósito:** Geração de identificadores únicos.
  - **Justificativa:** Utilizado para criar identificadores únicos, garantindo integridade e unicidade em diversos contextos da aplicação.

## Frontend
No frontend, adotamos o [React](https://reactjs.org/) como nossa principal biblioteca. Além disso, incorporamos o [hookforms](https://react-hook-form.com/) para facilitar a manipulação de formulários. 

### Sobre React

**React** é uma biblioteca JavaScript de código aberto desenvolvida pelo Facebook para construção de interfaces de usuário (UI) interativas e eficientes. Uma das principais características do React é a criação de componentes reutilizáveis que representam partes específicas da interface do usuário. Esses componentes podem ser compostos para formar a estrutura completa da aplicação.

## Principais Conceitos do React:

1. **Componentes:** Os componentes são blocos de construção fundamentais em React. Eles encapsulam o comportamento e a aparência da interface do usuário, promovendo reutilização e modularidade.

2. **Estado (State):** O estado é uma representação instantânea dos dados na aplicação. Quando o estado de um componente muda, o React re-renderiza automaticamente a interface do usuário para refletir essas alterações.

3. **Propriedades (Props):** As propriedades são mecanismos para passar dados de um componente pai para um componente filho. Elas são passadas como atributos nos componentes.

4. **Virtual DOM:** O React utiliza um conceito chamado Virtual DOM para otimizar as atualizações de interface do usuário. Em vez de atualizar diretamente o DOM, o React compara uma versão virtual do DOM e aplica apenas as alterações necessárias.

## Exemplo de Estrutura de um Projeto React

A estrutura de um projeto React típico pode ser organizada da seguinte maneira:

```markdown
meu-projeto-react/
│
├── public/
│   ├── index.html
│   └── favicon.ico
│
├── src/
│   ├── components/
│   │   ├── MeuComponente.js
│   │   └── OutroComponente.js
│   │
│   ├── pages/
│   │   ├── PaginaPrincipal.js
│   │   └── PaginaSecundaria.js
│   │
│   ├── App.js
│   ├── index.js
│   └── index.css
│
├── package.json
└── README.md
```

**Código por trás**
<img width="1360" alt="Screenshot 2023-12-14 at 19 40 30" src="https://github.com/SergioMacedo15/ProjetoIntegrador/assets/63246587/f2c4c0b4-ce79-4504-836d-38e5769ba4f9">

**Pagina exemplo de uso de Hookform**
<img width="1439" alt="Screenshot 2023-12-14 at 19 39 24" src="https://github.com/SergioMacedo15/ProjetoIntegrador/assets/63246587/5f943c43-67c0-4cb2-8489-6db3686a4533">

No desenvolvimento do frontend, a ênfase foi dada à área de registro e visualização do cliente na página. Essa seção é crucial para a interação e experiência do usuário, e, portanto, as dependências foram cuidadosamente escolhidas para garantir eficiência e facilidade de uso nesse contexto específico.

#### Dependências do Frontend:

- **[@fontsource/roboto](https://www.npmjs.com/package/@fontsource/roboto):** ^5.0.8
  - **Propósito:** Fonte Roboto para estilização de texto.
  - **Justificativa:** Adoção de uma fonte padrão que oferece legibilidade e aparência moderna aos elementos de texto na interface.

- **[@hookform/resolvers](https://www.npmjs.com/package/@hookform/resolvers):** ^3.3.2
  - **Propósito:** Resolvedores para formulários React Hook.
  - **Justificativa:** Facilita a validação e resolução de formulários, melhorando a experiência do usuário durante a interação com formulários.

- **[next](https://www.npmjs.com/package/next):** 13.5.6
  - **Propósito:** Framework React para renderização de páginas no lado do servidor (SSR).
  - **Justificativa:** Oferece funcionalidades avançadas, como renderização no lado do servidor, e navegação de forma simplicada, facilitando a criação de aplicativos web eficientes.

- **[react](https://www.npmjs.com/package/react):** ^18
  - **Propósito:** Biblioteca JavaScript para construção de interfaces de usuário.
  - **Justificativa:** Base fundamental para o desenvolvimento de componentes e interfaces interativas na aplicação.

- **[react-bootstrap](https://www.npmjs.com/package/react-bootstrap):** ^2.9.1
  - **Propósito:** Biblioteca de componentes Bootstrap para React.
  - **Justificativa:** Facilita a criação de interfaces atraentes e responsivas com componentes pré-estilizados.

- **[react-dom](https://www.npmjs.com/package/react-dom):** ^18
  - **Propósito:** Pacote de renderização DOM para React.
  - **Justificativa:** Necessário para a renderização de componentes React no navegador.

- **[react-feather](https://www.npmjs.com/package/react-feather):** ^2.0.10
  - **Propósito:** Ícones Feather como componentes React.
  - **Justificativa:** Adição de ícones elegantes e leves para melhorar a estética e a usabilidade da interface.

- **[react-hook-form](https://www.npmjs.com/package/react-hook-form):** ^7.47.0
  - **Propósito:** Biblioteca para criação e gerenciamento de formulários React.
  - **Justificativa:** Simplifica o processo de criação de formulários, tornando a coleta e validação de dados mais eficientes.

- **[zod](https://www.npmjs.com/package/zod):** ^3.22.4
  - **Propósito:** Validador de esquemas para JavaScript e TypeScript.
  - **Justificativa:** Facilita a validação de dados, especialmente útil em conjunto com formulários para garantir a integridade dos dados submetidos.

Essas dependências foram escolhidas para otimizar o desempenho, a usabilidade e a aparência da seção de registro e visualização do cliente, proporcionando uma experiência consistente e agradável aos usuários. Certifique-se de consultar a documentação de cada dependência para uma implementação eficaz e personalização conforme necessário.

## Possíveis Melhorias Futuras

1. **Adoção de Bibliotecas de Estilização Prontas, como Bootstrap:**
   - **Justificativa:** A incorporação de bibliotecas de estilização prontas, como o [Bootstrap](https://getbootstrap.com/), pode acelerar o desenvolvimento, garantindo uma aparência visualmente atrativa e consistente em toda a aplicação. Isso permite que os desenvolvedores foquem mais na lógica de negócios e menos na criação de estilos personalizados.

2. **Integração do Redux para Gerenciamento de Estado:**
   - **Justificativa:** A implementação do [Redux](https://redux.js.org/) pode trazer benefícios significativos para o gerenciamento do estado da aplicação, especialmente em projetos complexos. Ele oferece um fluxo de dados unidirecional, facilitando o rastreamento de mudanças e a manutenção do estado global de forma mais organizada e escalável.

3. **Otimização de Desempenho com Serviço de Cache:**
   - **Justificativa Técnica:** Considerando a implementação de um serviço de cache, essa melhoria técnica pode aumentar significativamente o desempenho da aplicação. Ao armazenar temporariamente dados frequentemente acessados em um sistema de cache, podemos reduzir a necessidade de solicitações ao servidor, melhorando a velocidade de carregamento e a eficiência geral da aplicação.

## Mobile


A escolha do React Native para o desenvolvimento mobile no projeto é motivada por uma série de vantagens, incluindo a facilidade de integração e diversos benefícios práticos.

## Vantagens do React Native:

- **Compartilhamento Eficiente de Código:** Reduz a duplicação de esforços no desenvolvimento ao permitir o compartilhamento de código entre aplicações iOS e Android.

- **Familiaridade com React:** Desenvolvedores familiarizados com React para web podem aplicar diretamente seus conhecimentos ao ambiente mobile, agilizando a curva de aprendizado e promovendo consistência na aplicação.

- **Integração Simplificada:** Oferece uma integração facilitada com bibliotecas nativas, permitindo a utilização de módulos nativos quando necessário. Isso garante uma experiência de usuário uniforme e eficiente.

## Estrutura Básica de Pastas e Arquivos no Projeto React Native

A estrutura básica de pastas e arquivos no projeto React Native segue uma organização similar às outras partes do projeto, adaptada para ambientes móveis.

```plaintext
meu-projeto-react-native/
│
├── android/
│
├── ios/
│
├── node_modules/
│
├── src/
│   ├── components/
│   │   ├── MeuComponente.js
│   │   └── OutroComponente.js
│   │
│   ├── screens/
│   │   ├── TelaPrincipal.js
│   │   └── TelaSecundaria.js
│   │
│   ├── App.js
│   └── index.js
│
├── .gitignore
├── package.json
├── README.md
└── yarn.lock

```

# APIs Utilizadas no Projeto

## Parte Web

### Google Maps API

- **Objetivo:** A Google Maps API foi integrada para fornecer funcionalidades de mapa na parte web do projeto.
  
- **Recursos:**
  - **Mapas Interativos:** Incorporação de mapas interativos para permitir aos usuários visualizar e interagir com diferentes localizações.
  - **Marcadores e Informações:** Adição de marcadores e informações sobre pontos específicos no mapa para uma experiência mais rica.

### Routes API

- **Objetivo:** A API de rotas foi implementada para calcular e otimizar trajetos específicos na parte web.

- **Recursos:**
  - **Cálculo de Rotas:** Utilização de algoritmos avançados para calcular as melhores rotas entre pontos definidos, proporcionando uma navegação eficiente.

### Location API

- **Objetivo:** A API de Localização foi incorporada para fornecer funcionalidades relacionadas à posição geográfica na parte web.

- **Recursos:**
  - **Rastreamento de Localização:** Possibilidade de rastrear e exibir a localização atual do usuário.
  - **Geocodificação e Reversão:** Conversão de endereços em coordenadas geográficas e vice-versa.

## Parte Mobile (Expo Libraries e Redux)

### Expo Permissions

- **Objetivo:** A Expo Permissions foi utilizada para gerenciar e obter permissões do usuário no ambiente mobile.

- **Recursos:**
  - **Acesso à Localização:** Solicitação de permissões para acessar a localização do dispositivo, permitindo a funcionalidade de rastreamento.

### Expo Location

- **Objetivo:** A Expo Location ofereceu funcionalidades avançadas de localização para o aplicativo mobile.

- **Recursos:**
  - **Rastreamento Contínuo:** Capacidade de rastrear a localização em tempo real do dispositivo.
  - **Integração com Mapas:** Facilitou a integração com mapas para exibir a localização em um contexto visual.

### Expo MapView

- **Objetivo:** A Expo MapView permitiu a incorporação de mapas interativos na parte mobile.

- **Recursos:**
  - **Mapas Nativos:** Utilização de mapas nativos para fornecer uma experiência de usuário familiar e intuitiva.
  - **Personalização:** Adição de marcadores, sobreposições e outros elementos personalizados ao mapa.

### Expo SecureStore

- **Objetivo:** A Expo SecureStore foi empregada para garantir o armazenamento seguro de dados sensíveis no aplicativo mobile.

- **Recursos:**
  - **Segurança de Dados:** Armazenamento seguro de informações sensíveis, como tokens de acesso e identificadores.

### Redux

- **Objetivo:** O Redux foi adotado para gerenciar o estado da aplicação, especialmente para viagens abertas pelos usuários.

- **Recursos:**
  - **Centralização de Estado:** Utilização de um store central para armazenar e gerenciar o estado global da aplicação.
  - **Gerenciamento de Viagens:** Armazenamento e manipulação eficiente do estado das viagens abertas pelos usuários.

Essas APIs e bibliotecas desempenharam papéis cruciais no desenvolvimento tanto da parte web quanto mobile do projeto, fornecendo acesso seguro a recursos e dados essenciais, além de garantir uma gestão eficiente do estado da aplicação mobile por meio do Redux.

**Link para apresentação**
https://drive.google.com/drive/folders/1oqTGs1FoT2qiCoB0k9HFkAmWYxFT_CjX?usp=sharing


