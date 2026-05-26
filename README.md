# Desafio Criativo: Extraindo Insights do Feedback de Clientes Bancários

> **Autor:** Luana Gomes
> 
> **Tema:** Análise de feedbacks de clientes bancários com apoio de IA  

---

## Passo 1 — Intenção

Quero que a IA analise uma base de feedbacks de clientes bancários (comentários abertos, avaliações de NPS, reviews do app e mensagens de atendimento) para identificar temas recorrentes, sentimentos predominantes, dores críticas, elogios e oportunidades de melhoria.

O resultado será usado pela equipe de Customer Experience (CX) e pelo time de Produto Digital do banco para apoiar decisões de priorização de melhorias no aplicativo, nos canais de atendimento e nos produtos financeiros oferecidos.

A entrega deve conter um resumo executivo, uma tabela com temas classificados (tema, sentimento, urgência, evidência e ação sugerida) e uma lista final com as 3 prioridades estratégicas mais importantes.

O resultado será considerado bom se for claro, organizado, baseado exclusivamente nos dados fornecidos, livre de exposição de dados sensíveis e útil para priorizar ações de curto e médio prazo.

---

## Passo 2 — Contexto e Restrições

**Contexto:** Estou trabalhando com feedbacks de clientes bancários relacionados ao **aplicativo mobile, Pix, cartão de crédito, abertura de conta e atendimento por chat e telefone**.

**Dados disponíveis:** A base contém os seguintes campos:
- `data_do_comentario` (data em que o feedback foi registrado)
- `canal` (app, chat, telefone, e-mail, redes sociais)
- `produto_citado` (Pix, cartão, conta, investimentos, empréstimo etc.)
- `texto_do_feedback` (comentário aberto do cliente)
- `nota_satisfacao` (escala de 1 a 5)
- `segmento_cliente` (PF varejo, PF alta renda, PJ)

**Critérios de análise:** A IA deve classificar os feedbacks por:
- **Tema** (ex.: lentidão do app, falha no Pix, atendimento demorado)
- **Sentimento** (positivo, negativo, neutro)
- **Urgência** (alta, média, baixa)
- **Canal e produto impactados**
- **Possível impacto na experiência e no risco de churn**

**Cuidados e restrições:**
- Use **apenas os dados fornecidos**.
- **Não invente** números, causas, percentuais ou conclusões sem evidência.
- **Não exponha dados pessoais ou sensíveis** (nome, CPF, conta, agência, e-mail, telefone, endereço). Anonimize ao citar exemplos.
- Se houver **informação insuficiente**, indique claramente a limitação.
- Respeite a **LGPD** e as boas práticas de privacidade do setor financeiro.
- Use **linguagem simples, executiva e voltada à tomada de decisão**.

---

## Passo 3 — Prompt Final Consolidado

```markdown
Atue como analista sênior de dados e Customer Experience (CX) especializado no setor bancário, 
com experiência em análise qualitativa de feedbacks, identificação de padrões comportamentais 
e geração de insights estratégicos para produtos e canais digitais.

Sua tarefa é analisar feedbacks de clientes bancários sobre aplicativo mobile, Pix, cartão de crédito, 
abertura de conta e atendimento (chat e telefone), para identificar temas recorrentes, 
sentimentos predominantes, dores críticas, elogios e oportunidades de melhoria.

Contexto:
A análise será usada pela equipe de Customer Experience e pelo time de Produto Digital de um banco, 
com o objetivo de priorizar melhorias nos canais digitais, reduzir atritos no atendimento e 
fortalecer a retenção de clientes. O foco é transformar comentários soltos em insights claros, 
acionáveis e baseados em evidências.

Dados disponíveis:
Serão fornecidos registros com os seguintes campos:
- data_do_comentario
- canal (app, chat, telefone, e-mail, redes sociais)
- produto_citado (Pix, cartão, conta, investimentos, empréstimo, etc.)
- texto_do_feedback (comentário aberto)
- nota_satisfacao (1 a 5)
- segmento_cliente (PF varejo, PF alta renda, PJ)

Instruções de análise:
1. Classifique os feedbacks por tema, sentimento (positivo, negativo, neutro), 
   urgência (alta, média, baixa), canal e produto citado.
2. Identifique os principais padrões, dores recorrentes, elogios e oportunidades.
3. Aponte evidências nos dados fornecidos, usando trechos curtos e anonimizados de comentários.
4. Sugira ações práticas para a equipe de CX e para o time de Produto Digital.
5. Relacione cada insight ao possível impacto na experiência do cliente e no risco de churn.

Formato da resposta:
- **Resumo executivo:** até 5 linhas com os principais achados.
- **Tabela de análise:** colunas → Tema | Sentimento | Urgência | Canal/Produto | Evidência (trecho anonimizado) | Ação Sugerida.
- **Top 3 prioridades estratégicas:** lista final com as ações mais importantes, 
  justificadas por evidência e impacto esperado.
- **Alertas de criticidade:** sinalize qualquer feedback que indique risco 
  reputacional, legal, regulatório ou de segurança.

Restrições:
- Use apenas os dados fornecidos.
- Não invente números, causas, percentuais ou conclusões.
- Não exponha dados pessoais ou sensíveis (nome, CPF, conta, agência, telefone, e-mail, endereço). 
  Anonimize qualquer trecho citado.
- Informe limitações quando os dados forem insuficientes para conclusões robustas.
- Respeite a LGPD e as boas práticas de privacidade do setor financeiro.
- Use linguagem simples, direta, executiva e voltada à tomada de decisão.
```

---

## Checklist de Qualidade do Prompt

- [x] Papel da IA definido com clareza  
- [x] Objetivo da análise explícito  
- [x] Público e finalidade do resultado descritos  
- [x] Dados disponíveis detalhados (campos da base)  
- [x] Critérios de classificação definidos  
- [x] Formato de resposta estruturado  
- [x] Cuidados com dados sensíveis e LGPD incluídos  
- [x] Restrições contra alucinação da IA aplicadas  
- [x] Linguagem adequada ao público executivo  

---

## Como usar este prompt

1. Copie o bloco do **Passo 3 – Prompt Final Consolidado**.  
2. Cole no ChatGPT, Claude, Gemini ou qualquer outra IA generativa.  
3. Anexe ou cole a base de feedbacks que deseja analisar.  
4. Receba insights estruturados e prontos para apresentar à liderança.  

---

*Desafio entregue como parte da formação em Engenharia de Prompts – DIO.*
