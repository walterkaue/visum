<!-- VISUM_TEMPLATE_3P_Insumo_v1.5 · 14-ago-2026 -->

# Insumo do 3P

**Como usar:** copie o bloco abaixo, repita uma vez por projeto, preencha depois de cada `*` e cole no chat pedindo a geração do status. O insumo preenchido não vai para a Base — é entrada de conversa.

**Regra única que não muda:** escreva por **função**, nunca por nome — de time ou de cliente. A única exceção é o campo GERENTE, que leva nome de pessoa.

**Exige `MODULO_3P` v2.0 ou superior.** Os nomes de campo mudaram na v1.5; módulo antigo com este template produz correspondência errada.

---

## Bloco para copiar

```
════════════ PROJETO ════════════
* 

──────── PROGRESSOS IMPORTANTES ────────
Até 5. Só o que terminou. Não havendo nada, escreva: sem movimento nesta semana.
* 
* 
* 

──────── PRÓXIMOS PASSOS ────────
Até 5. Cada linha com prazo e a função responsável.
* 
* 
* 

──────── PENDÊNCIAS / PONTOS DE ATENÇÃO ────────
Até 5. Dois campos por item. Impacto em branco volta como pergunta.
* SITUAÇÃO: 
  IMPACTO: 
  DECISÃO DE: 

* SITUAÇÃO: 
  IMPACTO: 
  DECISÃO DE: 

──────── PORTAL VPM ────────
Consultar hoje. Não copiar da semana passada.

Projeto já teve status gerado antes? (sim / não)
* 

Preencher sempre:
Margem Realizada
* 
Existe backlog mapeado? (sim / não)
* 
Existe proposta em negociação? (sim / não)
* 
Existe risco de relacionamento declarado? (sim / não)
* 

Preencher só se respondeu NÃO acima — projeto novo, cadastro do zero:
GERENTE (nome da pessoa)
* 
CLIENTE
* 
PROJETO (nome oficial)
* 
DATA INÍCIO (DD/MM/AAAA)
* 
DATA FIM (DD/MM/AAAA)
* 
Margem Venda
* 
Margem Prevista
* 

════════════ FIM DO PROJETO ════════════
```

---

## O que mudou na v1.5

**Os nomes dos blocos são os mesmos do Excel.** "1. O QUE FECHOU" virou PROGRESSOS IMPORTANTES, e assim por diante. Nomenclatura dupla para a mesma coisa é o primeiro lugar onde quem não construiu o sistema trava.

**Os bullets usam `*`, igual ao modelo da planilha.** Um símbolo só do insumo ao arquivo final.

**A semana saiu do insumo.** O assistente assume a semana da geração e declara em uma linha qual assumiu. Gerando fora do ritmo, corrija na resposta.

**Ponto de atenção tem dois campos, não uma linha livre.** Campo vazio se vê; frase incompleta não. Era a falha mais comum do preenchimento.

---

## Quatro coisas que fazem o status sair errado

**Progresso é o que fechou**, não o que andou. "Avançou 60%" não é progresso.

**Impacto é o que acontece se ninguém agir.** "Aguardando retorno" não é impacto; "trava o teste da jornada desde 05/08" é.

**Projeto parado continua no insumo**, com "sem movimento nesta semana". Projeto omitido some da planilha e ninguém percebe a ausência.

**Margem realizada se consulta toda sexta.** Número da semana passada não parece errado na planilha — por isso ninguém pega na revisão.

---

## O que o assistente preenche sozinho

**KPI de Renovação e KPI Geral.** Calculados a partir das respostas do bloco VPM e das margens. Ele declara em uma linha, por projeto, as duas cores e o que determinou cada uma. **Confira essa linha antes de aprovar** — é o único ponto em que você verifica a decisão dele.

**A semana de cada bloco**, a partir da data de geração.

**Cadastrais e margens de venda e prevista**, quando o projeto já teve status gerado antes. Vêm da cópia mais recente da planilha na Base.

---

## Depois de gerado

**Correção volta pelo assistente.** Precisando ajustar qualquer coisa, peça a ele e deixe que regere planilha e PPTs juntos. Editar só um dos arquivos à mão faz os dois divergirem — e a planilha corrigida vira a cópia de referência da semana seguinte, então a divergência se propaga sem aviso.
