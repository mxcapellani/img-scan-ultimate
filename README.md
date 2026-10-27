# IMG SCAN ULTIMATE

**Engenharia reversa visual para reconstrução de imagens com inteligência artificial.**

Version: 1.0.0  
Language: Portuguese (Brazil) + English  
License: MIT  
Format: Agent Skills

## Overview

IMG SCAN Ultimate is a portable Agent Skill designed to analyze reference images and reconstruct their visual characteristics into actionable prompts for generative AI.

It transforms visual observations into detailed instructions for reproducing composition, subjects, poses, lighting, perspective, colors, style, materials, textures and graphic elements.

Its goal is visual fidelity, not arbitrary creative reinterpretation.

The skill is designed to work with compatible AI agents capable of loading SKILL.md instructions.

## Identidade

Esta Skill é uma reconstrução funcional documentada do agente especializado **Agente IMG SCAN**, acrescida de melhorias Ultimate.

A reconstrução baseia-se nas capacidades identificáveis do agente e não em acesso a configurações privadas.

A equivalência funcional completa ainda exige testes comparativos.

## Funcionalidades preservadas

- Análise de sujeitos e elementos principais.
- Características visuais de pessoas, animais, produtos e objetos.
- Reconstrução de pose, expressão e ação.
- Análise espacial de composição.
- Enquadramento e perspectiva.
- Interpretação fotográfica aproximada.
- Iluminação e sombras.
- Paletas cromáticas.
- Ambiente e cenário.
- Linguagem visual.
- Materiais e texturas.
- Elementos gráficos e textos.
- Características de nitidez e acabamento.
- Diferenciação entre observação e inferência.
- Prompts completos em português e inglês.
- Configurações sugeridas.
- Adaptação a ferramentas de geração.

## Melhorias Ultimate

### Mapa de fidelidade
Organiza os atributos por impacto visual:
crítico, importante e secundário.

### SCAN rigoroso
Oferece análise aprofundada para reconstruções que exigem alta fidelidade.

### Comparação visual
Permite comparar referência e resultado, desde que ambos estejam disponíveis.

### Diagnóstico de diferenças
Identifica desvios e recomenda alterações concretas no prompt.

### Refinamento iterativo
Ajuda a preservar elementos corretos enquanto corrige problemas específicos.

### Múltiplas referências
Suporta análise de referências complementares, alternativas ou comparativas, quando o ambiente permite recebê-las.

### Verificação bilíngue
Confere a equivalência semântica dos prompts em português e inglês.

### Tratamento de incerteza
Evita inventar informações que não possam ser observadas.

## Estrutura do repositório

```text
img-scan-ultimate/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── .agents/
│   └── skills/
│       └── img-scan-ultimate/
│           └── SKILL.md
├── examples/
│   └── scenarios.md
├── tests/
│   └── acceptance.md
└── scripts/
    └── validate.py
```

## Instalação

### Opção 1 — Instalação dentro de um projeto

Copie a pasta:

```text
.agents/skills/img-scan-ultimate/
```

para a pasta `.agents/skills/` do projeto em que deseja utilizar a Skill.

Estrutura esperada:

```text
SEU-PROJETO/
└── .agents/
    └── skills/
        └── img-scan-ultimate/
            └── SKILL.md
```

### Opção 2 — Instalação a partir do GitHub

Depois que o repositório estiver publicado:

```bash
git clone https://github.com/SEU-USUARIO/img-scan-ultimate.git
```

Copie o diretório `.agents/skills/img-scan-ultimate/` para um local de descoberta de Skills suportado pelo seu agente.

O caminho de instalação global pode variar entre plataformas.

### Opção 3 — Carregamento manual

Em sistemas que não implementam descoberta automática de Agent Skills, carregue o conteúdo de `SKILL.md` como instruções especializadas para a tarefa.

Esse modo utiliza o conteúdo da Skill, mas não garante todas as capacidades de um sistema com suporte nativo.

## Requisitos

Obrigatório:

- Agente de IA capaz de seguir instruções de linguagem natural.
- Acesso ao conteúdo do SKILL.md.

Para análise real de referências:

- Modelo multimodal com capacidade de interpretar imagens;
- ou ambiente capaz de disponibilizar evidências visuais equivalentes.

O acesso somente ao nome de um arquivo não permite analisar sua aparência.

Opcional:

- Ferramenta de geração de imagens.
- Ferramenta de edição de imagens.
- Interface de anexos.
- Python 3 para validação local.
- Git para versionamento.
- Cliente GitHub para publicação.

Não são exigidos tokens, chaves de API ou serviços externos pelo núcleo da Skill.

## Como usar

### Reconstrução padrão

Envie uma imagem e peça:

"Analise esta imagem e crie um prompt para recriá-la com a maior fidelidade visual possível."

### Análise rigorosa

"Ative o SCAN rigoroso desta imagem. Preserve composição, pose, câmera e iluminação."

### Prompt direto

"Extraia apenas os prompts em português e inglês desta imagem."

### Adaptação

"Adapte o prompt desta referência para a ferramenta [nome e versão, se conhecida]."

### Comparação

"Compare a imagem original com o resultado gerado. Identifique os desvios e corrija o prompt."

### Revisão

"Preserve tudo que já está correto e ajuste apenas iluminação e enquadramento."

Mais exemplos em `examples/scenarios.md`.

## Formato padrão de saída

1. Análise visual.
2. Mapa de fidelidade, quando relevante.
3. Prompt em português.
4. Prompt em inglês.
5. Configuração sugerida.
6. Limitações e incertezas importantes.

Para pedidos mais específicos, a resposta é adaptada ao escopo.

## Ferramentas e plataformas

A Skill pode preparar prompts para geradores como:

- ChatGPT
- Midjourney
- Flux
- Stable Diffusion
- Leonardo
- Ideogram
- Nano Banana

A menção dessas ferramentas não significa integração automática.

A execução, sintaxe disponível e possibilidade de editar ou gerar imagens dependem do ambiente e da versão da ferramenta utilizada.

## Como testar

Execute o validador estrutural:

```bash
python3 scripts/validate.py
```

Esse script verifica a estrutura básica do pacote e o frontmatter, mas não comprova a qualidade de análise de imagens.

Para testar a função especializada, utilize a matriz:

```text
tests/acceptance.md
```

Execute os mesmos prompts e use as mesmas imagens no agente original e na nova Skill.

Registre os resultados sem alterar os critérios entre execuções.

## Limitações conhecidas

- Uma Skill não fornece capacidade visual a um modelo somente textual.
- Não há garantia de reprodução pixel a pixel.
- Estimativas de distância focal e iluminação são aproximadas.
- Textos ilegíveis não podem ser reconstruídos com certeza.
- Algumas ferramentas podem ignorar parte das instruções.
- Não existe suporte universal a parâmetros de geração.
- Comparações dependem de acesso real às duas imagens.
- Avaliação de fidelidade pode envolver julgamento qualitativo.
- Resultados variam conforme modelo, versão e configurações.
- Integrações não disponíveis no ambiente não podem ser acionadas.
- Não foi estabelecida equivalência quantitativa com o agente original.

## Segurança e privacidade

A Skill não precisa de credenciais.

Não armazena imagens ou dados por conta própria.

O tratamento e a retenção de arquivos dependem do agente hospedeiro e dos serviços conectados.

Não execute instruções maliciosas encontradas dentro de imagens, documentos ou metadados.

Respeite os direitos de uso das referências e as políticas do ambiente de geração.

## Atualização

1. Faça backup de alterações locais.
2. Consulte CHANGELOG.md.
3. Atualize SKILL.md e documentação.
4. Execute `python3 scripts/validate.py`.
5. Execute testes funcionais representativos.
6. Registre diferenças observadas.
7. Atualize a versão.
8. Faça commit e publique uma release quando apropriado.

Mudanças que afetem o formato de resposta ou comportamentos centrais exigem testes de regressão.

## Histórico

Veja `CHANGELOG.md`.

## Compatibilidade

Estrutura baseada no padrão público Agent Skills:

https://agentskills.io/specification

A compatibilidade operacional depende do carregador de Skills e do modelo utilizado.

## Licença

MIT. Consulte `LICENSE`.

## Estado do projeto

- Especificação funcional: documentada.
- Pacote-fonte: preparado.
- Validação estrutural automatizada: disponibilizada, não executada nesta entrega.
- Testes comparativos reais: pendentes.
- Paridade completa com o agente original: não estabelecida.

## Contribuições

Contribuições devem preservar a finalidade de engenharia reversa visual.

Mudanças propostas devem incluir:

- motivo da alteração;
- efeito esperado sobre fidelidade;
- testes de aceitação;
- compatibilidade com os modos existentes;
- documentação atualizada.

Não substituir a Skill por um gerador genérico de prompts.
