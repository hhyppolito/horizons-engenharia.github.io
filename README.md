# HEST Engenharia — site institucional

Site de apresentação de serviços de engenharia e BIM. O repositório mantém o nome `horizons-engenharia.github.io`, mas o título atual do HTML é **HEST Engenharia**.

## Conteúdo e funcionamento

A página inclui serviços, método de trabalho, projetos em destaque, contactos e um visualizador IFC. A implementação está em HTML, CSS e JavaScript, com recursos externos para o visualizador, fontes e análise de utilização.

## Estrutura

- [index.html](index.html): página principal, estilos e scripts.
- [privacidade.html](privacidade.html): página de privacidade.
- [CNAME](CNAME): configuração de domínio para o alojamento.
- Imagens PNG na raiz: logótipo e fundos.

Não há `package.json` nem processo de compilação definido na árvore atual.

## Pré-visualizar localmente

Com Python 3 instalado, executar na raiz:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Abrir [localhost:8000](http://localhost:8000). Um servidor HTTP é preferível a abrir o ficheiro diretamente, devido aos scripts e carregamento de recursos.

O visualizador e alguns recursos dependem de acesso à Internet. O código inclui um pedido a um IFC de exemplo alojado externamente; a sua disponibilidade não é controlada por este repositório.

## Atualizar o site

1. Alterar textos, serviços e contactos em `index.html`.
2. Substituir imagens preservando os caminhos ou atualizar as referências.
3. Conferir a página de privacidade ao alterar formulários, integrações ou análise de utilização.
4. Testar navegação, contactos, visualizador e apresentação em diferentes larguras.
5. Rever a versão final antes de publicar.

A página inclui Microsoft Clarity e Google Fonts. Considerar estas integrações ao verificar o comportamento e a informação apresentada aos visitantes.

## Publicação

O projeto é compatível com alojamento estático. A existência de `CNAME` e o nome do repositório não confirmam, por si só, que o domínio ou o GitHub Pages estejam ativos. Confirmar a branch/pasta de origem e as definições de domínio no alojamento antes de alterar a publicação.

## Verificação

Documentação baseada no HTML e na árvore inspecionados em 11/11/2026. Não foram executados testes de navegador nem verificada a implantação. Não há suite de testes ou build automatizado identificado no repositório.
