# Tabela FIPE 2025

![HTML](https://img.shields.io/badge/HTML-5-orange)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)
![Tailwind](https://img.shields.io/badge/Tailwind-CSS-blue)
![API](https://img.shields.io/badge/API-FIPE-green)
![License](https://img.shields.io/badge/License-GNU-blue)

Uma aplicação web moderna para consulta de valores da tabela FIPE de veículos, desenvolvida como projeto acadêmico para a disciplina de Programação Orientada a Serviços (POS) do curso técnico de Informática para Internet.

## Sobre o Projeto

O **Tabela FIPE 2025** é uma aplicação que permite consultar valores oficiais da tabela FIPE para diversos tipos de veículos (carros, motos e caminhões) de forma simples e intuitiva. Após a consulta, o sistema busca automaticamente uma imagem do veículo selecionado para enriquecer a experiência do usuário.

## Funcionalidades

- ✅ Consulta de valores da tabela FIPE
- 🚗 Suporte a carros, motos e caminhões
- 🖼️ Busca automática de imagens dos veículos
- 🎨 Interface moderna com design neumórfico
- 📱 Layout responsivo
- ⚡ Carregamento rápido e eficiente

## Tecnologias Utilizadas

- **HTML5** - Estrutura da aplicação
- **Tailwind CSS** - Framework para estilização
- **JavaScript (ES6+)** - Lógica e interatividade
- **API FIPE** - Dados oficiais de veículos
- **Google Custom Search API** - Busca de imagens

## Configuração e Instalação

### Pré-requisitos

Para utilizar todas as funcionalidades do projeto, você precisará configurar as seguintes APIs:

### 1. Configuração da API do Google

#### Parte 1: Obter a Chave de API (API Key)

1. **Ative a API:**
   - Acesse a [Custom Search JSON API](https://console.cloud.google.com/apis/library/customsearch.googleapis.com)
   - Selecione ou crie um novo projeto
   - Clique em **"ATIVAR"**

2. **Crie a Chave:**
   - Vá para [Credenciais](https://console.cloud.google.com/apis/credentials)
   - Clique em **"+ CRIAR CREDENCIAIS"** → **"Chave de API"**
   - Copie a chave gerada

#### Parte 2: Obter o ID do Mecanismo de Pesquisa (CX)

1. **Acesse o Painel:**
   - Vá para [Mecanismo de Pesquisa Programável](https://programmablesearchengine.google.com/controlpanel/all)

2. **Crie um Novo Mecanismo:**
   - Clique em **"Adicionar"**
   - Dê um nome (ex: "Buscador FIPE")
   - Marque **"Pesquisar em toda a Web"**
   - Clique em **"CRIAR"**

3. **Configure e Copie o ID:**
   - Ative a opção **"Pesquisa de imagens"**
   - Copie o **"ID do mecanismo de pesquisa"** (CX)

### 2. Configuração no Código

No arquivo `script.js`, substitua as chaves padrão pelas suas credenciais:

```javascript
// COLE SUAS CHAVES DO GOOGLE AQUI
const GOOGLE_API_KEY = 'SUA_CHAVE_API_DO_GOOGLE_AQUI';
const SEARCH_ENGINE_ID = 'SEU_ID_DE_BUSCA_CX_AQUI';
```

## Como Usar

1. **Selecione o tipo de veículo:** Carros, Motos ou Caminhões
2. **Escolha a marca** do veículo desejado
3. **Selecione o modelo** específico
4. **Escolha o ano** de fabricação
5. **Visualize o resultado** com valor FIPE e imagem do veículo

## Estrutura do Projeto

```
tabela-fipe-2025/
│
├── index.html          # Estrutura principal da aplicação
├── script.js           # Lógica JavaScript e integração com APIs
├── LICENSE            # Licença GNU
└── README.md          # Este arquivo
```

## ⚠️ Observações Importantes

- O projeto utiliza a API pública da FIPE disponível em `parallelum.com.br`
- As imagens são buscadas automaticamente através da Google Custom Search API
- É necessário configurar suas próprias chaves de API para o funcionamento completo
- A aplicação é totalmente client-side (executa no navegador)

## 📄 Licença

Este projeto está licenciado sob a **Licença Pública Geral GNU (GPL)**. Isso significa que você pode:

- ✅ Usar o software para qualquer propósito
- ✅ Estudar como o programa funciona e adaptá-lo às suas necessidades
- ✅ Redistribuir cópias
- ✅ Melhorar o programa e liberar as melhorias para o público

**Condições da licença:**
- Você deve disponibilizar o código fonte de quaisquer trabalhos derivados
- Você deve manter os avisos de licença e copyright originais
- Quaisquer modificações devem ser licenciadas sob a mesma licença GPL

Para mais detalhes, consulte o arquivo [LICENSE](LICENSE) ou visite [https://www.gnu.org/licenses/gpl-3.0.html](https://www.gnu.org/licenses/gpl-3.0.html).

## 👨‍💻 Desenvolvido por Francisco

Projeto acadêmico desenvolvido para a disciplina de Programação Orientada a Serviços (POS) do curso técnico de Informática para Internet.

---

*Projeto atualizado em 2025*  
*Licenciado sob GNU General Public License v3.0*
