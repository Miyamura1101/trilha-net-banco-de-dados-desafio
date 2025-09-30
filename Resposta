-- 1 - Buscar o nome e o ano dos filmes

Select Nome, Ano 
From Filmes;

-- 2 - Buscar o nome e o ano dos filmes, ordenados por ordem crescente pelo ano

Select Nome, Ano 
From Filmes
Order by Ano ASC;

-- 3 - Buscar pelo filme de volta para o futuro, trazendo o nome, ano e a duração

Select Nome, Ano, Duracao 
From Filmes
Where Nome LIKE 'De Volta para o Futuro';

-- 4 - Buscar os filmes lançados em 1997

Select *
From Filmes
Where Ano = 1997;

-- 5 - Buscar os filmes lançados APÓS o ano 2000

Select *
From Filmes
Where Ano > 2000;

-- 6 - Buscar os filmes com a duracao maior que 100 e menor que 150, ordenando pela duracao em ordem crescente

Select *
From Filmes
Where Duracao > 100 And Duracao < 150
Order by Duracao ASC;

-- 7 - Buscar a quantidade de filmes lançadas no ano, agrupando por ano, ordenando pela duracao em ordem decrescente

Select Ano, Count(Ano) as Quantidade
From Filmes
Group by Ano
Order By COUNT(Ano) DESC;

-- 8 - Buscar os Atores do gênero masculino, retornando o PrimeiroNome, UltimoNome

Select PrimeiroNome, UltimoNome, Genero
From Atores
Where Genero LIKE 'M'

-- 9 - Buscar os Atores do gênero feminino, retornando o PrimeiroNome, UltimoNome, e ordenando pelo PrimeiroNome

Select PrimeiroNome, UltimoNome, Genero
From Atores
Where Genero LIKE 'F'
Order by PrimeiroNome;

-- 10 - Buscar o nome do filme e o gênero

Select f.Nome, g.Genero
From Filmes f
Join FilmesGenero fg on fg.IdFilme = f.id
Join Generos g on g.Id = fg.IdGenero;

-- 11 - Buscar o nome do filme e o gênero do tipo "Mistério"

Select f.Nome, g.Genero
From Filmes f
Join FilmesGenero fg on fg.IdFilme = f.id
Join Generos g on g.Id = fg.IdGenero
Where g.Genero LIKE 'Mistério';

-- 12 - Buscar o nome do filme e os atores, trazendo o PrimeiroNome, UltimoNome e seu Papel

Select f.Nome, a.PrimeiroNome, a.UltimoNome, e.Papel
From Filmes f
Join ElencoFilme e on e.IdFilme = f.Id
Join Atores a on a.Id = e.IdAtor;
