# IMG SCAN Ultimate — Cenários de utilização

Este documento demonstra como utilizar a Skill em diferentes condições.

Os cenários ilustrativos não representam imagens efetivamente verificadas.

## Exemplo 1 — Retrato fotográfico

### Referência

Imagem de teste com:
- uma pessoa centralizada;
- enquadramento do peito para cima;
- fundo escuro e desfocado;
- luz suave lateral;
- vestuário preto;
- expressão neutra.

### Solicitação

"Analise esta imagem e gere um prompt para recriá-la com máxima fidelidade."

### Resultado esperado

Análise:
- um sujeito;
- enquadramento de retrato;
- posição central;
- postura e expressão;
- fundo escuro;
- iluminação lateral;
- profundidade de campo reduzida.

Prompt ilustrativo PT:

"Retrato fotográfico de uma única pessoa
centralizada no quadro, enquadrada do peito
para cima, utilizando roupa preta, expressão
neutra e postura frontal. Fundo escuro,
uniforme e desfocado, com separação visual
entre sujeito e cenário. Iluminação suave
vinda de um dos lados, produzindo transição
gradual de luz e sombra sobre o rosto.
Perspectiva natural de retrato, foco
prioritário no rosto, profundidade de campo
reduzida, cores discretas e acabamento
fotográfico realista. Composição vertical."

Prompt ilustrativo EN:

"Photographic portrait of a single person
centered in the frame, cropped from the
chest upward, wearing black clothing,
with a neutral expression and frontal
posture. Dark, uniform, softly blurred
background, visually separating the
subject from the scene. Soft lighting
coming from one side, creating a gradual
transition between light and shadow across
the face. Natural portrait perspective,
primary focus on the face, shallow depth
of field, subdued colors and a realistic
photographic finish. Vertical composition."

Nota: a direção específica da luz depende da
imagem efetivamente apresentada.

## Exemplo 2 — Produto publicitário

### Referência

Fotografia com:
- uma embalagem cilíndrica;
- superfície metálica;
- produto em primeiro plano;
- fundo de cor única;
- sombra definida;
- reflexos verticais.

### Solicitação

"Faça a engenharia reversa desta fotografia de produto."

### Resultado esperado

A análise deve contemplar:
- formato geométrico;
- proporção altura/largura;
- acabamento e reflexos;
- posição do produto;
- superfície de apoio;
- distribuição da sombra;
- fundo;
- perspectiva;
- tipografia, quando legível.

Não inventar nome ou marca da embalagem.

## Exemplo 3 — Cena cinematográfica

### Solicitação

"Ative o SCAN rigoroso.
Reconstrua a cena com atenção especial
ao enquadramento, câmera, iluminação
e organização dos elementos."

### Resultado esperado

O agente deverá:
1. identificar todos os sujeitos principais;
2. separar camadas de profundidade;
3. reconstruir o eixo de câmera;
4. examinar fontes aparentes de luz;
5. mapear atributos críticos;
6. produzir os dois prompts;
7. registrar informações incertas.

Não presumir modelo de câmera ou lente exata.

## Exemplo 4 — Cartaz tipográfico

### Solicitação

"Extraia um prompt fiel deste cartaz.
Preserve a hierarquia visual e transcreva
somente os textos realmente legíveis."

### Resultado esperado

O agente deverá identificar:
- área da composição;
- texto principal;
- textos secundários;
- alinhamento;
- tipografia aproximada;
- distribuição de cores;
- relação texto/imagem;
- eventuais cortes e oclusões.

Textos ilegíveis devem permanecer marcados
como ilegíveis, sem preenchimento inventado.

## Exemplo 5 — Adaptação para plataforma

### Solicitação

"Adapte o prompt da imagem enviada
para Midjourney, preservando a composição."

### Resultado esperado

- Prompt especializado.
- Elementos visuais preservados.
- Nenhuma sintaxe de versão presumida.
- Informação sobre dependência da versão
  para parâmetros específicos.
- Conteúdo visual equivalente ao universal.

## Exemplo 6 — Comparação entre resultado e referência

### Entradas

Imagem A: referência.
Imagem B: resultado gerado.

### Solicitação

"Compare as duas imagens e identifique
por que o resultado está visualmente
diferente da referência."

### Resultado esperado

Diagnóstico estruturado:
- diferenças de composição;
- diferenças de pose;
- diferenças de perspectiva;
- diferenças de iluminação;
- diferenças cromáticas;
- diferenças de fundo;
- prioridades de correção;
- prompt revisado PT/EN.

Não inventar diferenças não observadas.

## Exemplo 7 — Refinamento incremental

### Solicitação

"Preserve a pose, o rosto e o enquadramento.
Ajuste somente a direção da luz para
aproximar o resultado da referência."

### Resultado esperado

Preservar:
- sujeito;
- pose;
- composição;
- perspectiva.

Modificar:
- iluminação, quando justificado.

Não redesenhar a cena completa.

## Exemplo 8 — Referência incompleta

### Solicitação

"Recrie esta imagem borrada com fidelidade."

### Resultado esperado

- Analisar os elementos identificáveis.
- Explicar quais atributos são incertos.
- Produzir os prompts possíveis.
- Evitar inventar microdetalhes.
- Solicitar imagem melhor somente quando
  indispensável à tarefa.

## Exemplo 9 — Nenhuma imagem

### Solicitação

"Transforme a imagem em prompt."

### Resultado esperado

"Envie a imagem de referência para
que eu possa analisá-la e reconstruir
o prompt com fidelidade."

Não criar características imaginárias.

## Exemplo 10 — Análise parcial

### Solicitação

"Analise somente a câmera e a iluminação
desta imagem. Não preciso de um prompt."

### Resultado esperado

- Perspectiva;
- enquadramento;
- comportamento da lente, quando inferível;
- fontes aparentes de luz;
- qualidade de sombras;
- limitações da estimativa.

Não incluir prompts desnecessários.

## Exemplo 11 — Duas referências complementares

### Solicitação

"Use a primeira imagem como referência
de composição e a segunda apenas como
referência de iluminação."

### Resultado esperado

- Separar papéis das imagens.
- Preservar geometria da primeira.
- Transferir apenas características
  relevantes de iluminação da segunda.
- Explicitar essa combinação.
- Produzir prompts bilíngues.

## Exemplo 12 — Texto ilegível

### Solicitação

"Recrie o anúncio e preserve exatamente
o texto da embalagem."

### Condição

Parte do texto não está legível.

### Resultado esperado

- Transcrever somente o legível.
- Identificar o conteúdo indeterminável.
- Não completar textos por adivinhação.
- Recomendar referência de maior resolução.
- Preservar a geometria e a área gráfica.

## Exemplos de início de conversa propostos

Estes são atalhos sugeridos para a Skill,
não alegações sobre a configuração do GPT original.

1. "Analise esta imagem e gere prompts PT/EN."
2. "Faça um SCAN rigoroso desta referência."
3. "Extraia um prompt para Midjourney."
4. "Compare esta imagem com o resultado gerado."
5. "Corrija meu prompt para aumentar a fidelidade."
6. "Reconstrua a iluminação e a composição."
7. "Analise apenas as características fotográficas."
8. "Identifique os elementos mais importantes
   para reproduzir esta imagem."

## Orientação para novos exemplos

Ao adicionar exemplos ao repositório:
- não inventar resultados de testes;
- identificar imagens usadas;
- registrar permissão para distribuição;
- separar entrada, resposta esperada e resultado;
- evitar dados pessoais desnecessários;
- manter a especialidade de engenharia reversa.
