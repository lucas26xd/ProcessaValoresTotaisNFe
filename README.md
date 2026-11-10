<div align="center">

# 🧾 ProcessaValoresTotaisNFe

**Processe arquivos XML de NFS-e e confira valores e retenções em segundos.**

Uma aplicação web simples e standalone, criada para automatizar tarefas do dia a dia contábil.

[![HTML](https://img.shields.io/badge/HTML-5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS-3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?logo=javascript&logoColor=222)](https://developer.mozilla.org/docs/Web/JavaScript)
[![Sem dependências](https://img.shields.io/badge/dependências-zero-2ea44f)](#tecnologias)
[![Execução local](https://img.shields.io/badge/processamento-local-6f42c1)](#privacidade)

</div>

---

## ✨ Visão geral

O **ProcessaValoresTotaisNFe** lê arquivos XML de NFS-e diretamente no navegador e organiza os principais dados fiscais em uma visualização clara. Selecione uma pasta ou arraste os arquivos para consultar os valores por nota e os totais do conjunto.

> Feito para simplificar uma rotina contábil: menos consulta manual de XMLs e mais praticidade na conferência.

## 🖼️ Prévia da interface

![Prévia ilustrativa da interface do Processador de NFS-e](docs/screenshot.svg)

<sub>Imagem ilustrativa da interface; os dados exibidos são fictícios.</sub>

## 🚀 Funcionalidades

- 📂 Seleção de uma pasta com arquivos XML ou de arquivos individuais.
- 🖱️ Arraste e solte de arquivos na área de envio.
- 🧾 Visualização de número, emissão, competência, emitente, tomador e descrição do serviço.
- 💰 Exibição dos valores de serviço, líquido e desconto incondicionado.
- 🧮 Soma dos valores das notas processadas.
- 🔎 Indicação de arquivos processados e arquivos com erro.
- 📱 Interface responsiva para diferentes tamanhos de tela.

## ⚙️ Como funciona

1. **Abra a aplicação** no navegador.
2. **Selecione uma pasta** com XMLs de NFS-e ou arraste os arquivos para a área indicada.
3. **O navegador lê os arquivos** e interpreta os campos disponíveis no XML.
4. **Confira os resultados:** totais consolidados e detalhes de cada nota aparecem na tela.
5. **Verifique os arquivos sinalizados** caso algum XML não possa ser processado.

A aplicação é feita em HTML, CSS e JavaScript, sem servidor, banco de dados ou etapa de instalação de dependências. A leitura é realizada localmente no navegador.

## 💡 Exemplo de uso

Imagine uma pasta com três XMLs de NFS-e. Depois de selecioná-la, a tela apresenta a quantidade de notas aceitas, os totais calculados e um cartão de detalhes para cada documento. Por exemplo:

| Informação | Exemplo ilustrativo |
| --- | ---: |
| Notas processadas | 3 |
| Valor total dos serviços | R$ 3.000,00 |
| Valor total líquido | R$ 2.850,00 |
| Desconto incondicionado total | R$ 0,00 |

Os valores acima são apenas um exemplo. O resultado depende das informações presentes nos arquivos selecionados.

## 🧑‍💻 Como executar

### Abrir diretamente

1. Clone o repositório:
   ```bash
   git clone https://github.com/lucas26xd/ProcessaValoresTotaisNFe.git
   ```
2. Entre na pasta:
   ```bash
   cd ProcessaValoresTotaisNFe
   ```
3. Abra `index.html` em um navegador moderno.

### Usar um servidor local (opcional)

```bash
python -m http.server 8000
```

Acesse [http://localhost:8000](http://localhost:8000).

## 🔒 Privacidade e compatibilidade

- Os XMLs são lidos no navegador; o projeto não envia os arquivos para um backend.
- A aplicação espera XMLs compatíveis com o padrão de NFS-e implementado no parser. Estruturas diferentes ou campos ausentes podem não ser exibidos como esperado.
- A seleção de pastas usa recursos do navegador; o suporte pode variar. Se necessário, arraste os arquivos XML diretamente.
- Confira os resultados antes de utilizá-los em procedimentos contábeis ou fiscais. A ferramenta é um apoio à conferência, não substitui a validação profissional.

## 🧰 Tecnologias

- HTML5
- CSS3
- JavaScript (sem frameworks)
- `DOMParser` para leitura de XML no navegador

## 📁 Estrutura do projeto

```text
ProcessaValoresTotaisNFe/
├── docs/
│   └── screenshot.svg
├── index.html
└── README.md
```

## 📄 Licença

O repositório não especifica uma licença. Consulte o mantenedor antes de reutilizar ou distribuir o código.

## 👤 Autor

Desenvolvido por [Lucas](https://github.com/lucas26xd).
