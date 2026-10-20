# FaceID Studio

Protótipo de reconhecimento facial no navegador usando face-api.js.

## Executar no VS Code

1. Extraia a pasta `faceid-studio` para um local de sua preferência.
2. Abra o VS Code e selecione **File > Open Folder** (Arquivo > Abrir Pasta).
3. Abra `index.html` com a extensão **Live Server** e clique em **Go Live**.
4. Permita o acesso à câmera. Os modelos são carregados pela internet.

Alternativa sem extensão: abra um terminal na pasta e execute `python -m http.server 8000`; depois acesse `http://localhost:8000`.

## Git e GitHub

No GitHub, crie um repositório novo chamado `faceid-studio`. Para simplificar, não marque a opção de adicionar README, licença ou `.gitignore` (este projeto já contém README).

Abra o terminal integrado do VS Code na pasta do projeto e execute, substituindo `SEU-USUARIO` pelo seu nome de usuário do GitHub:

```bash
git init
git add .
git commit -m "Primeira versão do FaceID Studio"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/faceid-studio.git
git push -u origin main
```

Se o Git pedir identidade, configure uma vez com seu nome e e-mail:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
```

Use o e-mail associado à sua conta GitHub se quiser que os commits apareçam no seu perfil. Ao fazer `git push`, o GitHub pode abrir uma janela de login no navegador.

## Atualizar o GitHub depois de editar

```bash
git add .
git commit -m "Descreva a alteração"
git push
```

## Privacidade e limites

- O repositório deve conter apenas o código. Não publique fotos, descritores biométricos, tokens, senhas ou dados pessoais.
- O protótipo salva descritores faciais no armazenamento local do navegador; isso não sincroniza cadastros entre dispositivos.
- A câmera exige permissão e normalmente funciona em `localhost` ou HTTPS.
- O reconhecimento pode errar e não garante identificação em todos os ângulos. Use apenas com consentimento e não como única verificação de identidade.
