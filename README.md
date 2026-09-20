# App2fit · PWA

Aplicação web progressiva de composição corporal, treinos e evolução (instalável no Android).

## Publicar no GitHub Pages

1. Em [github.com/new](https://github.com/new) crie um repositório (ex.: `app2fit`).
2. Carregue os ficheiros desta pasta (`index.html`, `manifest.json`, `sw.js`, ícones, etc.).
3. **Settings → Pages → Source**: branch `main`, pasta `/ (root)`.
4. Abra: `https://SEU_UTILIZADOR.github.io/app2fit/`

## Fitbit

1. Registe uma app em [dev.fitbit.com/apps](https://dev.fitbit.com/apps).
2. Callback URL = URL do GitHub Pages.
3. Na app App2fit → **Ligações** → Client ID → Ligar.

## Dados

Os dados ficam no `localStorage` do browser. Use **Ligações → Backup** para exportar/importar JSON.

## Ícones (`icons/`)

| Ficheiro | Uso |
|----------|-----|
| `icons/mark.svg` | Favicon vectorial |
| `icons/mark-192.png` / `mark-512.png` | Ícone PWA / Apple Touch |
| `icons/mark.png` | Símbolo em alta resolução |
| `icons/full.png` | Logo completo (símbolo + texto) |
| `icons/wordmark.png` | Apenas texto «App2Fit» |

Na raiz mantêm-se `icon-192.png`, `icon-512.png` e `icon.svg` por compatibilidade com o service worker e installs antigos.
