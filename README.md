# Consumo Consciente — Semeando Futuro

Landing page institucional do projeto **Consumo Consciente**, iniciativa educacional do **Semeando Futuro**, vinculada à E.E. PEI Maria Helena Faria Lima e Cunha, em Guarulhos — SP.

> Este repositório contém a página institucional de apresentação. O aplicativo funcional é um produto separado, hospedado no Base44.

## Links oficiais

| Recurso | Endereço |
|---|---|
| Site institucional | https://consumo-consciente-page.vercel.app |
| Repositório GitHub | https://github.com/wzrichardy/consumo-consciente-page |
| Aplicativo | https://consumo-consciente.base44.app |
| Arquivo principal | [index.html](./index.html) |
| Material de referência para Notebook do Gemini | [FONTES_NOTEBOOK_GEMINI.md](./FONTES_NOTEBOOK_GEMINI.md) |

*Se o domínio público da Vercel for alterado, consulte a URL de produção exibida no painel do projeto Vercel.*

## Objetivo do projeto

Apresentar a proposta do Consumo Consciente e explicar como educação ambiental, participação da comunidade escolar, tecnologia e gestão responsável podem ser articuladas em uma iniciativa escolar.

A página funciona como porta de entrada institucional: contextualiza o desafio, apresenta os pilares ESG, descreve a proposta da plataforma e direciona o visitante ao aplicativo.

## Estrutura da página

1. **Hero / apresentação:** mensagem principal, resumo do propósito e acesso à plataforma.
2. **O desafio:** contextualização do desperdício, dos hábitos de consumo e da necessidade de participação.
3. **Nossa proposta:** apresentação da iniciativa e de sua abordagem.
4. **Pilares ESG:** dimensões ambiental, social e governança.
5. **Conheça a plataforma:** descrição de funcionalidades e mockup de celular.
6. **Diferenciais:** integração ESG, contexto escolar, participação, reflexão e tecnologia educativa.
7. **Diagnóstico:** apresentação descritiva dos dados da pesquisa realizada com a comunidade.
8. **Chamada para ação e rodapé:** acesso ao aplicativo e identificação institucional.

## Identidade visual

A interface utiliza uma linguagem visual leve, institucional e responsiva, com tons de azul e cartões arredondados.

| Token | Cor | Aplicação |
|---|---|---|
| Navy | `#1B263A` | Títulos, fundos escuros e navegação |
| Blue | `#4778B8` | Ações e elementos de destaque |
| Sky | `#8AB9F6` | Elementos suaves e fundos |
| Accent | `#679BDF` | Acentos e detalhes |

**Tipografia:** Fredoka para títulos e elementos de personalidade; DM Sans para textos corridos e interface.

## Tecnologias e arquitetura

- HTML5 semântico.
- CSS3 incorporado ao próprio `index.html`, incluindo Grid, Flexbox, variáveis CSS e media queries.
- JavaScript nativo incorporado ao HTML para menu mobile e animações de entrada por Intersection Observer.
- Google Fonts para Fredoka e DM Sans.
- Imagens hospedadas externamente no domínio do Pinterest (`i.pinimg.com`).
- Aplicativo externo hospedado no Base44.
- Publicação da landing page por integração GitHub + Vercel.

Não há framework JavaScript, gerenciador de pacotes ou etapa de compilação declarada no repositório. O ponto de entrada é `index.html`.

## Executar localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/wzrichardy/consumo-consciente-page.git
   ```
2. Abra a pasta do projeto.
3. Abra `index.html` no navegador ou utilize a extensão Live Server do Visual Studio Code.

Como é uma página estática, não é necessário instalar dependências para visualizar a versão atual.

## Publicação na Vercel

1. Acesse a Vercel e importe **exatamente** o repositório `wzrichardy/consumo-consciente-page`.
2. Confirme que o diretório raiz do projeto é a raiz do repositório.
3. Selecione **Other** como preset, caso a Vercel solicite um framework.
4. Não configure comandos de instalação ou build que não existem neste projeto.
5. Publique e confirme o domínio de produção no painel da Vercel.
6. Com a integração GitHub ativa, novos commits na branch de produção devem iniciar um novo deploy automaticamente.

A configuração efetiva de domínio, branch de produção e deploy deve ser confirmada no painel da própria Vercel.

## Dados do diagnóstico: interpretação correta

A página apresenta **221 respostas** coletadas no diagnóstico escolar:
- **103** respostas de alunos.
- **118** respostas de outros membros da comunidade escolar.

Esses números representam respostas da pesquisa diagnóstica. Não devem ser descritos como quantidade de usuários cadastrados na plataforma, amostra representativa de toda a população escolar ou comprovação de eficácia/impacto do projeto.

## Auditoria técnica — pontos de atenção

A estrutura atual é simples e adequada a uma landing page estática. Os itens abaixo devem ser considerados em futuras evoluções:

- **Imagens externas:** logo, favicon, imagem do mockup e imagem de compartilhamento dependem de URLs externas. Uma mudança ou indisponibilidade no provedor pode afetar a apresentação.
- **SEO:** já existem título, descrição e metadados Open Graph básicos. Recomenda-se adicionar URL canônica, imagem social com dimensões adequadas e metadados adicionais quando o domínio definitivo estiver confirmado.
- **Acessibilidade:** manter textos alternativos úteis para imagens informativas, contraste suficiente, foco visível, navegação por teclado e estados acessíveis do menu mobile.
- **Movimento:** a página já respeita `prefers-reduced-motion` para reduzir animações.
- **JavaScript:** o efeito de entrada utiliza `IntersectionObserver`; uma melhoria futura seria prever fallback para navegadores muito antigos e garantir que o conteúdo continue acessível caso o script falhe.
- **Conteúdo:** manter explícita a distinção entre pesquisa diagnóstica e métricas de uso ou impacto.
- **Responsividade:** testar em larguras pequenas, médias e grandes após mudanças no CSS, principalmente o mockup e os elementos posicionados absolutamente.
- **Segurança:** a landing page não implementa autenticação nem processa dados pessoais. O aplicativo Base44 é independente e deve ser auditado separadamente; não presumir que as proteções desta página se aplicam a ele.

## Escopo e limites

Este repositório não contém o backend, banco de dados, autenticação ou código-fonte do aplicativo Base44. Alterações em `index.html` afetam apenas a landing page. Para alterar funcionalidades internas do aplicativo, é necessário trabalhar no projeto correspondente.

## Manutenção

- Preserve a identidade visual e a hierarquia das seções ao alterar o layout.
- Prefira mudanças localizadas e responsivas.
- Não substitua URLs de imagens ou destinos externos sem confirmar os novos endereços.
- Após cada alteração, revise a página em desktop e mobile e confira o deploy de produção.

---

**Projeto:** Semeando Futuro — Consumo Consciente  
**Instituição:** E.E. PEI Maria Helena Faria Lima e Cunha  
**Localidade:** Guarulhos — SP  
