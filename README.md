# Qraft — Gerador de QR Code

Gerador de QR Code executado diretamente no navegador. Permite criar códigos a partir de links ou textos, personalizar sua aparência, adicionar um logotipo e exportar o resultado em PNG.

O projeto é composto por um único arquivo HTML e não requer instalação, servidor, cadastro ou conexão com um serviço externo para gerar os códigos.

## Funcionalidades

- Geração de QR Code a partir de link ou texto;
- Atualização da pré-visualização em tempo real;
- Inclusão de logotipo no centro do código;
- Ajuste do tamanho e do recorte do logotipo;
- Personalização das cores do código e do fundo;
- Diferentes estilos para módulos e marcadores;
- Configuração de margem e resolução;
- Avisos automáticos sobre contraste e legibilidade;
- Exportação em PNG;
- Temas de cor para a interface;
- Layout responsivo para computadores e dispositivos móveis.

## Como usar

1. Baixe ou clone este repositório.
2. Abra o arquivo `index.html` em um navegador moderno.
3. Informe um link ou selecione a opção de texto.
4. Personalize as cores, os módulos e os marcadores, se necessário.
5. Adicione um logotipo opcional.
6. Teste o código com a câmera de um celular.
7. Clique em **Baixar QR Code** para salvar o arquivo PNG.

Não é necessário executar `npm install`, compilar o projeto ou configurar variáveis de ambiente.

## Execução com servidor local

Embora o arquivo possa ser aberto diretamente, também é possível executá-lo por meio de um servidor local.

Com Python:

```bash
python -m http.server 8000
```

Depois, acesse:

```text
http://localhost:8000
```

## Estrutura do projeto

```text
.
├── index.html   # Interface, estilos, biblioteca de QR Code e lógica da aplicação
└── README.md    # Documentação do projeto
```

Toda a aplicação está contida no arquivo `index.html`, incluindo:

- HTML da interface;
- Estilos CSS;
- Biblioteca de geração do QR Code;
- Lógica de personalização e exportação.

## Privacidade

Os dados informados e as imagens selecionadas são processados localmente no navegador. O projeto não envia nem armazena o conteúdo usado para gerar o QR Code.

## Compatibilidade

Recomenda-se utilizar uma versão atualizada de um dos seguintes navegadores:

- Google Chrome;
- Microsoft Edge;
- Mozilla Firefox;
- Safari.

## Boas práticas

- Mantenha contraste suficiente entre o código e o fundo;
- Prefira módulos escuros sobre fundo claro;
- Evite ocupar uma área central muito grande com o logotipo;
- Teste o QR Code em mais de um aparelho antes de imprimir ou publicar;
- Para impressão, utilize uma resolução maior e preserve a margem ao redor do código.

## Dependência incorporada

A matriz do QR Code é gerada com a biblioteca `qrcode-generator`, distribuída sob licença MIT.

QR Code é uma marca registrada da DENSO WAVE INCORPORATED.

## Licença

Antes de publicar o repositório, inclua o arquivo de licença correspondente aos termos escolhidos para o projeto. A dependência incorporada mantém sua licença MIT original.
