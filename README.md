# Greencycle — Mapa de Reciclagem (SP)

Mapa interativo de pontos de reciclagem com filtros por material, lista dos locais e rota no Google Maps.  
Inclui seções de **Recursos**, **Planos**, **Portal B2B**, **Contato** e bloco **LGPD**.

> **Stack**: HTML estático + Tailwind (CDN) + Leaflet (CDN).  
> **Sem build** / **Sem frameworks** — funciona apenas com `index.html`.

---

## ✨ Funcionalidades
- 🗺️ **Mapa interativo** (Leaflet) centrado em São Paulo
- 🔎 **Busca** por nome e **filtro AND** por materiais (ex.: PET + Plástico)
- 📍 **Rota** no Google Maps a partir de cada ponto
- 📦 Mock com **10 pontos** (nome, lat/lng, materiais, rating, horário)
- 📱 Layout responsivo
- 🔒 Bloco de **LGPD** (opt-in simples)
- 🧭 Seções de marketing: Recursos, Planos, B2B e Contato

---

## 🚀 Publicação

### GitHub Pages
1. Garanta que o arquivo se chama **`index.html`** (na **raiz** do repositório).
2. Vá em **Settings → Pages**  
   - **Source**: *Deploy from a branch*  
   - **Branch**: `main` • **Folder**: `/ (root)` → **Save**
3. Abra a URL exibida (ex.: `https://SEU_USUARIO.github.io/Greencycle`).

> **Dica**: se a página não subir, confirme o nome **exato** `index.html`  
> (não `index.html.html`) e faça um *hard refresh* (Ctrl/Cmd + Shift + R).

### Netlify (Drop)
1. Coloque `index.html` dentro de uma pasta (ex.: `Greencycle/`)  
2. Compacte a pasta em `Greencycle.zip`
3. Acesse **app.netlify.com → Add new site → Deploy manually** e arraste o `.zip`.

---

## 🔧 Rodar localmente
- Clique duas vezes no `index.html` (abre direto no navegador), **ou**
- Sirva via HTTP para evitar bloqueios de geolocalização:
  ```bash
  # Python 3
  python -m http.server 3000
  # Abra http://localhost:3000
