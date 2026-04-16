<div class="container">
    <h1>Guia do Desenvolvedor: Clonar & Migrar</h1>
    <p>Este guia ensina como baixar este projeto e configurá-lo no <strong>seu próprio GitHub</strong> de forma rápida.</p>

   <hr>

 <h2>📥 Passo 1: Baixar o código original</h2>
    <p>Abra o seu terminal na pasta onde deseja salvar o projeto e digite:</p>
    <pre><code>git clone https://github.com/Luann8/LACIA-16-04.git
cd LACIA-16-04</code></pre>

   <hr>
    <h2>🔗 Passo 2: Desvincular do dono atual</h2>
    <p>Para você poder salvar na sua conta, precisamos remover a conexão com o repositório original:</p>
    <pre><code>git remote remove origin</code></pre>

   <hr>

   <h2>🌐 Passo 3: Conectar ao SEU repositório</h2>
    <p>Vá ao seu GitHub, crie um novo repositório vazio e copie a URL. Então, execute:</p>
    <pre><code>git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git</code></pre>
    <p><strong>⚠️ Atenção:</strong> Substitua <code>SEU_USUARIO</code> e <code>SEU_REPOSITORIO</code> pelos seus dados.</p>

   <hr>

  <h2>🚀 Passo 4: Padronizar e Enviar (Main)</h2>
    <p>Vamos garantir que a branch principal se chame <code>main</code> e enviar tudo:</p>
    <pre><code>git branch -M main
git push -u origin main</code></pre>

   <hr>

  <h2>⌨️ Atenção: Sair do editor Vim</h2>
    <p>Se o terminal "travar" em uma tela de texto (Vim), pressione <kbd>Esc</kbd>, digite <code>:q!</code> e aperte <kbd>Enter</kbd> para sair.</p>

   <hr>

   <h2>📌 Dicas de Uso Diário (Comandos Git essenciais)</h2>
    <h3>✅ Salvar mudanças localmente</h3>
    <pre><code>git add .
git commit -m "mensagem do commit"</code></pre>

   <h3>📤 Enviar para o GitHub</h3>
    <pre><code>git push</code></pre>

  <h3>📥 Baixar atualizações do GitHub</h3>
  <pre><code>git pull</code></pre>

  <h3>📜 Ver histórico de commits</h3>
    <pre><code>git log</code></pre>
    <p><strong>Dica:</strong> Para sair do log, pressione a tecla <kbd>q</kbd>.</p>

  <h3>🔍 Verificar status dos arquivos</h3>
    <pre><code>git status</code></pre>

   <h3>🌿 Ver e trocar de branch</h3>
    <pre><code>git branch           # lista branches
git checkout nome-da-branch   # troca de branch
git checkout -b nova-branch   # cria e troca para nova branch</code></pre>

 <h3>🔗 Ver repositórios remotos conectados</h3>
    <pre><code>git remote -v</code></pre>
    <hr>

   <h2>🛠️ Solução de problemas comuns</h2>

   <ul>
        <li><strong>Erro "fatal: remote origin already exists"</strong><br>
        <pre><code>git remote remove origin
git remote add origin URL_DO_SEU_REPOSITORIO</code></pre>
        </li>

        <li><strong>Push rejeitado (falta de permissão ou conflito)</strong><br>
        <pre><code>git pull origin main --allow-unrelated-histories
git push origin main</code></pre>
        </li>

  <li><strong>Esqueceu de mudar a branch para main</strong><br>
   <pre><code>git branch -M main</code></pre>
        </li>
        <li><strong>Desfazer último commit (mantém as alterações)</strong><br>
        <pre><code>git reset --soft HEAD~1</code></pre>
        </li>
     <li><strong>Desfazer último commit (descarta alterações)</strong><br>
        <pre><code>git reset --hard HEAD~1</code></pre>
        </li>

  <li><strong>Ver diferenças entre arquivos modificados</strong><br>
    <pre><code>git diff</code></pre>
        </li>
    </ul>

   <hr>

   <h2>📋 Fluxo completo (resumo)</h2>
    <pre><code># 1. Clonar
git clone https://github.com/Luann8/LACIA-16-04.git
cd LACIA-16-04

# 2. Remover vínculo original
git remote remove origin

# 3. Adicionar seu repositório
git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git

# 4. Renomear branch e enviar
git branch -M main
git push -u origin main

# 5. Dia a dia (após alterações)
git add .
git commit -m "descrição"
git push</code></pre>

 <hr>
    <p><strong>🎯 Objetivo alcançado:</strong> Agora o projeto está 100% vinculado ao SEU GitHub! Você pode compartilhar, colaborar ou continuar desenvolvendo.</p>

  <hr>
    <p><em>⚡ Guia prático para desenvolvedores — Repositório original: <strong>Luann8/LACIA-16-04</strong></em></p>
</div>
