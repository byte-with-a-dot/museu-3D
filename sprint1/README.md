# Museu 3D

## Sobre o Projeto
Este projeto tem como objetivo realizar a digitalização em 3D do acervo do Museu Histórico Municipal Gilberto Gerlach através de técnicas de fotogrametria. O material produzido será disponibilizado em um site, permitindo acesso virtual aos objetos do museu.

O projeto é desenvolvido como parte da disciplina de Atividade de Extensão I do curso de Análise e Desenvolvimento de Dados (ADS) do Instituto Federal de Santa Catarina (IFSC), campus São José.

## Sprint 1 - Estudo das Ferramentas

Na primeira sprint, realizamos testes com as três principais ferramentas que serão utilizadas no projeto. Como objeto de teste, utilizamos uma maçã para criar um fluxo de trabalho completo desde a captura até a visualização web.

### 1. Fotogrametria com Meshroom
- Captura de 83 fotos com câmera Sony αRII
- Processamento inicial resultando em 15.655 pontos
- Geração de malha com 560.247 faces
- Identificação de problemas como textura rugosa e caule incompleto
- Documentação de parâmetros ideais para próximas capturas

### 2. Pós-processamento no Blender
- Suavização da malha para corrigir rugosidade
- Otimização usando Instant Meshes: redução para 8.271 vértices
- Simplificação da camada UV
- Criação de base metálica refletiva
- Pendência: correção do caule danificado

### 3. Visualização Web com Three.js
- Configuração do ambiente de desenvolvimento com Node.js e Vite
- Implementação inicial com cubo 3D para teste
- Adaptação do código para carregar modelos externos (.obj e .mtl)
- Configuração de iluminação com luz ambiente e direcional
- Ajustes de câmera para melhor visualização do objeto

## Estrutura do Projeto
```
/museu-3D
└── /sprint1
    ├── /meshroom
    │   └── Documentação do processo de fotogrametria
    ├── /blender
    │   └── Documentação do pós-processamento
    └── /three.js
        └── Documentação da implementação web
```

## Documentação Detalhada

### Documentação do Projeto
- [Processo de Fotogrametria com Meshroom](./sprint1/meshroom/README.md)
- [Pós-processamento no Blender](./sprint1/blender/README.md)
- [Implementação Web com Three.js](./sprint1/three.js/README.md)

### Links Úteis
#### Meshroom
- [Documentação Oficial Meshroom](https://meshroom-manual.readthedocs.io/en/latest/)
- [Tutorial Meshroom Sketchfab](https://www.youtube.com/watch?v=j3lhPKF8qjU)
- [Photogrammetry Course](https://www.youtube.com/watch?v=jI7nd2EQW1w)

#### Blender
- [Manual do Blender](https://docs.blender.org/manual/en/latest/)
- [Tutorial Blender em Português](https://www.youtube.com/watch?v=QX_D7uhqGfI)
- [Instant Meshes GitHub](https://github.com/wjakob/instant-meshes)

#### Three.js
- [Documentação Three.js](https://threejs.org/docs/)
- [Exemplos Three.js](https://threejs.org/examples/)
- [Three.js Fundamentals](https://threejsfundamentals.org/)
- [Tutorial Three.js](https://www.youtube.com/watch?v=Q7AOvWpIVHU)

## Próximos Passos
- Refinar o processo de captura fotográfica
- Desenvolver solução para o problema do caule
- Criar metodologia para objetos mais complexos
- Integrar visualização web com site principal do museu
