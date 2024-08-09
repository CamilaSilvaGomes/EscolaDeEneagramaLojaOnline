# EscolaDeEneagramaLojaOnline

**Este Website é o projeto final da formação: Avançado em Desenho e Programção de Website - Master D - Lisboa.**

Após definir o tema Eneagrama, conduzi uma pesquisa abrangente sobre websites relacionados a essa abordagem, além de explorar plataformas dedicadas à venda de cursos no âmbito educacional. 
Esta investigação me permitiu identificar as melhores práticas e funcionalidades essenciais para criar uma plataforma robusta e atrativa para os utilizadores interessados no estudo do Eneagrama. 
O próximo passo foi definir o design do produto, abordando aspetos cruciais para uma experiência de utilizadores positiva. Começamos estabelecendo o "style gap", garantindo consistência em todos os elementos visuais, como tipografia e cores, para evitar inconsistências que poderiam prejudicar a experiência do utilizador. Escolhemos uma paleta de cores harmoniosa que complementa a logomarca, reforçando a identidade visual do website. 
Utilizamos a ferramenta Figma para criar um wireframe detalhado do site, definindo a estrutura e o layout de cada página. Esse wireframe funcionou como um guia visual essencial para o desenvolvimento, garantindo que todas as partes do site estivessem bem organizadas e funcionais. Além disso, incorporamos mensagens claras e intuitivas para facilitar a navegação e melhorar a interação do utilizador com o website, assegurando uma experiência agradável e eficiente. Para nos organizarmos de maneira eficiente, também criamos um sitemap detalhado do website, ilustrando todas as interações entre as páginas. Isso permitiu uma visão clara da arquitetura do site, ajudando a manter a consistência e a fluidez da navegação. As linguagens de programação utilizadas no desenvolvimento do website incluem HTML e CSS, complementadas pela biblioteca Bootstrap para garantir um design responsivo e moderno. Também empregamos JavaScript para criar interatividade e melhorar a experiência do utilizador. No back-end, utilizamos PHP para a lógica de servidor e a interação com o banco de dados, assegurando que os dados fossem gerenciados de maneira eficiente e segura.


**Funcionalidades por Página:** 

O website é composto por onze páginas. Ao se logar no site, o utilizador é recebido com uma saudação personalizada que utiliza a variável "nome" da tabela utilizador, melhorando a experiência de uso.

**- Página Principal (index):** esta página é de boas-vindas e contém informações gerais sobre o Eneagrama. Apresenta um carrossel com três imagens ilustrativas, transmitindo a essência do Eneagrama.

**- Página Sobre o Eneagrama:** nesta página, apresentamos uma explicação sobre os nove tipos de personalidades descritos pelo Eneagrama, proporcionando ao usuário uma compreensão de cada tipo e suas características.

**- Página de Cursos:** nesta página, são exibidos os cursos disponíveis para compra. Ao clicar no botão "Adicionar ao Carrinho", se o utilizador não estiver logado, será redirecionado para a página de login. Caso o utilizador ainda não tenha um registo, a página de login possui um link para a página de registro. Após completar o registro e o login, o utilizador é automaticamente direcionado para a página do carrinho, onde será apresentado o curso que adicionou, e pode realizar a ação de concluir a compra do curso.

**- Página de Carrinho:** esta página é a mais complexa em termos de programação e está dividida em duas seções principais:
Carrinho de Compras: nesta seção, são exibidos os cursos que o utilizador adicionou ao carrinho utilizando o botão "Adicionar ao Carrinho". O utilizador pode optar por "Voltar aos Cursos" para retornar à página de cursos e adicionar mais itens ao carrinho. Além disso, o botão "Excluir" permite remover cursos específicos do carrinho. Para finalizar a compra, o utilizador deve clicar em "Finalizar Compra". Após a conclusão da transação, o carrinho é esvaziado e todas as informações são removidas. Os detalhes da compra são registados na tabela de compras no banco de dados. Caso o utilizar efetue a compra de mais de um curso, na tabela de compras o registo é feito por curso, cada curso comprado tem o seu registo na tabela.
Cursos Comprados: esta seção apresenta um resumo de todos os cursos que o utilizador adquiriu, permitindo uma visão clara e organizada dos produtos comprados.

**- Página de Imersões:** nesta página, são exibidas as imersões programadas para ocorrer ao longo do ano. O utilizador pode manifestar interesse clicando no botão "Tenho Interesse". Ao clicar, é exibido um formulário para que o usuário preencha com suas informações pessoais e quaisquer dúvidas relacionadas às imersões.

**- Página de Interesse:** quando o utilizador clica no botão "Tenho Interesse" na página de Imersões, ele é redirecionado para o formulário de interesse. Neste formulário, o utilizador pode especificar a imersão desejada e inserir uma mensagem com suas dúvidas e perguntas. Ao clicar em "Enviar", as informações fornecidas são registradas na tabela de interesse no banco de dados, permitindo um acompanhamento eficiente das consultas e preferências dos utilizadores.

**- Página Fale Conosco:** esta página disponibiliza um formulário para que o utilizador possa enviar dúvidas e questões gerais sobre o site, informações sobre os cursos ou outros assuntos. Após preencher o formulário e clicar em "Enviar", as informações são registradas na tabela de contatos, no banco de dados.

**- Página de Login:** nesta página, o utilizador pode realizar o acesso ao site inserindo o login e senha. Após o login bem-sucedido, o utilizador é automaticamente redirecionado para a página do carrinho. No menu de navegação, aparecem dois novos links: um para o carrinho e outro para o logout. Além disso, o menu exibe uma saudação personalizada, como "Olá, [nome]", utilizando a
variável correspondente ao nome do utilizador registrado na tabela de utilizadores. 
Existem dois tipos de acesso: Acesso de Utilizador: O utilizador é direcionado para a página do carrinho ao acessar o portal.
Acesso de Administrador: O administrador é direcionado para a página de administração, onde pode gerenciar os cursos e utilizadores da aplicação.

**- Página de Administrador:** com acesso de administrador, o utilizador entra na página de administração, onde pode gerenciar os cursos disponíveis no site. As funcionalidades incluem a adição de novos cursos, a exclusão de cursos existentes e a atualização das informações dos cursos atuais. Além disso, é possível gerenciar a lista de utilizadores, incluindo a edição de registros e a exclusão de contas. O acesso a página de administração é feito ao clicar em cima da saudação "Olá, [administrador]". Para proteger as informações dos utilizadores, foi implementada uma restrição: se um utilizador tiver compras associadas, não será possível excluí-lo do sistema.
Uma mensagem de alerta é exibida nesses casos para garantir que nenhuma ação de exclusão seja realizada erroneamente.

**- Página de Registro:** nesta página, o utilizador pode criar suas credenciais de acesso ao site. Ao preencher o formulário com suas informações, os dados são salvos na tabela de utilizadores do banco de dados, permitindo o gerenciamento e a autenticação do acesso ao portal.

**- Logout:** Quando o utilizador está logado no site, a opção de logout está disponível em todas as páginas. Ao clicar em "Logout", a sessão do utilizador é encerrada e ele é automaticamente
redirecionado para a página principal (index).
