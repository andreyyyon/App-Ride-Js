# App-Ride

Aplicativo web para registro e acompanhamento de corridas, com funcionalidades de velocímetro, armazenamento de dados de localização (latitude/longitude), visualização de detalhes e histórico de corridas.

## Funcionalidades
- Medir a velocidade em tempo real durante a corrida (velocímetro).
- Armazenar a velocidade, latitude e longitude de cada ponto do trajeto.
- Listar todas as corridas realizadas.
- Visualizar detalhes de cada corrida, incluindo:
  - Cidade e país de início
  - Velocidade máxima
  - Distância percorrida
  - Duração
  - Data e hora de início
  - Trajeto no mapa
- Excluir corridas do histórico.

## Estrutura do Projeto
```
App-Ride/
├── anotações.txt         # Notas e especificações do projeto
├── index.html            # Tela inicial com lista de corridas
├── speedometer.html      # Tela de velocímetro e início de nova corrida
├── detail.html           # Tela de detalhes de uma corrida
├── css/
│   └── global.css        # Estilos globais e customização do Bootstrap
├── js/
│   ├── dataManager.js    # Funções utilitárias para dados de corridas
│   ├── detail.js         # Lógica da tela de detalhes
│   ├── index.js          # Lógica da tela inicial
│   ├── speedometer.js    # Lógica do velocímetro e controle de corrida
│   └── storage.js        # Gerenciamento de armazenamento local
```

## Tecnologias Utilizadas
- HTML5, CSS3 (com Bootstrap 5 e Bootstrap Icons)
- JavaScript (ES6)
- [Leaflet.js](https://leafletjs.com/) para mapas
- LocalStorage para persistência dos dados
- API de Geolocalização do navegador
- API externa para geocodificação reversa (BigDataCloud)

## Telas
- **Index:** Lista de corridas com botão para adicionar nova corrida.
- **Speedometer:** Velocímetro em tempo real, botões de start/stop para iniciar/finalizar corrida.
- **Details:** Exibe detalhes completos da corrida selecionada, incluindo mapa do trajeto.

## Como Usar
1. Abra o `index.html` em um navegador moderno.
2. Clique no botão de adicionar para iniciar uma nova corrida.
3. Na tela do velocímetro, clique em **Start** para começar a registrar a corrida.
4. Clique em **Stop** para finalizar e salvar a corrida.
5. Visualize o histórico de corridas na tela inicial e clique em uma corrida para ver seus detalhes.
6. Na tela de detalhes, é possível excluir a corrida.

## Observações
- O projeto utiliza recursos do navegador como LocalStorage e Geolocalização, portanto, é necessário conceder permissão de localização.
- Para funcionamento completo dos mapas, é necessário acesso à internet.

---
Desenvolvido por [Seu Nome].

