<!-- VISUM_GUIA_ClienteProjeto_v0.1 · 11-ago-2026 -->

# Guia de Cliente e Projeto

Este guia diz **como manter** os registros de cliente e de projeto. Ele não contém dado de cliente nenhum — os dados vivem em arquivos locais, gerados por você, que nunca são publicados.

---

## Os dois níveis

| | `VISUM_CLIENTE_[Nome]` | `VISUM_PROJETO_[Nome]` |
|---|---|---|
| **Guarda** | O que é da conta | O que é da frente de trabalho |
| **Exemplo** | `VISUM_CLIENTE_Afya` | `VISUM_PROJETO_Afya-Viva` |
| **Muda quando** | Estrutura ou contexto da conta muda | Escopo, fase ou status da frente muda |
| **Quantidade** | Um por cliente | Um por frente |

**Por que separado:** uma conta pode ter várias frentes. Modelo de negócio, glossário e quem é quem são compartilhados; escopo e status não são. Se você fundir, duplica o contexto da conta e, em alguns meses, as cópias divergem.

**O projeto herda o cliente.** Ao pedir algo sobre `Afya-Viva`, o assistente usa os dois arquivos.

---

## O que vai no arquivo de CLIENTE

**Modelo de negócio** — o que a empresa faz, como ganha dinheiro, qual o público. Duas ou três linhas bastam; serve para o assistente não escrever bobagem sobre o setor.

**Quem é quem, por função** — *nunca por nome*. "Coordenação de CRM decide sobre jornadas", "Diretoria de Marketing aprova investimento". É o que permite escrever material client-safe desde a origem.

**Glossário da conta** — nomenclaturas, siglas internas, nomes de sistemas, convenções de nomeação de DEs, automações e jornadas.

**Estrutura técnica** — nuvens contratadas, integrações existentes, particularidades de ambiente.

**Histórico relevante** — o que já foi entregue, o que deu errado antes, sensibilidades conhecidas.

---

## O que vai no arquivo de PROJETO

**Escopo** — o que está dentro e, mais importante, **o que está fora**. Escopo sem exclusão é escopo pela metade.

**Fase e cronograma** — em que ponto está, marcos, datas críticas.

**Time alocado, por função** — "um funcional sênior, um desenvolvedor pleno". Sem nomes.

**Status RAG atual** e desde quando.

**Premissas e dependências** — o que foi assumido e o que depende de terceiros. É daqui que saem os Pontos de Atenção mais úteis.

**Decisões tomadas** — o que foi decidido, quando, e o que ficou pendente.

---

## Como criar

Escreva `cadastrar projeto` no assistente. Ele gera o conteúdo dos dois arquivos (ou só o de projeto, se o cliente já existir), você salva e sobe na Base de Conhecimento.

**Você é quem salva.** O assistente gera o conteúdo; quem cria o arquivo e sobe é você.

---

## Manutenção

| Quando | O quê |
|---|---|
| **Semanal** | Status RAG e decisões novas no arquivo de projeto |
| **A cada mudança de escopo** | Atualizar escopo e premissas — e subir a versão |
| **A cada fase concluída** | Registrar o que fechou e o que ficou pendente |
| **Trimestral** | Revisar o arquivo de cliente: glossário e estrutura envelhecem |

**Versão:** ao alterar, suba o número no nome do arquivo (`v1.0` → `v1.1`) e **remova a versão antiga da Base**. Duas versões convivendo fazem o assistente responder com informação já superada.

---

## Regras fixas

1. **Nunca publique estes arquivos.** São locais, sempre. Não vão para o domínio, não vão para pasta compartilhada pública.
2. **Nunca escreva nome de pessoa** — do cliente ou do time. Sempre por função.
3. **Nunca inclua credencial, dado pessoal de titular ou informação sob NDA** que não precise estar ali.
4. **Um arquivo por conta e um por frente.** Não agrupe clientes num arquivo só.

---

*Guia v0.1 · em construção · sujeito a revisão após o piloto.*
