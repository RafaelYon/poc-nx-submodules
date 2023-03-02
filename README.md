# poc-nx-submodules

Teste de app para microfrontend

comandos executados:

# Iniciando
## Cria um novo workspace integrado usando a estrutua de "app"
npx create-nx-workspace@15.0.4 poc-nx-submodules2 --nxCloud=false

# Estrutura com o git submodules:
git submodule add -b main git@github.com:andersoncontreira/poc-nx-submodules-apps-host.git

# Criar um novo app react
npm install --save-dev @nrwl/react
npx nx generate @nrwl/react:app host

# Atualização de arquivos pela raiz do projeto
git submodule foreach --recursive git pull
