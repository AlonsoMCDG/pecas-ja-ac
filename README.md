# PeçasJá AC — Landing page

Página de pré-cadastro do **PeçasJá AC**, um marketplace local de peças automotivas e para motocicletas em Rio Branco (AC). A página apresenta a proposta e recebe o interesse de motoristas, oficinas e lojas parceiras.

Projeto desenvolvido para a disciplina **CCET183 – Gestão da Informação** (Bacharelado em Sistemas de Informação, UFAC).

**Autor:** Alonso Martins de Araújo

**Página publicada:** https://pecas-ja-ac.onrender.com/

## Conteúdo da página

- Chamada principal com as duas entradas: motoristas/oficinas e lojas parceiras.
- Explicação do problema e do processo em quatro passos (informe, encontre, compare e receba).
- Benefícios separados para cada público.
- Dois formulários de pré-cadastro, com aviso de finalidade e consentimento para o uso dos dados (Lei nº 13.709/2018, LGPD).

## Integração com Google Forms e planilhas

Os dois formulários da página enviam as respostas ao Google Forms, que grava cada envio em uma planilha do Google Sheets:

- **Motoristas e oficinas:** formulário próprio, com planilha de respostas própria.
- **Lojas parceiras:** formulário próprio, com planilha de respostas própria.

O envio acontece em uma janela oculta, então o visitante continua na página e vê a mensagem de confirmação. O botão mostra "Enviado" e só volta a ficar disponível quando algum campo é alterado.

Os campos do site têm os mesmos nomes e a mesma ordem das perguntas nos formulários. Se você alterar uma pergunta no Google Forms, é preciso atualizar o código `entry.` correspondente no `index.html`.

## Tecnologias

- HTML5: estrutura da página, com os textos, as seções e os formulários.
- CSS3: aparência da página, com cores, tipografia e layout adaptável para celular e computador. Suporta o modo claro e o escuro.
- JavaScript: validação dos campos e controle do botão de envio, sem frameworks nem dependências de build.
- GitHub para versionamento do código.
- Render para publicação da página como site estático.
- Google Forms e Google Planilhas: recebem e armazenam os cadastros (uma planilha por formulário).
- Google Fonts: Barlow Condensed e Source Sans 3 (licença SIL Open Font License).

## Como visualizar localmente

Não é preciso instalar nada. Abra o arquivo `index.html` em qualquer navegador.


## Limitações conhecidas

- Os cadastros são gravados em planilhas do Google Sheets, por meio do Google Forms. Uma planilha é um armazenamento simples, não um sistema gerenciador de banco de dados.
- Os dados enviados aparecem nas planilhas vinculadas aos formulários. A contagem e a análise por bairro ainda são feitas manualmente.
- A página não mostra disponibilidade de estoque em tempo real. A disponibilidade depende da confirmação de cada loja parceira.
- Os valores e condições citados (comissão de 10%, cadastro sem mensalidade) são premissas do plano de negócios, ainda não validadas no mercado.

## Estrutura do repositório

```
.
├── index.html   # página completa (HTML, CSS e JavaScript em um arquivo)
└── README.md    # este arquivo
```

## Projeto acadêmico

PeçasJá AC é um projeto acadêmico. Não somos uma loja e não temos vínculo com as marcas ou estabelecimentos citados.
