# Configurações Personalizadas para o VS Code

Este guia explica como configurar o seu Visual Studio Code com as personalizações incluídas neste repositório. Ele cobre configurações gerais, atalhos de teclado e a customização de estilo do editor.

---

## Configurar `settings.json`

1. Abra o arquivo `settings.json` deste repositório e copie todo o conteúdo.
2. No Visual Studio Code, pressione `Ctrl+Shift+P` (ou `Cmd+Shift+P` no macOS).
3. Procure e selecione **Preferences: Open User Settings (JSON)**.
4. Substitua o conteúdo do seu `settings.json` atual pelo conteúdo copiado.

---

## Configurar `keybindings.json`

1. Abra o arquivo `keybindings.json` deste repositório e copie todo o conteúdo.
2. Siga os mesmos passos acima, mas desta vez selecione **Preferences: Open Keyboard Shortcuts (JSON)**.
3. Substitua o conteúdo do seu arquivo `keybindings.json` pelo conteúdo copiado.

---

## Customizar o Estilo do VS Code

### Requisitos
Você precisará instalar a extensão **Custom CSS and JS Loader**.

1. No VS Code, pressione `Ctrl+P` (ou `Cmd+P` no macOS) e digite:
   ```plaintext
   ext install be5invis.vscode-custom-css
   ```
   Pressione Enter para instalar.
2. Alternativamente, acesso o [***link oficial da extensão***](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css) para intalar

## Configuraçõs

1. Abra o arquivo `settings.json` no VS Code, conforme descrito anteriormente.
2. Encontre ou adiocione a propriedade:
    ```json
    "vscode_custom_css.imports": []
    ```
3. No array, insira as URLs dos arquivos CSS e JS personalizados. Por exemplo:
    ```json
    "vscode_custom_css.imports": [
        "file:///CAMINHO/PARA/custom.css",
        "file:///CAMINHO/PARA/custom.js"
    ]
    ```
    Substitua CAMINHO/PARA pelo caminho onde você armazenou os arquivos da pasta `custom-css-and-js` fornecidos pelo repositório.

4. Após salvar as alterações, reinicie o VS Code.
5. Pressione F1 ou Ctrl+Shift+P, procure por Enable Custom CSS and JS, e ative as customizações.
6.Reinicie o VS Code novamente para aplicar as mudanças.

> Qualquer dúvida sobre a extensão pode ser esclarecida no [***README oficial***](https://github.com/be5invis/vscode-custom-css/blob/master/README.md).

## Disclaimer

Caso não esteja usando o tema '[*Min Theme*](https://marketplace.visualstudio.com/items?itemName=miguelsolorio.min-theme) Dark' pode-se haver conflitos entre as cores, mas isso pode ser resolvido manualmente apenas modificando ou removendo as cores do seu arquivo css.

---

Inspiração: [***Glenn Raya***](https://www.youtube.com/watch?v=9_I0bySQoCs)
