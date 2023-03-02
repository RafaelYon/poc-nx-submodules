# poc-nx-submodules

Teste de app para microfrontend

comandos executados:

# Iniciando
<h2>#Cria um novo workspace integrado usando a estrutua de "app"</h2>
npx create-nx-workspace@15.0.4 poc-nx-submodules2 --nxCloud=false

<h2># Estrutura com o git submodules:</h2>
git submodule add -b main git@github.com:andersoncontreira/poc-nx-submodules-apps-host.git

<h2># Criar um novo app react</h2>
npm install --save-dev @nrwl/react </br>
npx nx generate @nrwl/react:app host

<h2># Atualização de arquivos pela raiz do projeto</h2>
git submodule foreach --recursive git pull
