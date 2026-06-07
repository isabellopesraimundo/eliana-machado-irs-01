# INSTRUÇÕES DE CORREÇÃO NO DRAKE
## ELIANA MACHADO DE ALMEIDA — FORM 1040-X DE 2024
## Preparado para: Isabel Raimundo, EA | Data: 7 de junho de 2026

---

## PARTE 1 — RESPOSTAS ÀS SUAS PERGUNTAS

### P1: Posso apresentar uma declaração retificadora (Form 1040-X) DURANTE uma auditoria ativa do IRS?

**SIM. Você pode e deve apresentar o Form 1040-X agora, antes que o IRS emita um ajuste proposto.**

Veja exatamente como funciona no âmbito do procedimento tributário norte-americano:

**Estágio atual desta auditoria:** A Carta 566-T (Letter 566-T) é uma "exame por correspondência" no estágio mais inicial. Nenhuma deficiência foi proposta ainda. O IRS está simplesmente solicitando documentação.

**O que você pode fazer agora:**
1. Responder à Letter 566-T com o pacote de defesa da auditoria (já preparado).
2. Na carta de apresentação, informar ao examinador que você está concedendo o excesso declarado e corrigiu a declaração no Drake.
3. Incluir o Form 14900 preenchido com a resposta.
4. Apresentar (ou oferecer-se para apresentar) o Form 1040-X com os valores corrigidos.

**Você NÃO precisa aguardar** que o IRS conclua sua revisão. Na verdade, apresentar proativamente:
- Demonstra conformidade voluntária e boa-fé
- Pode resultar em redução de penalidades
- Frequentemente leva o examinador a encerrar o caso mais rapidamente
- Evita que o IRS emita um ajuste proposto formal (o que desencadeia um processo mais formal)

---

### P2: O que acontece se você aguardar em vez de agir agora?

| Ação | O Que Acontece |
|--------|-------------|
| **Agir agora (apresentar o Form 1040-X + responder à Letter 566-T)** | O examinador do IRS poderá aceitar as concessões e encerrar o caso. Resolução mais rápida. |
| **Aguardar a revisão do IRS** | O IRS emite um relatório de exame (carta de 30 dias) propondo o ajuste. Eliana terá então 30 dias para concordar ou contestar. Processo mais formal e demorado. |
| **Não responder** | O IRS desconsidera toda a dedução e emite uma cobrança de imposto. Pior desfecho. |

**Recomendação:** Responder à Letter 566-T até 17 de junho de 2026 com o pacote da auditoria. Declarar claramente na carta de apresentação que você concede o excesso declarado e incluir o Form 14900 corrigido.

---

### P3: Procedimento no Drake — Deve-se corrigir no Drake e preparar um Form 1040-X?

**Sim.** Veja o processo:
1. Fazer as correções no Drake (instruções abaixo).
2. O Drake gerará automaticamente os valores corrigidos do Form 1040.
3. Abrir o módulo **Form 1040-X** no Drake e ele importará os valores originais e corrigidos.
4. Imprimir o Form 1040-X para Eliana assinar.
5. O Form 1040-X deve ser **enviado pelo correio** (declaração em papel) — não pode ser transmitido eletronicamente nesta situação, pois a declaração original foi transmitida eletronicamente e um Form 1040-X durante um exame de auditoria ativa é tipicamente enviado diretamente ao escritório de exame, e não ao centro de serviço normal do Form 1040-X, salvo instrução em contrário do examinador.

**Observação:** Anexar o Form 14900 ao Form 1040-X como documento de suporte.

---

---

## PARTE 2 — INSTRUÇÕES DE CORREÇÃO NO DRAKE

### O QUE MUDOU E POR QUÊ

Dois erros foram identificados na declaração original:

| Erro | Original | Corrigido | Fundamentação |
|-------|----------|-----------|-----------|
| Limite de empréstimo do IRC §163(h) não aplicado | $114.034 deduzidos | $77.409 dedutíveis | IRC §163(h)(3)(B) / Form 14900 |
| Pontos hipotecários (points) do Radius tratados como integralmente dedutíveis | $18.900 em 2024 | ~$67 em 2024 (amortizados) | IRC §461(g)(2) / Pub. 936 |
| Juros do Radius ($1.870) excluídos do Schedule A | $0 incluído | Incluído no Form 14900 | Forms 1098 |

---

### PASSO 1 — ABRIR A DECLARAÇÃO DE 2024 DE ELIANA NO DRAKE
Arquivo: MACHADO DE ALMEIDA, ELIANA | SSN: 697-75-6336

---

### PASSO 2 — CORRIGIR O LANÇAMENTO DO Form 1098 DO RADIUS
**Caminho no Drake:** Data Entry → Form 1098 → Record 2 of 2 (Radius Financial Group)

**Problema identificado:** O campo "Deductible amount, if different" ao lado do Box 1 exibe **0**.
Este zero substitui os juros de $1.869,86 e instrui o Drake a transportar $0 para o Schedule A.

**Ação necessária:**

| Campo | Valor Atual | Alterar Para |
|-------|--------------|-----------|
| Box 1 — Mortgage interest received | 1870 | Manter como está (correto) |
| **"Deductible amount, if different" (ao lado do Box 1)** | **0** | **EXCLUIR O ZERO — deixar EM BRANCO** |
| Box 2 — Outstanding principal | 840000 | Manter como está |
| Box 3 — Origination date | 11-13-2024 | Manter como está |
| Box 6 — Points | 18900 | Manter como está (valor correto) |

**Justificativa:** Ao limpar o 0, o Drake utilizará o valor real do Box 1 ($1.870) e o incluirá no cálculo do Schedule A.

**Também necessário — informar ao Drake que o empréstimo do Radius é um REFINANCIAMENTO:**
No lançamento do Form 1098 do Radius no Drake, procure um campo ou caixa de seleção que questione a natureza do empréstimo. O rótulo do Box 6 indica "Points paid on purchase of principal residence" — porém trata-se de um REFINANCIAMENTO, não de uma compra. É necessário indicar isso no Drake para que os pontos hipotecários (points) sejam amortizados em vez de deduzidos integralmente.

No Drake 2024, procure por:
- Um botão de opção ou caixa de seleção próximo ao Box 6 com a indicação "Refinance" ou que questione se trata-se de um empréstimo para compra
- OU o link "Loan Limit Worksheet" no canto superior direito da tela de lançamento do Form 1098 — clique para abrir a planilha de Juros Hipotecários Dedutíveis

Caso o Drake não possua uma caixa de seleção direta para "pontos de refinanciamento", isso será tratado no Passo 3 abaixo.

---

### PASSO 3 — PREENCHER A PLANILHA DE JUROS HIPOTECÁRIOS DEDUTÍVEIS NO DRAKE
**Caminho no Drake:** A partir de qualquer tela do Form 1098 → Clicar em "Loan Limit Worksheet" (canto superior direito) — OU —
**Data Entry → Deductible Mortgage Interest (a tela que estava em branco)**

Esta é a tela que foi deixada completamente em branco na declaração original. **Todos os campos devem ser preenchidos.**

**Inserir os seguintes valores:**

| Campo no Drake | Valor a Inserir | Explicação |
|-------------|---------------|-------------|
| Line 1 — Average balance, grandfathered debt (pre-10/14/1987) | **0** | Sem dívida anterior a 1987 |
| Line 2 — Average balance, pre-12/16/2017 acquisition debt | **0** | Sem dívida anterior ao TCJA |
| Line 7 — Average balance, post-12/15/2017 acquisition debt | **939.744** | AmWest $519.744 + Radius $420.000 |
| Line 12 — Total average balances (Drake may auto-fill) | **939.744** | Igual à Line 7 |
| Line 13 — Total interest paid (NO points) | **97.004** | AmWest $95.134 + Radius $1.870 |
| Line 17 — Points reported on 1098 | **18.900** | Radius Box 6 |
| Points NOT reported on 1098 | **0** | |

**Após inserir Line 7 = 939.744:**
O Drake calculará automaticamente:
- Line 8: $750.000
- Line 9: $750.000
- Line 10: $939.744
- Line 11: **$750.000** ← Limite de empréstimo qualificado
- Line 14: $750.000 ÷ $939.744 = **0,798**
- Line 15: $97.004 × 0,798 = **$77.409** ← Juros hipotecários dedutíveis

**Verificar se o Drake transporta $77.409 para o Schedule A.**

---

### PASSO 4 — TRATAR OS PONTOS HIPOTECÁRIOS (POINTS) DO REFINANCIAMENTO RADIUS ($18.900)

Os $18.900 em pontos hipotecários (points) do Radius devem ser amortizados ao longo do prazo do empréstimo — NÃO deduzidos integralmente em 2024.

**Caminho no Drake:** A amortização dos pontos hipotecários (points) é tipicamente configurada por meio do lançamento do Form 1098 ou por meio de uma tela específica de amortização de pontos.

**Você precisa da Nota Hipotecária (Mortgage Note) do Radius para confirmar o prazo do empréstimo.** Considerando 30 anos (360 meses):

| Cálculo | Valor |
|-------------|--------|
| Total de pontos hipotecários (points) | $18.900 |
| Prazo do empréstimo | 360 meses (30 anos) — CONFIRMAR NA MORTGAGE NOTE |
| Amortização mensal | $18.900 ÷ 360 = $52,50 |
| Data de originação do empréstimo | 11/13/2024 |
| Meses em 2024 (11/13 a 12/31) | 1,57 meses |
| Pontos brutos dedutíveis em 2024 | $52,50 × 1,57 = $82,43 |
| Após aplicação do índice de limite de empréstimo (× 0,798) | $82,43 × 0,798 = **$65,78 → $66** |
| Pontos dedutíveis em 2024 | **$66** |
| Dedução anual futura (anos 2025–2054) | $52,50 × 12 × 0,798 = **$502/ano** |
| Ano final (2054, parcial) | Saldo remanescente |

**No Drake:**
- Procurar uma tela "Points Amortization" ou "Unamortized Points"
- Inserir: data de originação do empréstimo 11/13/2024, total de pontos $18.900, prazo do empréstimo (360 meses)
- Confirmar se o Drake limita a dedução de 2024 ao valor proporcional (aproximadamente $66)
- O Drake transportará automaticamente os pontos não amortizados remanescentes para os anos futuros

**Caso o Drake aplique automaticamente o índice de limite de empréstimo aos pontos por meio da Planilha de Juros Hipotecários Dedutíveis, verificar o resultado. Caso contrário, inserir manualmente os pontos dedutíveis de 2024 como aproximadamente $66 na linha 8c do Schedule A (Points not reported on Form 1098 — a parcela amortizada).**

---

### PASSO 5 — VERIFICAR O SCHEDULE A CORRIGIDO

Após concluir os Passos 2 a 4, o Schedule A do Drake deverá apresentar:

| Linha | Descrição | Original | Corrigido |
|------|-------------|---------|-----------|
| 5a | State/local income taxes | $5.424 | $5.424 (sem alteração) |
| 5b | Real estate taxes | $2.651 | $2.651 (sem alteração) |
| 5e | Taxes cap | $8.075 | $8.075 (sem alteração) |
| 7 | Total taxes | $8.075 | $8.075 (sem alteração) |
| 8a | Mortgage interest (Form 14900 limited) | $114.034 | **$77.409** |
| 8c | Points (2024 amortized, if on this line) | $0 | **$66** |
| 8e | Total interest | $114.034 | **$77.475** |
| **17** | **Total itemized deductions** | **$122.109** | **$85.550** |

---

### PASSO 6 — VERIFICAR O RECÁLCULO AUTOMÁTICO DO Form 8995 (QBID)

O Drake recalculará automaticamente o QBID quando o Schedule A for alterado. Verificar:

| Linha do Form 8995 | Original | Corrigido |
|----------------|---------|-----------|
| Valores de QBI (Lines 1i–1iii) | $75.630 + $42.054 + $30.405 | Sem alteração |
| Line 4 — Total QBI | $148.089 | Sem alteração |
| Line 5 — 20% of QBI | $29.618 | Sem alteração |
| Line 11 — Pre-QBID taxable income | $25.980 | **$62.539** |
| Line 14 — Income limitation (×20%) | $5.196 | **$12.508** |
| **Line 15 — QBID** | **$5.196** | **$12.508** |

---

### PASSO 7 — VERIFICAR O Form 1040 CORRIGIDO

| Linha | Descrição | Original | Corrigido |
|------|-------------|---------|-----------|
| 11 | Adjusted gross income | $148.089 | $148.089 (sem alteração) |
| 12 | Schedule A deductions | $122.109 | **$85.550** |
| 13 | QBID | $5.196 | **$12.508** |
| 14 | Total deductions (12+13) | $127.305 | **$98.058** |
| **15** | **Taxable income** | **$20.784** | **$50.031** |
| 16 | Income tax | $2.261 | **$6.060** |
| 23 | SE tax | $11.498 | $11.498 (sem alteração) |
| **24** | **Total tax** | **$13.759** | **$17.558** |
| 25d | Tax withheld | $0 | $0 (sem alteração) |
| **37** | **Amount owed** | **$14.379** | **$17.558** |

**Cálculo do imposto de renda corrigido sobre $50.031 (contribuinte solteiro, faixas de 2024):**
- Faixa de 10% ($0–$11.600): $11.600 × 10% = $1.160
- Faixa de 12% ($11.601–$47.150): $35.550 × 12% = $4.266
- Faixa de 22% ($47.151–$50.031): $2.881 × 22% = $634
- **Total do imposto de renda = $6.060**

**SE tax: $11.498 (inalterado)**
**Total do imposto corrigido: $17.558**

---

### PASSO 8 — PREPARAR O Form 1040-X NO DRAKE

**Caminho no Drake:** Tools → Amended Return → Form 1040-X

O Drake preencherá três colunas automaticamente:
- **Coluna A (Original):** Valores originais conforme declarados
- **Coluna B (Net Change):** A diferença
- **Coluna C (Corrected):** Novos valores

**Principais linhas do Form 1040-X a verificar:**

| Linha do Form 1040-X | Descrição | Col A (Original) | Col B (Alteração) | Col C (Corrigido) |
|-------------|-------------|-----------------|----------------|-------------------|
| 1 | Adjusted gross income | $148.089 | $0 | $148.089 |
| 4 | Itemized deductions | $122.109 | ($36.559) | $85.550 |
| 5 | QBI deduction | $5.196 | $7.312 | $12.508 |
| 7 | Taxable income | $20.784 | $29.247 | $50.031 |
| 10 | Tax | $2.261 | $3.799 | $6.060 |
| 16 | Total tax | $13.759 | $3.799 | $17.558 |
| 20 | Amount previously paid | $0 | — | — |
| 22 | Amount you owe | $13.759 | $3.799 | **$17.558** |

**Part III — Explanation of Changes (obrigatório no Form 1040-X):**

Inserir a seguinte explicação no campo de explicação do Form 1040-X no Drake:

> "The taxpayer's home mortgage interest deduction on Schedule A is being corrected pursuant to IRC §163(h)(3)(B). Both mortgages (AmWest Funding Corp, originated 10/20/2023; Radius Financial Group, originated 11/13/2024) were incurred after December 15, 2017. The average combined mortgage balance for 2024 was $939,744, exceeding the $750,000 qualified loan limit. Per the completed Form 14900 (attached), the correct deductible interest is $77,409 (vs. $114,034 originally claimed), a ratio of 79.8%. Additionally, the $18,900 in points paid on the Radius refinancing loan must be amortized over the loan term under IRC §461(g)(2); only approximately $66 is deductible in 2024. The corrected Schedule A deduction is $85,550. The QBID under IRC §199A increases from $5,196 to $12,508 as a result of the higher taxable income. The additional tax owed is $3,799. Form 14900 is enclosed."

---

### PASSO 9 — ANEXAR O Form 14900 AO Form 1040-X

No Drake, é possível anexar o Form 14900 como um anexo em PDF à declaração.
- O Form 14900 já está preenchido no Pacote de Defesa da Auditoria (Seção 3).
- Imprimi-lo ou gerá-lo e anexá-lo tanto ao envio pelo correio do Form 1040-X quanto à resposta à Letter 566-T do IRS.

---

### PASSO 10 — APRESENTAÇÃO DO Form 1040-X

**Como apresentar:**
- O Form 1040-X **não pode ser transmitido eletronicamente** nesta situação (exame por correspondência ativo).
- Imprimir o Form 1040-X assinado.
- Enviá-lo JUNTO com o pacote de resposta à auditoria para:

**IRS Correspondence Examination (resposta à auditoria):**
Internal Revenue Service
P.O. Box 309011, AMC 8236
Memphis TN 38130-0911
*(Utilizar o Form 14817 Reply Cover Sheet no topo)*

- OU incluí-lo como um Anexo no pacote de resposta à auditoria com uma nota solicitando ao examinador que o processe.
- Na carta de apresentação, declarar: "We are enclosing a corrected Form 1040-X conceding the overstatement. Please advise if you will process this adjustment through the examination or if a separate submission is required."

---

---

## PARTE 3 — RESUMO COMPLETO DE TODAS AS ALTERAÇÕES

### Alterações a Realizar no Drake:

| # | Local no Drake | O Que Alterar |
|---|----------------|----------------|
| 1 | Form 1098 — Radius (Record 2) | Excluir o "0" em "Deductible amount, if different" → deixar EM BRANCO |
| 2 | Form 1098 — Radius (Record 2) | Marcar o empréstimo como REFINANCIAMENTO (não compra) para que os pontos hipotecários (points) sejam amortizados |
| 3 | Deductible Mortgage Interest Worksheet | Inserir Line 7: 939.744 |
| 4 | Deductible Mortgage Interest Worksheet | Inserir Line 13: 97.004 |
| 5 | Deductible Mortgage Interest Worksheet | Inserir Line 17 (Points on 1098): 18.900 |
| 6 | Points Amortization | Configurar $18.900 ao longo do prazo do empréstimo; dedutível em 2024 = ~$66 |
| 7 | Form 1040-X | Preencher com os valores corrigidos + explicação |
| 8 | Form 1040-X | Anexar o Form 14900 como documento de suporte |

### O Que o Drake Calculará Automaticamente Após as Alterações:

| Formulário | Linha | Passará a Ser |
|------|------|----------------|
| Form 14900 | Line 11 (Qualified Loan Limit) | $750.000 |
| Form 14900 | Line 14 (Ratio) | 0,798 |
| Form 14900 | Line 15 (Deductible interest) | $77.409 |
| Schedule A | Line 8a | $77.409 |
| Schedule A | Line 8c | $66 (pontos amortizados) |
| Schedule A | Line 17 (Total) | $85.550 |
| Form 8995 | Line 15 (QBID) | $12.508 |
| Form 1040 | Line 15 (Taxable income) | $50.031 |
| Form 1040 | Line 16 (Tax) | $6.060 |
| Form 1040 | Line 24 (Total tax) | $17.558 |

### Impacto Financeiro Líquido sobre Eliana:

| Item | Valor |
|------|--------|
| Imposto total original | $13.759 |
| Imposto total corrigido | $17.558 |
| **Imposto adicional devido** | **$3.799** |
| Juros estimados sobre $3.799 (de 15/04/2025 até hoje) | ~$380–450 |
| Penalidade por pagamento insuficiente | Será calculada pelo IRS |

---

## OBSERVAÇÕES IMPORTANTES PARA ISABEL

1. **Nota Hipotecária (Mortgage Note) do Radius:** Você precisa da nota para confirmar o prazo do empréstimo (30 anos, 15 anos ou outro). Isso afeta o valor da amortização dos pontos hipotecários (points). A diferença é pequena ($66 versus $132 em 2024), mas deve ser exata.

2. **Transporte de pontos para anos futuros:** Após a correção de 2024, o Drake criará um transporte de "pontos a serem amortizados em anos futuros". Lembre-se de incluir isso nas declarações de Eliana de 2025, 2026... até que os pontos sejam integralmente amortizados.

3. **Assinatura de Eliana:** O Form 1040-X requer a assinatura de Eliana antes de poder ser apresentado.

4. **Pagamento:** Caso Eliana ainda não tenha pago os $14.379 originais, ela deve pagar pelo menos esse valor agora para interromper o acúmulo de juros, e em seguida pagar os $3.799 adicionais quando o Form 1040-X for apresentado.

5. **Prazo:** A resposta à Letter 566-T do IRS vence em **17 de junho de 2026** (30 dias a partir de 18 de maio de 2026). Não perder este prazo.

---

*Arquivo de Correção no Drake preparado por: Advance Tax Services Accountants Inc | 7 de junho de 2026*
*Para uso de: Isabel Raimundo, EA — Advance Tax Services Accountants Inc*
*PTIN: P02482553 | Tel: 781-759-2202*
