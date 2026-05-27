# Minicurso Prático de Git e GitHub — IFSP

Este repositório contém a maquete e o código-fonte (HTML e CSS) da Landing Page do IFSP utilizada em nosso laboratório prático. O objetivo deste guia é servir como uma colinha rápida com todos os comandos essenciais ensinados ao longo do curso.

---

Antes de começar a registrar suas alterações, é obrigatório carimbar quem é o autor dos commits.
```bash
# Configura seu nome de usuário global no computador
git config --global user.name "Seu Nome"

# Configura seu e-mail global no computador
git config --global user.email "seuemail@exemplo.com"

# Verifica se os dados foram salvos corretamente
git config user.name
git config user.email

# Verifica o estado atual dos seus arquivos (Modificado, Pronto ou Não Rastreado)
git status

# Adiciona um arquivo específico para a área de preparação (Stage Changes)
git add index.html

# Adiciona TODOS os arquivos modificados da pasta de uma vez só
git add .

# Grava permanentemente suas alterações salvas na mala de preparação
git commit -m "Mensagem descritiva e clara do que foi resolvido"

# Lista todos os ramos existentes no seu projeto local
git branch

# Cria um novo ramo paralelo e altera seu ponteiro de trabalho para ele instantaneamente
git checkout -b nome-da-sua-branch

# Muda de uma branch para outra já existente (ex: voltando para a principal)
git checkout main

# Junta as alterações de um ramo secundário para dentro do ramo onde você está pisando agora
git merge nome-da-sua-branch

# Exibe o diário de bordo do projeto em uma única linha por alteração para caçar o histórico
git log --oneline

# DESCARTAR ALTERAÇÕES: Joga fora o que você editou e puxa a última versão salva (Discard Changes)
git checkout nome-do-arquivo.html

# REVERT (SEGURO): Cria um novo commit que faz o inverso do commit ruim para anular o erro
git revert <hash-do-commit-ruim>

# RESET (DRÁSTICO): Limpa o histórico local e força o projeto a voltar exatamente ao commit bom especificado
git reset --hard <hash-do-commit-bom>

# Envia suas alterações salvas locais (commits) direto para o servidor do GitHub
git push origin main

# Apenas espia e baixa o histórico novo da nuvem sem mexer ou misturar no seu código atual
git fetch origin

# Baixa as atualizações do GitHub e já as mistura (merge) direto na sua branch de trabalho atual
git pull
