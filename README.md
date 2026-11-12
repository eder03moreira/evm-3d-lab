# EVM 3D Lab — Layout Premium

Site para catálogo e solicitação de orçamentos por WhatsApp. **Sem preços, sem checkout, sem banco de dados e sem painel administrativo online** nesta fase.

## Marca

Usa a **logomarca oficial enviada pelo proprietário**, salva em `assets/logo-oficial.png`. O arquivo de origem não foi redesenhado: apenas retiramos o excesso de margem preta para uso no cabeçalho. Os elementos do catálogo e banner são **imagens de demonstração extraídas da referência visual enviada pelo usuário**; substitua por fotografias próprias antes de divulgar os produtos como disponíveis.

## Como atualizar seu site no GitHub Pages

1. Extraia o ZIP desta entrega.
2. Abra o repositório `eder03moreira/evm-3d-lab` no GitHub.
3. Envie os arquivos `index.html`, `style.css`, `app.js`, `products.json`, `site-config.json` e a **pasta inteira `assets/`**. Preserve os caminhos e nomes dos arquivos. Substitua os arquivos antigos.
4. Se o repositório já estiver configurado em **Settings > Pages > Deploy from a branch > main > /(root)**, o site se atualizará após o próximo deploy.
5. Abra `https://eder03moreira.github.io/evm-3d-lab/` para conferir. Dê um recarregamento forçado (Ctrl+F5) se estiver vendo a versão antiga.

**Atenção:** Se você enviou um arquivo chamado `CNAME` contendo `eder03moreira.github.io/evm-3d-lab/`, exclua-o. Esse caminho não é um domínio personalizado.

## Como editar os produtos

O catálogo é carregado pelo arquivo `products.json`. Cada produto tem: `id`, `name`, `cat`, `desc`, `image`, `icon`, `active` e `sample`.

- Para ocultar um produto, defina `"active": false`.
- Para mostrar imagens próprias, faça upload de fotos na pasta `images/`, depois escreva `"image":"images/minha-foto.jpg"` no JSON.
- Remova ou altere a marca `sample` depois de cadastrar seus próprios produtos. Um `sample:false` significa que a foto já é sua e foi confirmada para aquele produto.
- **Nunca coloque senhas ou dados privados nesses arquivos**, porque o GitHub Pages é um site público.

## Como editar os textos

Edite `site-config.json` para a frase principal, texto do banner, sobre e seção de personalizados. Os títulos fixos do layout continuam em `index.html`.

## Futuro e-commerce

O catálogo foi separado de seu visual para facilitar migração futura para banco de dados, painel com autenticação, estoque, pedidos e pagamento. **Não há backend implementado.** O site utiliza somente HTML, CSS e JS e pode ser hospedado gratuitamente em GitHub Pages nos limites da plataforma.
