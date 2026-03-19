```mermaid
 sequenceDiagram
	participant U as Usuário
	participant P as Plataforma
	participant Back as BackEnd
	participant B as Banco de dados com os jogos
	participant E as Plataforma externa
	
	U->>P: Pesquisa o jogo de interesse
	P->>Back: Manda pesquisar o jogo pedido
	Back->>B: Buscar Local do jogo com o menor preço
	B-->>B: Pesquisa local com o menor preço
	B-->>Back: Retorna o local com o menor preço e o preço
	Back-->>P: Retorna o local do jogo e preço
	P-->>U: Informa pro usuário o preço e plataforma que esta o jogo
	U->>E: Manda para a plataforma com o jogo
	
