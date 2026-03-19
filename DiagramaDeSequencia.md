```mermaid
 sequenceDiagram
	participant U as Usuário
	participant P as Plataforma
	participant B as Banco de dados com os jogos
	participant E as Plataforma externa
	
	U->>P: Pesquisa o jogo de interesse
	P->>B: Procura o jogo pesquisado
	B-->>P: Retorna o jogo procurado e o preço
	P-->>U: Informa pro usuário o preço e plataforma que esta o jogo
	P->>E: Manda para a plataforma com o jogo
	
