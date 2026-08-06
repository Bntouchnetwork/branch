# Reupload — bntouchnetwork.github.io/branch/

## O que aconteceu antes

O `index.html` subiu sozinho, sem a pasta `assets`. A página procurava o CSS, o JavaScript e o logo, recebia erro 404 nos três, e o navegador mostrava só o texto puro.

## O que mudou neste pacote

O `index.html` agora é **autossuficiente**: CSS, JavaScript, logo e ícone estão embutidos dentro dele. Mesmo que nada mais suba, a página aparece completa e estilizada.

A pasta `assets` continua aqui, mas só com imagens acessórias. Se ela faltar, você perde apenas a miniatura de compartilhamento e o ícone da aba — o site em si não quebra.

Todos os endereços já apontam para `https://bntouchnetwork.github.io/branch/`.

---

## Como subir

### Opção A — só o essencial (1 minuto)

Se quiser resolver agora e cuidar do resto depois:

1. Abra o repositório no GitHub e entre na pasta `branch`
2. Clique no `index.html` atual
3. Clique no ícone de lápis (Edit)
4. `Ctrl+A` e apague tudo
5. Abra o `index.html` deste pacote num editor de texto, copie todo o conteúdo e cole
6. **Commit changes**

Recarregue a página em um ou dois minutos. Ela já vem estilizada.

### Opção B — pacote completo (recomendado)

1. No repositório, entre na pasta `branch`
2. **Add file → Upload files**
3. Arraste **os arquivos da raiz** deste pacote: `index.html`, `404.html`, `favicon.ico`, `robots.txt`, `sitemap.xml`, `site.webmanifest`
4. **Commit changes**
5. Repita o processo, agora arrastando a **pasta `assets` inteira**

> Se o navegador não aceitar a pasta, crie os arquivos um a um: **Add file → Create new file**, e digite `assets/og-image.jpg` no nome — a barra faz o GitHub criar a pasta sozinho. Só que esse método não aceita imagens; nesse caso use **Upload files** já dentro da pasta `assets`.

### O arquivo `.nojekyll`

Ele é vazio e começa com ponto, então o Finder e o Explorer costumam escondê-lo, e o upload pelo navegador pode ignorá-lo. Se não aparecer no repositório:

**Add file → Create new file** → digite `.nojekyll` no nome → deixe em branco → **Commit**.

Sem ele, o GitHub processa o site pelo Jekyll e pode ignorar pastas — foi um dos suspeitos do problema anterior.

---

## Como confirmar que funcionou

Abra `https://bntouchnetwork.github.io/branch/` numa aba anônima (para escapar do cache).

Deve aparecer: fundo preto esverdeado, barra verde correndo no topo, logo GlobalNet e a chamada em caixa alta condensada. Se ainda vier texto branco com links azuis, o navegador está servindo a versão antiga do cache — force com `Ctrl+Shift+R`.

---

## Ainda pendente

- Links de **Política de Privacidade** e **Termos de Uso** no rodapé (hoje `href="#"`)
- **Ativação do formulário**: envie o formulário uma vez e clique no e-mail de confirmação que o FormSubmit manda para `info@globalnetmortgage.com`. Até isso, nenhuma mensagem é entregue.
- Confirmar no [NMLS Consumer Access](https://www.nmlsconsumeraccess.org) os estados de atuação, para ajustar o texto "alcance nacional" da seção 04
