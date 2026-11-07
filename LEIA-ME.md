# Site da KOI Island (GitHub Pages)

Arquivos desta pasta:
- `index.html` — a página.
- `latest.json` — versão atual, arquivos para baixar e novidades. A página lê este arquivo (e, no futuro, a ilha também, para avisar que tem atualização).
- `assets/` — imagens, ícone e fonte.
- `.nojekyll` — avisa o GitHub para publicar os arquivos como estão.

## A cada versão nova
1. Crie a release `vX.Y.Z` no GitHub e anexe `KOI-Island-Setup-X.Y.Z.exe` e `KOI-Island-X.Y.Z-portable.exe`.
2. Edite o `latest.json`: `version`, `date`, `tagline`, os nomes, tamanhos e `sha256` dos dois arquivos, e coloque um item novo no começo de `changelog`.
3. Pronto: a página passa a mostrar a versão nova e os botões já baixam os arquivos novos.

Os links de download são montados assim: `https://github.com/USUARIO/REPOSITORIO/releases/download/TAG/ARQUIVO (a tag vem do campo "tag" do latest.json, ex.: v1.3.0-beta)`.
No GitHub Pages o usuário e o repositório são lidos do próprio endereço do site; fora dele, preencha `"repo": "usuario/repositorio"` no `latest.json`.
