# Safe Download - GitHub Pages

Página de download segura com proteção contra bots, hospedada no GitHub Pages.

## 🚀 Como Usar

### 1. Criar um Repositório no GitHub

1. Acesse [github.com/new](https://github.com/new)
2. Preencha:
   - **Repository name**: `safe-download` (ou outro nome)
   - **Description**: `Página de download segura`
   - **Public**: Deixe público
   - **Initialize this repository**: Deixe desmarcado
3. Clique em **"Create repository"**

### 2. Upload dos Arquivos

**Opção A: Via GitHub Web**
1. Clique em **"Add file"** → **"Upload files"**
2. Arraste o arquivo `index.html` para a área
3. Clique em **"Commit changes"**

**Opção B: Via Git (Terminal)**
```bash
git clone https://github.com/seu-usuario/safe-download.git
cd safe-download
# Copie o arquivo index.html aqui
git add index.html
git commit -m "Adicionar página de download"
git push origin main
```

### 3. Ativar GitHub Pages

1. Vá para **Settings** do repositório
2. Clique em **"Pages"** (lado esquerdo)
3. Em **"Source"**, selecione **"Deploy from a branch"**
4. Selecione **"main"** e **"/ (root)"**
5. Clique em **"Save"**

Aguarde alguns minutos e sua página estará disponível em:
```
https://seu-usuario.github.io/safe-download
```

### 4. Configurar o Link de Download

Abra o arquivo `index.html` e procure por esta linha:

```javascript
const DOWNLOAD_LINK = 'https://gatasexy.com';
```

Substitua `https://gatasexy.com` pelo seu link real de download.

**Exemplo:**
```javascript
const DOWNLOAD_LINK = 'https://exemplo.com/app-v2.0.apk';
```

Depois faça commit e push das mudanças:
```bash
git add index.html
git commit -m "Atualizar link de download"
git push origin main
```

## 🔒 Recursos de Segurança

✅ **Cronômetro de Verificação**: 15 segundos antes de liberar o download
✅ **Proteção contra Bots**: Detecta e bloqueia Googlebot, Bingbot, etc
✅ **Meta Tags**: `noindex` e `nofollow` para não indexar
✅ **Design Dark Mode**: Interface elegante e profissional
✅ **Sem Servidor**: Funciona 100% no GitHub Pages (grátis)

## 📝 Estrutura

```
safe-download/
├── index.html          # Página principal
└── README.md           # Este arquivo
```

## 🎯 Fluxo de Uso

1. Usuário acessa a página
2. Clica em "OBTER AGORA"
3. Cronômetro de 15 segundos começa
4. Após terminar, botão muda para "BAIXAR AGORA"
5. Clica no botão e é redirecionado para o link

## ⚠️ Importante

- O link é armazenado no código JavaScript
- Para trocar o link, você precisa editar o arquivo e fazer push
- Não há painel admin (seria necessário um servidor)
- A proteção contra bots é básica (JavaScript puro)

## 📞 Suporte

Se precisar de ajuda, abra uma issue no repositório.

---

**Criado com ❤️ para proteção de downloads**
