# Plano — novo site EJR Robótica Educacional

Proposta de redesenho de https://ejrrobotica.com.br/ (hoje em WordPress, uma página longa).
Esta é a v1: estática, sem build, abre direto no navegador e no GitHub Pages.

## Conceito

**"Programe antes de ler."** A primeira coisa que o visitante vê é a arena verde
dos robôs da EJR (a mesma da foto da turma) com um robô que ele programa na hora,
usando o vocabulário dos próprios jogos da EJR: **PF** (para frente), **PT** (para trás),
**PE** (gira à esquerda), **PD** (gira à direita). O visitante monta a sequência,
aperta Executar e leva o robô até os três alvos. Em 20 segundos ele entendeu o
produto sem ler um parágrafo — e o coordenador pedagógico entende o que a turma
vai viver.

O resto da página é calmo e direto: catálogo de kits com orçamento por WhatsApp,
as três plataformas, a foto real da turma e os contatos.

## Público e objetivo

- Coordenaçêo pedagógica e direçêo de escolas (decide a compra/contrataçêo).
- Professores e instrutores (usam kits, formaçêo e plataformas).
- Pais e alunos (aulas, EJR Games).
- Objetivo principal da página: **pedido de orçamento pelo WhatsApp**, já com o nome do kit.

## Identidade (tokens)

Tudo sai do logo: blocos laranja/verde/azul com contorno preto grosso.

| token | valor | uso |
|---|---|---|
| `--ink` | `#000000` | contornos, texto |
| `--paper` | `#FFFFFF` | fundo geral |
| `--orange` | `#FF5A1F` | E do logo, botões primários |
| `--green` | `#22C93B` | J do logo, sucesso |
| `--blue` | `#1E8FFF` | R do logo, links e plataformas |
| `--mat` | `#13803A` | arena (tapete verde) |
| `--robot` | `#FFC21A` | corpo do robô (os robôs amarelos da foto) |

- Tipografia: **Bricolage Grotesque** (títulos, robusta e brincalhona) +
  **Atkinson Hyperlegible** (texto; criada para legibilidade, bom para escola).
- Linguagem visual: "adesivo" — contorno preto de 3px e sombra dura deslocada,
  igual ao logo. Sem gradiente, sem sombra borrada.
- Fundo claro de propósito: o logo tem traço preto (a lâmpada some em fundo escuro).

## Estrutura da página

1. **Topo fixo** — logo, Kits, Plataformas, Contato, botêo WhatsApp.
2. **Arena** (hero) — título, frase, botões "Pedir orçamento" e "Ver kits"; à direita
   a arena 6×6 programável. Teclado e celular funcionam; `prefers-reduced-motion` respeitado.
3. **O que a EJR faz** — Aulas, Vendas, Assessoria, Formaçêo.
4. **Kits** — os 7 kits do site atual, com filtro por tipo (robô, placa, jogo, desplugado)
   e botêo de orçamento que abre o WhatsApp com o nome do kit.
5. **Plataformas** — EJR Hub, Jabuti Edu Nuvem, EJR Games (Trilogia Barco Robô Amazônia).
6. **Turma** — a foto real dos robôs na arena.
7. **Contato** — WhatsApp/Telegram/telefone, e-mail, Instagram, Facebook e os 4 formulários
   (Enviar trabalho, Avaliar EJR Games, Trabalhe conosco, EJR Promo).

## Regra de conteúdo

Só fatos que já estêo no site atual. Nada de depoimentos, números, preços ou
equipe inventados. Lacunas estêo marcadas no HTML como `<!-- TODO EJR: ... -->`.

## O que a EJR precisa mandar (pendências de conteúdo)

- [ ] Fotos de cada um dos 7 kits (hoje o site usa ilustraçêo por tipo).
- [ ] Uma frase por kit: faixa etária/série, o que vem na caixa.
- [ ] Texto curto de cada serviço (Aulas, Vendas, Assessoria, Formaçêo).
- [ ] Cidade/regiêo atendida e endereço (se quiserem mostrar).
- [ ] Fotos de turma com autorizaçêo de imagem (mais de uma).
- [ ] Domínio: apontar ejrrobotica.com.br para o novo site quando aprovado.

## Fora da v1 (próximas etapas)

- Página por kit (com galeria e ficha técnica).
- Blog/novidades e área de eventos (Mostratec, torneios de sumô).
- Versões EN/ES, se houver mercado fora do Brasil.
- Formulário de orçamento próprio (hoje vai direto ao WhatsApp, sem backend).

## Arquivos

- `index.html` — a página.
- `assets/css/style.css` — estilos e tokens.
- `assets/js/arena.js` — a arena programável.
- `assets/img/` — imagens do site atual (logo com fundo removido, foto da turma, telas das plataformas).
