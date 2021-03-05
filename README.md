<h1 align="center">
📄<br>COMMITS SEMÂNTICOS
<a href="apresentation.pdf" target="_blank">Apresentação PDF</a>
</h1>

<h1 align="center">
  <img src="gitcommit.png"> 
</h1>

<p>
  De acordo com a documentação do <strong>Convetional Commits</strong>, Commits Semânticos são uma convenção simples para ser utilizada nas mensagens de commit. Essa convenção define  um conjunto de regras para criar um histórico de commit explícito, o que facilita a criação de ferramentas automatizadas.
</p>

<p>
  Esses commits auxiliarão você e sua equipe a entenderem de forma facilitada quais alterações foram realizadas no trecho de código que foi commitado.
</p>

<p>
  Essa identificação ocorre por meio de uma palavra e emoji que identifica se aquele commit realizado se trata de uma alteração de código, atualização de pacotes, documentação, alteração de visual, teste...
</p>


## 🦄 Tipo e Descrição

O commit semântico possui os elementos estruturais abaixo (tipos), que informam a intenção do seu commit ao utilizador(a) de seu código.

- `fix` - Commits do tipo fix Essencialmente definem o tratamento de correções de bugs;

- `feat`- Commits do tipo feat Tratam adições de novas funcionalidades ou dequaisquer outras novas implantações ao código;

- `docs` - Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. (Não inclui alterações em código);

- `style` - Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons, trailing spaces, lint... (Não inclui alterações em código);

- `refactor` - Commits do tipo refactor Tipo utilizado em quaisquer mudanças que sejam  executados no código, porém não alterem a funcionalidade final da tarefa impactada;

- `build` - Commits do tipo build  Alterações que afetam o sistema de construção ou dependências externas (escopos de exemplo: gulp, broccoli, npm);

- `test` - Commits do tipo test Adicionando testes ausentes ou corrigindo testes existentes nos processos de testes automatizados (TDD);
  
- `env` - Commits do tipo env utilizado quando se modifica ou adiciona algum arquivo de CI/CD.Exemplo: modificar um comando do Dockerfile ou adicionar um step a um Jenkinsfile.

- `chore` - Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)


## 🎉 Escopos <tipo>[escopo opcional]: <descrição> 
<table>
  <thead>
    <tr>
      <th>Commit semântico</th>
      <th>Commit comum</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>feat(login/routes): novas configurações
de rota para o login</td>
      <td> melhorando as configurações de login </td>
    </tr>
    <tr>
      <td> fix(AuthService): ajustando a url de
autenticação</td>
      <td> correção url de autenticação</td>
    </tr>
    <tr>
      <td> refactor: padronizando logs em todo o
serviços   </td>
      <td> ajustando o log de serviços </td>
    </tr>
    <tr>
      <td>  style: indentação e padronização no
código usando o lint:fix </td>
      <td> padronização de código  </td>
    </tr>
    <tr>
      <td>  build: adicionando variável para rebuild
automáticos nos containers docker  </td>
      <td> ajustes no containers docker </td>
    </tr>
  </tbody>
</table>


## 💻 Exemplo
```bash
git commit -am "feat(routes/settings): adjust settings to be called in any screen"
```
```bash
git commit -am "feat: ajuste as configurações de rotas a serem chamadas em qualquer tela"
```



## 💈 Padrões de emojis (opcional)

<table>
  <thead>
    <tr>
      <th>Tipo de commit</th>
      <th>Emojis </th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>Commit inicial  </td>
      <td> 🎉 <code>:tada:</code>   </td>
    </tr>
    <tr>
      <td> Tag de versão  </td>
      <td> 🔖 <code>:bookmark:</code>   </td>
    </tr>
    <tr>
      <td>  Novo recurso   </td>
      <td> ✨ <code>:sparkles:</code>   </td>
    </tr>
    <tr>
      <td>  Bugfix  </td>
      <td> 🐛 <code>:bug:</code>   </td>
    </tr>
    <tr>
      <td>  Documentação  </td>
      <td> 📚 <code>:books:</code>   </td>
    </tr>
    <tr>
      <td>  Testes  </td>
      <td> 🚨 <code>:rotating_light: </code>   </td>
    </tr>
    <tr>
      <td>Adicionando um teste</td>
      <td> ✅ <code> :white_check_mark: </code>   </td>
    </tr>
    <tr>
      <td> Teste de aprovação </td>
      <td> ✔️ <code> :heavy_check_mark: </code>   </td>
    </tr>
    <tr>
      <td>  Acessibilidade    </td>
      <td> ♿ <code> :wheelchair: </code>   </td>
    </tr>
    <tr>
      <td>  Texto     </td>
      <td> 📝 <code> :pencil: </code>   </td>
    </tr>
    <tr>
      <td>  Package.json em JS      </td>
      <td> 📦 <code> :package: </code>   </td>
    </tr>
    <tr>
      <td>  Em progresso        </td>
      <td> 🚧 <code> :construction: </code>   </td>
    </tr>
    <tr>
      <td>   Arquivos de configuração        </td>
      <td> 🔧 <code> :wrench: </code>   </td>
    </tr>
    <tr>
      <td>   Removendo uma dependência        </td>
      <td> ➖ <code> :heavy_minus_sign: </code>   </td>
    </tr>
    <tr>
      <td>   Adicionando uma dependência        </td>
      <td> ➕ <code> :heavy_plus_sign: </code>   </td>
    </tr>
    <tr>
      <td>   Revertendo mudanças         </td>
      <td> 💥 <code> :boom: </code>   </td>
    </tr>
    <tr>
      <td>   Alterações de revisão de código        </td>
      <td> 👌 <code> :ok_hand: </code>   </td>
    </tr>
    <tr>
      <td>   Mover/Renomear        </td>
      <td> 🚚 <code> :truck: </code>   </td>
    </tr>
  </tbody>
</table>
