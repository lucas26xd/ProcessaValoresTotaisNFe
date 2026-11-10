# ProcessaValoresTotaisNFe

Página standalone para automatizar o processamento de notas fiscais de serviço eletrônicas (NFS-e) em arquivos XML.

A aplicação permite selecionar uma pasta ou arquivos XML, interpretar os dados da nota, calcular totais e exibir um resumo completo de cada NFS-e processada.

## Descrição

Este projeto foi criado para facilitar o dia a dia de trabalho de uma contadora, automatizando a leitura de arquivos XML de NFS-e e apresentando informações como:

- número da NFS-e
- data de emissão
- competência
- emitente e tomador
- descrição do serviço
- valor do serviço
- valor líquido
- desconto incondicionado
- retenções de ISS e PIS/COFINS
- somatório total dos arquivos processados

## Funcionalidades

- upload de uma pasta contendo arquivos XML
- upload de arquivos XML isolados
- arraste e solte de arquivos no navegador
- processamento local no frontend
- cálculo automático de totais por arquivo/processados
- exibição do resumo de cada NFS-e em cards visuais
- identificação de arquivos inválidos ou não processados

## Como usar

### Opção 1: abrir diretamente no navegador

1. Clone o repositório:
   ```bash
   git clone https://github.com/lucas26xd/ProcessaValoresTotaisNFe.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd ProcessaValoresTotaisNFe
   ```
3. Abra o arquivo `index.html` em qualquer navegador moderno.

### Opção 2: rodar um servidor local

Se preferir, pode servir a aplicação localmente para evitar algumas restrições do navegador:

```bash
cd ProcessaValoresTotaisNFe
python -m http.server 8000
```

Depois abra no navegador:

```text
http://localhost:8000
```

## Estrutura do projeto

```text
ProcessaValoresTotaisNFe/
├── index.html
├── .gitignore
├── .gitattributes
└── README.md
```

## Observações

- O processamento é feito no navegador, sem backend ou banco de dados.
- A aplicação depende de arquivos XML no padrão NFS-e esperado pela lógica de extração.
- É uma solução prática e leve, ideal para uso pontual e automatização de cálculos contábeis.

## Tecnologias

- HTML
- CSS
- JavaScript
- DOMParser para leitura de XML no navegador

## Licença

Este projeto não informa uma licença específica no repositório. Caso queira distribuir ou reutilizar o código em produção, verifique com o mantenedor antes de usar em contexto comercial.

## Autor

- Lucas

## Dica de uso

Para uma experiência mais organizada, mantenha os XMLs em uma pasta separada e use a opção de seleção da pasta para processar vários documentos de uma vez.
