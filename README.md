# BodyMetrics · PWA

Painel de composição corporal e atividade física (IMC, FFMI, FMI, treinos antes/depois, importação CSV/GPX, Fitbit OAuth, escalas científicas).

## Publicar no GitHub Pages

### 1. Criar repositório

1. Em [github.com/new](https://github.com/new) crie um repositório (ex.: `bodymetrics`).
2. Pode ser **público** (Pages gratuito) ou privado (Pages disponível em contas com plano que o permita).

### 2. Enviar os ficheiros

**Opção A — Interface web**

1. No repositório → **Add file** → **Upload files**.
2. Arraste **todos** os ficheiros desta pasta:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon.svg`
   - `icon-192.png`
   - `icon-512.png`
   - `README.md` (opcional)
3. **Commit changes**.

**Opção B — Git na linha de comandos**

```bash
cd bodymetrics-pwa
git init
git add .
git commit -m "BodyMetrics PWA"
git branch -M main
git remote add origin https://github.com/SEU_UTILIZADOR/bodymetrics.git
git push -u origin main
```

### 3. Ativar GitHub Pages

1. Repositório → **Settings** → **Pages**.
2. **Source**: Deploy from a branch.
3. **Branch**: `main` · pasta `/ (root)`.
4. **Save**.

Aguarde 1–2 minutos. O URL será:

```
https://SEU_UTILIZADOR.github.io/bodymetrics/
```

(se o repositório se chamar `bodymetrics`)

### 4. Instalar no Android

1. Abra o URL no **Chrome**.
2. Menu (⋮) → **Adicionar ao ecrã inicial** / **Instalar aplicação**.
3. O ícone abre a app em modo standalone (como app nativa).

### Fitbit (opcional)

1. Em [dev.fitbit.com/apps](https://dev.fitbit.com/apps) registe uma app tipo **Client**.
2. **Callback URL**: o mesmo URL do Pages, com barra final se necessário  
   `https://SEU_UTILIZADOR.github.io/bodymetrics/`
3. Na app BodyMetrics → **Ligações** → cole o Client ID → Ligar.

### Amazfit / Zepp

Exportar dados na app Zepp → importar CSV/GPX em **Adicionar**.

## Funcionalidades

- Pesagens e composição (IMC, FFMI, FMI, BMR, TDEE)
- Escalas de cores com referências (OMS, ACE, Kouri, ESPEN)
- Atividade física e análise antes/depois do treino + água
- Importação CSV (Runstar, Fitbit, Zepp) e GPX
- Relatórios de IA e exportação PDF
- PWA instalável offline (service worker)

Dados guardados apenas no **localStorage** do browser (não há servidor).
