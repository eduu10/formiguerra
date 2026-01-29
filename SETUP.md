# Formiguerra - Sincronização com itch.io

Este repositório armazena os arquivos do jogo Formiguerra e sincroniza automaticamente com itch.io.

## Como usar

### 1. Atualizar os arquivos do jogo
- Baixe a versão mais recente do seu jogo do Google Drive
- - Coloque os arquivos na pasta principal do repositório
 
  - ### 2. Fazer upload para o GitHub
  - ```
    git add .
    git commit -m "Descrição da atualização"
    git push origin main
    ```

    ### 3. Sincronizar com itch.io

    Escolha uma das opções:

    **OPÇÃO A: Upload Manual (Mais Simples)**
    1. Vá para https://eduu10.itch.io/formiguerra/edit
    2. 2. Na seção "Uploads", clique em "Upload files"
       3. 3. Selecione e envie os arquivos atualizados
         
          4. **OPÇÃO B: Butler (Automático - Recomendado)**
          5. 1. Instale Butler: https://itch.io/docs/butler/installing
             2. 2. Crie um API token no itch.io: https://itch.io/user/settings/api-keys
                3. 3. Execute para sincronizar:
                   4. ```
                      butler push ./formiguerra_web.zip eduu10/formiguerra:html --userversion=1.0.0
                      ```

                      ## Fluxo de trabalho

                      Google Drive → GitHub → itch.io

                      Baixe do Drive → Commit no GitHub → Sincronize com itch.io
