# 🚀 Deploy — Proposta Bia (Elienai)

Site **estático** (1 arquivo `index.html` + `assets/`). Sem build, sem framework.
Tudo que precisa já está nesta pasta.

---

## ✅ Antes de subir (checklist)
- [ ] **WhatsApp:** no `index.html`, trocar `WA_PLACEHOLDER` pelo número real
      (formato internacional sem `+`, ex.: `351912345678`). Está no topo do `<script>`.
- [ ] Conferir os domínios na proposta (`advena.com` / `beatrizconrado.com`).
- [ ] (Opcional) `assets/computador-3d.png` está **sem uso** — pode apagar pra deixar leve.

---

## Opção A — Vercel CLI (mais rápido)
```bash
npm i -g vercel          # se ainda não tiver
cd "caminho/para/Apresentacao_Beatriz"
vercel                   # 1ª vez: cria o PROJETO NOVO (preview)
vercel --prod            # publica em produção
```
Na 1ª vez o CLI pergunta:
- *Set up and deploy?* → **Y**
- *Which scope?* → sua conta/agência
- *Link to existing project?* → **N** (projeto novo)
- *Project name?* → ex.: `proposta-bia`
- *In which directory is your code?* → **./** (esta pasta)
- Framework → **Other** (estático)

## Opção B — Painel Vercel (sem CLI)
1. https://vercel.com/new
2. Arraste a pasta `Apresentacao_Beatriz` (ou conecte um repositório Git).
3. Framework Preset: **Other**. Root: esta pasta. **Deploy**.

---

## 🌐 Domínio — elienai.designer (conta: designelienai-code)
Como `elienai.designer` já está na sua conta Vercel, o mais limpo é um **subdomínio**
por cliente — ex.: **`bia.elienai.designer`**.

Depois do deploy:
**Project (proposta-bia) → Settings → Domains → Add → `bia.elienai.designer`**
→ como o apex já está na Vercel, o DNS é configurado **automaticamente** (1 clique, sem colar registro).

> Sugestão de URL pra mandar pra ela: `https://bia.elienai.designer`

---

## Atualizar depois
Edita o `index.html` → `vercel --prod` de novo (ou push no Git, se conectado).
