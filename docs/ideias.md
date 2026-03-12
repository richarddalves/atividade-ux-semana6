# Ideias

## Ideia 1: Gráfo geográfico

### Estrutura

Nós (vértices)

- Rastreadores
- UPs

Arestas

- Conexões de estrada entre os pontos

Peso da aresta

- Tempo de deslocamento

### Como funciona

Cada base será uma área geográfica com os rastreadores e UPs representadas como territórios.

# Ideia 2: Grafo de cobertura operacional

## Estrutura

**Nós (vértices)**

- Bases operacionais
- Focos de incêndio detectados

**Arestas**

- Conexão entre uma base e um foco de incêndio que ela consegue atender

**Peso da aresta**

- Tempo estimado de resposta da base até o foco

## Como funciona

Cada foco de incêndio detectado será conectado às bases que possuem capacidade operacional para atendê-lo.

Essa capacidade pode depender de fatores como:

- distância da base até o foco
- disponibilidade de caminhões, brigadistas ou aeronaves
- acessibilidade da região

O grafo permite identificar rapidamente qual base possui o menor tempo estimado de resposta para cada ocorrência, auxiliando na decisão de qual base deve ser acionada primeiro.

# Ideia 3: Grafo de alocação de recursos

## Estrutura

**Nós (vértices)**

- Recursos disponíveis (caminhões, aeronaves, equipes)
- Ocorrências de incêndio

**Arestas**

- Conexões que indicam que um recurso pode ser utilizado para atender determinada ocorrência

**Peso da aresta**

- Custo operacional ou tempo necessário para que o recurso chegue e atue no foco

## Como funciona

Cada recurso disponível é representado como um nó no grafo e se conecta aos focos de incêndio que ele pode atender.

Essas conexões representam possibilidades de alocação de recursos.

O peso das arestas permite avaliar fatores como:

- tempo de deslocamento
- eficiência do recurso naquele tipo de ocorrência
- custo operacional

A análise do grafo permite identificar a melhor combinação de recursos para atender os incêndios ativos, otimizando o uso da frota e das equipes disponíveis.
