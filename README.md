# dev-rails-box
Uma box criada para facilitar o desenvolvimento de aplicações ruby on rails. 

<h4>Instalado:</h4>
  - Git 
  - rbenv (Gerenciador de versões do Ruby) (Versão instalada é a <b>2.2.4</b>)
  - postgresql
  - Rails 4
  - Heroku toolbelt

<h5>Utilização: </h5>

<h6> Vagrant </h6>

<p>
  Inicie sua maquina virtual com o comando <br>
  <code>
    vagrant up
  </code>
</p>

<p>
  Depois utilize o comando <br>
  <code>
    vagrant ssh
  </code>
</p>

<p>
  Caso esteja usando windows, utilize o programa <a href="http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html" target="_blank">PuTTY</a> como client ssh e o programa PuTTYgem para gerar uma chave ssh. 
</p>

<h6>Ruby </h6>

Essa box está utilizando a versão 2.2.4 do ruby. 
- Se desejar alterar a versão, utilize o comando rbenv versions para listar todas as versões disponíveis. 
- A seguir, utilize o comando <b>(Ex: <i>rbenv install 2.3.0</i>)</b>. <br> 
<code>
  rbenv install versão-desejada
</code> 
- Por ultimo use o comando <br>
<code>
  rbenv global versão-que-você-escolheu
</code>

<h6>Rails </h6>

- Crie seu projeto rails dentro da pasta /vagrant utilizando o camando <b>rails new nome-da-aplicacao</b>.
- Crie sua aplicação Rails com o comando a seguir: 
 
<code>
  rails new nome-da-app --database=postgresql
</code>

<h5 style="color:#0A0B52;">Rodando sua aplicação rails</h5>

<code>
  rails s -b 192.168.33.10
</code>

<h6>PostgreSQL</h6>

- Inicie com o comando <br>
<code>
  psql - U postgres -h localhost -W -d postgres
</code>

<h6>Descrição do comando: </h6>

- psql  - Invoca o postgresql
- -U    - User postgres
- -h    - Seu host, no nosso caso é localhost
- -W    - Forçar password
- -d    - database -> postgres




