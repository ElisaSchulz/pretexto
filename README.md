# Pretexto · Clube do Livro

Site estático do Pretexto, clube do livro em Stillwater, OK.

## Arquivos
- `index.html`: a página inteira (HTML e CSS, sem build).
- `img/`: logo, ilustrações e favicon em WebP/PNG.
- `.nojekyll`: faz o GitHub Pages servir os arquivos como estão.

## Publicar no GitHub Pages
1. Criar o repositório `pretexto` na conta `elisaschulz` e enviar todos os arquivos desta pasta para a raiz da branch `main`.
2. Em Settings › Pages: Source = "Deploy from a branch", Branch = `main`, pasta `/ (root)`.
3. O site fica em https://elisaschulz.github.io/pretexto/

Com o GitHub CLI:
```
gh repo create pretexto --public --source=. --push
gh api -X POST repos/elisaschulz/pretexto/pages -f "source[branch]=main" -f "source[path]=/"
```
