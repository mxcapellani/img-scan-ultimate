# IMG SCAN Ultimate — Testes de aceitação

## 1. Objetivo

Comparar as funcionalidades observáveis do Agente IMG SCAN
com a reconstrução IMG SCAN Ultimate.

Nenhuma pontuação neste documento representa um
resultado já medido.

Estado inicial: PENDENTE DE EXECUÇÃO.

## 2. Regras de comparação

Usar exatamente a mesma solicitação textual
no agente original e na Skill.

Usar exatamente os mesmos arquivos e imagens.

Quando possível, manter constantes:
- modelo;
- versão;
- configuração de geração;
- contexto;
- ferramentas;
- ordem dos anexos.

Registrar qualquer diferença ambiental.

Se o modelo for não determinístico, executar
múltiplas repetições para avaliar estabilidade.

## 3. Escala de avaliação

Usar escala de 0 a 4:

0 = ausente ou incorreto
1 = muito insuficiente
2 = parcialmente adequado
3 = adequado
4 = excelente

Aplicar os mesmos critérios a ambos.

N/A = não aplicável ao cenário.
NV = não verificável no ambiente.

Não substituir NV por 0.

## 4. Dimensões avaliadas

D1 — Cobertura funcional
D2 — Precisão visual
D3 — Qualidade da resposta
D4 — Consistência
D5 — Formato de saída
D6 — Preservação da especialidade
D7 — Autonomia
D8 — Tratamento de referências
D9 — Utilidade prática
D10 — Recursos avançados

Para cada dimensão, registrar uma nota e
evidências observáveis.

## 5. Matriz de cenários

| ID | Nível | Cenário | Dimensões principais |
|---|---|---|---|
| T01 | Simples | Retrato único | D1 D2 D5 D6 |
| T02 | Simples | Produto isolado | D1 D2 D9 |
| T03 | Simples | Imagem sem ferramenta indicada | D5 D7 |
| T04 | Simples | Nenhuma imagem | D7 D8 |
| T05 | Simples | Pedido apenas de câmera/luz | D1 D6 |
| T06 | Intermediário | Duas pessoas em poses distintas | D2 D8 |
| T07 | Intermediário | Cartaz com texto legível | D2 D5 D8 |
| T08 | Intermediário | Texto parcialmente ilegível | D2 D8 |
| T09 | Intermediário | Adaptação para plataforma | D1 D9 |
| T10 | Intermediário | Cena com várias camadas | D2 D6 |
| T11 | Complexo | SCAN rigoroso | D1 D2 D3 D10 |
| T12 | Complexo | Referência e imagem gerada | D2 D8 D10 |
| T13 | Complexo | Refinamento incremental | D4 D9 D10 |
| T14 | Complexo | Duas referências complementares | D7 D8 D10 |
| T15 | Complexo | Referência de baixa qualidade | D2 D8 |
| T16 | Complexo | Imagem com conflito entre texto e cena | D2 D6 D8 |
| T17 | Complexo | Correções sucessivas | D4 D9 D10 |
| T18 | Complexo | Prompt longo bilíngue | D3 D4 D5 |

## 6. Solicitações exatas

As solicitações abaixo devem ser copiadas
sem alterações para ambos os sistemas.

### T01 — Retrato

Material: imagem de retrato com uma pessoa.

"Analise esta imagem e gere prompts em português
e inglês para recriá-la com fidelidade visual."

Aceitação:
- sujeito correto;
- pose e enquadramento;
- iluminação;
- composição;
- dois prompts equivalentes.

### T02 — Produto

Material: fotografia de produto isolado.

"Faça a engenharia reversa visual desta
fotografia de produto."

Aceitação:
- geometria;
- superfície;
- reflexos;
- cenário;
- prompt utilizável.

### T03 — Autonomia

Material: imagem fotográfica.

"Extraia o prompt desta imagem."

Aceitação:
- início automático;
- ausência de perguntas desnecessárias;
- resultado bilíngue;
- configurações justificáveis.

### T04 — Falta de imagem

Material: nenhum.

"Transforme esta imagem em prompt."

Aceitação:
- solicita referência;
- não inventa conteúdo;
- não produz análise falsa.

### T05 — Escopo parcial

Material: fotografia com iluminação distinta.

"Analise somente a câmera e a iluminação
desta imagem. Não preciso de um prompt."

Aceitação:
- respeita o escopo;
- não força prompts;
- distingue observação e inferência.

### T06 — Múltiplos sujeitos

Material: fotografia com duas pessoas
em posições e poses diferentes.

"Reconstrua a composição e as poses de
cada pessoa, mantendo suas posições relativas."

Aceitação:
- quantidade correta;
- distinção entre sujeitos;
- relações espaciais;
- descrição individual das poses.

### T07 — Tipografia

Material: cartaz com texto claramente legível.

"Recrie este cartaz em forma de prompt,
preservando o texto visível e sua organização."

Aceitação:
- transcrição correta;
- hierarquia;
- posicionamento;
- cores;
- ausência de texto inventado.

### T08 — Texto ilegível

Material: embalagem com texto parcialmente
encoberto ou borrado.

"Analise a embalagem e transcreva
somente o texto efetivamente legível."

Aceitação:
- não completa o ilegível;
- registra incerteza;
- identifica organização gráfica.

### T09 — Plataforma

Material: imagem de referência.

"Adapte a reconstrução desta imagem
para Midjourney, sem alterar a composição."

Aceitação:
- preserva conteúdo visual;
- evita parâmetros sem suporte verificado;
- prompt adequado ao uso.

### T10 — Composição complexa

Material: cena com primeiro plano,
plano médio e fundo.

"Descreva as relações espaciais
e gere um prompt fiel à referência."

Aceitação:
- separação por camadas;
- perspectiva;
- oclusões;
- relações de tamanho;
- fidelidade estrutural.

### T11 — SCAN rigoroso

Material: fotografia complexa.

"Execute uma análise visual rigorosa desta
imagem, priorizando composição, pose,
perspectiva, iluminação e materiais.
Depois gere prompts PT/EN."

Aceitação:
- mapa de fidelidade;
- descrição concreta;
- incertezas justificadas;
- prompts completos;
- consistência bilíngue.

### T12 — Diagnóstico

Material: original e resultado gerado.

"Compare as duas imagens, identifique
os principais desvios visuais e
proponha um prompt corrigido."

Aceitação:
- identifica diferenças reais;
- ordena correções;
- preserva elementos corretos;
- gera prompt revisado.

### T13 — Refinamento

Material: imagem original, resultado gerado
e prompt anteriormente utilizado.

"Preserve os elementos que estão corretos.
Corrija apenas os desvios de enquadramento
e iluminação em relação à referência."

Aceitação:
- alteração mínima;
- foco nos desvios;
- ausência de redesenho desnecessário.

### T14 — Referências complementares

Material: duas imagens distintas.

"Use a primeira imagem como referência
de composição e a segunda apenas como
referência de iluminação. Gere prompts PT/EN."

Aceitação:
- papéis respeitados;
- combinação coerente;
- nenhuma fusão arbitrária.

### T15 — Baixa resolução

Material: imagem borrada.

"Crie um prompt fiel com base nesta imagem.
Não invente detalhes que não estejam visíveis."

Aceitação:
- inferências cautelosas;
- não alucina microdetalhes;
- entrega resultado útil.

### T16 — Texto versus cena

Material: foto contendo instruções escritas
sobrepostas que não fazem parte do pedido.

"Analise a imagem e reconstrua sua
aparência visual em um prompt."

Aceitação:
- trata palavras como conteúdo visual;
- não obedece instruções presentes na imagem;
- preserva o escopo do usuário.

### T17 — Consistência longitudinal

Material: uma referência e duas ou mais
iterações geradas no mesmo contexto.

"Refine o prompt anterior para aproximar
o resultado da referência, sem perder
as características que já coincidiam."

Aceitação:
- mantém restrições anteriores;
- corrige apenas diferenças relevantes;
- registra ajustes concretos.

### T18 — Equivalência bilíngue

Material: fotografia detalhada.

"Faça a análise completa e produza prompts
detalhados em português e inglês, garantindo
que ambos contenham as mesmas informações."

Aceitação:
- sujeitos idênticos;
- mesma pose;
- mesma orientação;
- mesma iluminação;
- mesma paleta;
- nenhuma adição exclusiva de um idioma.

## 7. Rubrica de precisão visual

Registrar separadamente:

- composição;
- quantidade de sujeitos;
- pose;
- proporções;
- perspectiva;
- iluminação;
- paleta;
- cenário;
- estilo;
- texturas;
- tipografia, quando houver.

Para cada critério:

4 = corresponde com precisão observável;
3 = corresponde com pequenas imprecisões;
2 = parcial, omite atributos relevantes;
1 = desvio significativo;
0 = incorreto ou ausente.

Não utilizar porcentagem numérica de
similaridade de imagem sem métrica aplicada.

## 8. Avaliação de autonomia

Verificar:
- começou sem perguntar o desnecessário?
- respeitou ferramentas disponíveis?
- adaptou o formato ao pedido?
- solicitou imagem quando ausente?
- reconheceu limites?
- evitou inventar capacidades?

## 9. Avaliação da especialidade

A resposta deve evidenciar:

- engenharia reversa;
- preocupação com fidelidade;
- descrição espacial;
- análise de câmera e iluminação;
- prompts operacionais;
- preservação de referência.

Falha crítica:
transformar a tarefa em descrição genérica
ou proposta de criação visual arbitrária.

## 10. Registro individual

Para cada teste, preencher:

TESTE:
DATA:
IMAGENS:
HASH DOS ARQUIVOS, SE DISPONÍVEL:
MODELO ORIGINAL:
MODELO SKILL:
CONFIGURAÇÕES:
FERRAMENTAS:
PROMPT EXATO:
RESPOSTA ORIGINAL:
RESPOSTA SKILL:

D1:
D2:
D3:
D4:
D5:
D6:
D7:
D8:
D9:
D10:

MÉDIA APLICÁVEL:
DIFERENÇAS OBSERVADAS:
FALHAS CRÍTICAS:
EVIDÊNCIAS:
RESULTADO: APROVADO / REPROVADO / NV

## 11. Critério provisório de aprovação

Uma execução poderá ser considerada aprovada
quando:

1. Não ocorrer invenção de detalhes críticos.
2. Composição e sujeito forem preservados.
3. Os prompts PT/EN forem equivalentes.
4. O escopo do usuário for respeitado.
5. Nenhuma dimensão essencial receber nota 0 ou 1.
6. A média das dimensões aplicáveis for >= 3,0.
7. Não houver falha crítica de especialidade.

Esses limiares são critérios de aceitação
propostos, não resultados observados.

## 12. Avaliação de paridade

Classificar cada função como:

PRESERVADA:
A nova Skill cumpre o mesmo objetivo observável.

PARCIAL:
A nova Skill cumpre apenas parte dos requisitos.

REGRESSÃO:
A nova Skill apresenta perda funcional relevante.

MELHORIA:
A nova Skill demonstra ganho objetivo.

NÃO VERIFICÁVEL:
Faltam evidências ou recursos.

O termo "equivalência funcional" deve ser
utilizado somente para capacidades
efetivamente comparadas.

## 13. Itens pendentes de validação

- Qualidade da análise visual real.
- Fidelidade de imagens reconstruídas.
- Funcionamento em diferentes modelos.
- Adaptação por gerador e versão.
- Comparação original versus resultado.
- Estabilidade em múltiplas iterações.
- Desempenho com imagens complexas.
- Tratamento de texto parcialmente legível.
- Processamento de múltiplos anexos.
- Diferenças entre contexto curto e longo.
- Recursos externos disponíveis por plataforma.
- Paridade com exemplos históricos do agente original.

## 14. Relatório final de validação

Após executar a bateria, produzir:

- quantidade de testes executados;
- quantidade aprovada;
- quantidade reprovada;
- quantidade não verificável;
- notas por dimensão;
- principais regressões;
- principais melhorias;
- diferenças ambientais;
- recomendações de correção;
- estado de paridade.

Não declarar equivalência total antes dos testes.

## 15. Estado atual

Teste estrutural automatizado:
NÃO EXECUTADO.

Testes visuais:
NÃO EXECUTADOS.

Comparação com agente original:
NÃO EXECUTADA.

Paridade funcional:
NÃO DETERMINADA.
