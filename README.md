# SQL-alunos2
https://github.com/lucascalu/SQL_ALUNOS/blob/main/01.jpg

JPG 01

SELECT AVG(IDADE) AS MediaIdades FROM alunos;

SELECT SUM(IDADE) AS SomaIdades FROM alunos;

SELECT AVG(IDADE) AS MediaIdadeAlunas FROM alunos WHERE NOME LIKE 'A%' OR NOME LIKE 'I%';

SELECT AVG(IDADE) AS MediaIdadeAlunos FROM alunos WHERE NOME NOT LIKE 'A%' AND NOME NOT LIKE 'I%';

SELECT SUM(IDADE) AS SomaIdadeAlunos FROM alunos WHERE NOME NOT LIKE 'A%' AND NOME NOT LIKE 'I%';

#SELECT SUM(IDADE) AS SomaIdadeAlunas FROM alunos WHERE NOME LIKE 'A%' OR NOME LIKE 'I%';

JPG 02

-- Contagem de alunos com a letra 'b' no nome SELECT COUNT(*) AS total_alunos_com_b FROM alunos WHERE NOME LIKE '%b%' OR SOBRENOME LIKE '%b%';

SELECT SUM(IDADE) AS SomaIdade FROM alunos WHERE NOME LIKE '%S%' OR SOBRENOME LIKE '%S%';

SELECT AVG(IDADE) AS MediaIdade FROM alunos WHERE NOME LIKE 'I%' AND SEXO = 'Feminino';

SELECT AVG(IDADE) AS MediaIdade FROM alunos WHERE NOME LIKE 'G%' AND SEXO = 'Masculino';

SELECT SUM(IDADE) AS SomaIdadesComA FROM alunos WHERE NOME LIKE '%A%';

SELECT SUM(IDADE) AS SomaIdadesComF FROM alunos WHERE NOME LIKE '%F%';



JPG 03

SELECT MAX(IDADE) AS IdadeMaximaComC FROM alunos WHERE NOME LIKE '%C%';

SELECT MIN(IDADE) AS IdadeMinima FROM alunos WHERE NOME LIKE '%f%' AND SEXO = 'Masculino';

SELECT MAX(IDADE) AS IdadeMaxima FROM alunos WHERE NOME LIKE 'G%' AND SEXO = 'Feminino';

SELECT MIN(IDADE) AS IdadeMinima FROM alunos WHERE NOME LIKE 'R%' AND NOME <> 'Ryan' AND SEXO = 'Masculino';

SELECT SUM(MinIdade + MaxIdade) AS SomaIdadesAlunos FROM ( SELECT MIN(IDADE) AS MinIdade, MAX(IDADE) AS MaxIdade FROM alunos WHERE NOME <> 'Ryan' ) AS IdadesAlunos;

SELECT SUM(IDADE) AS SomaIdadesAlunas FROM alunos WHERE NOME LIKE '%A%' AND SEXO = 'Femin
