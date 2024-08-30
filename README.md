
Documentação do Projeto: Visualização 360° do Interior de um Carro
Sumário
Introdução
Objetivo
Tecnologias Utilizadas
Estrutura do Projeto
Como Executar o Projeto
Componentes e Funcionalidades
Personalização e Extensões
Boas Práticas e Considerações
Conclusão
Introdução
Este projeto implementa uma visualização interativa em 360° do interior de um carro utilizando tecnologias baseadas na web, como o framework A-Frame. Ele permite que os usuários explorem o interior de um carro em um ambiente de realidade virtual ou através de uma interface web tradicional. Esta documentação fornece uma visão geral do projeto, as tecnologias usadas, a estrutura do código e instruções para execução e personalização.

Objetivo
O principal objetivo deste projeto é tornar a visualização de produtos, como interiores de carros, acessível e interativa por meio de tecnologias web. Utilizando frameworks como o A-Frame, o projeto possibilita a criação de experiências imersivas que podem ser acessadas diretamente do navegador, sem a necessidade de software adicional.

Tecnologias Utilizadas
HTML: Para a estruturação da página.
A-Frame: Framework de código aberto para a criação de experiências de Realidade Virtual na web.
A-Frame Extras: Biblioteca de componentes adicionais para A-Frame, fornecendo funcionalidades estendidas.
A-Frame Haptics Component: Biblioteca para adicionar feedback tátil em dispositivos compatíveis.
CSS: Para estilização básica da interface.
JavaScript: Integrado no uso de bibliotecas externas para funcionalidades avançadas.

/////////////////////////////////////////////////////////////////////////////////////////
Estrutura do Projeto
/
├── index.html # Arquivo principal contendo a implementação A-Frame
└── assets/
    └── Previa de teste_360_BMW_F01.jpg  # Imagem 360° usada como fundo
////////////////////////////////////////////////////////////////////////////////////////

Como Executar o Projeto
Pré-requisitos: Navegador moderno (Chrome, Firefox, Edge, etc.) com suporte a WebVR/WebXR.
Passos para execução:
Faça o download ou clone o repositório do projeto.
Certifique-se de que o arquivo index.html e a imagem 360° estão no mesmo diretório.
Abra o arquivo index.html diretamente no navegador.
Componentes e Funcionalidades
a-sky: Componente A-Frame que define o panorama 360° que envolve o ambiente de visualização. Neste projeto, utiliza uma imagem esférica (Previa de teste_360_BMW_F01.jpg) para representar o interior do carro.

Câmera e Controles:

Camera: Configurada para permitir a visualização livre em 360°.
look-controls: Habilita a movimentação da câmera utilizando o mouse ou o movimento da cabeça em dispositivos de RV.
wasd-controls: Permite a navegação através das teclas de direção (W, A, S, D).
Controles de Mão:

hand-controls: Adiciona modelos de mãos interativas, configuradas como "lowPoly" e coloridas em laranja (#FF9900).
Iluminação:

Luz Ambiente (ambient light): Fornece iluminação geral suave ao ambiente.
Luz Direcional (directional light): Adiciona luz direta para melhorar o realismo e o efeito de sombreamento no ambiente.
Personalização e Extensões
Substituição da Imagem de Fundo: Para visualizar diferentes interiores de carros, substitua src de <a-sky> pela URL da nova imagem esférica.

Ajuste de Controles: Modifique os atributos look-controls e wasd-controls para ajustar a sensibilidade e a velocidade de navegação.

Adição de Modelos 3D: Utilize <a-entity obj-model="obj: url(objeto.obj); mtl: url(material.mtl)"> para adicionar modelos 3D ao ambiente.


Conclusão
Este projeto demonstra como tecnologias web modernas, como o A-Frame, podem ser utilizadas para criar experiências imersivas e interativas diretamente no navegador.
Com algumas personalizações e extensões, a mesma abordagem pode ser aplicada a uma ampla variedade de cenários, desde a visualização de produtos até a criação de tours virtuais interativos.

