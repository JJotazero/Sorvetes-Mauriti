# Sorvetes Mauriti

Site institucional estático da Sorvetes Mauriti Ltda (Mauriti, CE).

## Estrutura

```
index.html        página principal
404.html          página de erro
css/style.css     estilos
assets/img/       imagens publicadas
robots.txt
.nojekyll         faz o GitHub Pages servir os arquivos como estão
_arquivo/         arquivos guardados, fora do deploy (ignorado pelo git)
```

## Rodar localmente

```
python -m http.server 8000
```

Acesse http://localhost:8000

## Publicar no GitHub Pages

1. Crie um repositório vazio no GitHub (ex.: `sorvetes-mauriti`).
2. Na pasta do projeto:
   ```
   git remote add origin https://github.com/SEU_USUARIO/sorvetes-mauriti.git
   git push -u origin main
   ```
3. No GitHub: **Settings → Pages → Source: Deploy from a branch → `main` / `(root)`** → Save.
4. Em ~1 minuto o site fica em `https://SEU_USUARIO.github.io/sorvetes-mauriti/`.

Para atualizar: `git add .`, `git commit -m "mensagem"`, `git push`.

> Obs.: a página 404 usa caminhos absolutos (`/css/...`), que funcionam em domínio próprio
> ou num repositório `SEU_USUARIO.github.io`. Num repositório de projeto, troque `/` por `/sorvetes-mauriti/` no `404.html`.
