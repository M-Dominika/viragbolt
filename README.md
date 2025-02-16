<h2> Adatbázis: viragbolt (utf8_hungarian_ci)</h2>
<p>CREATE TABLE IF NOT EXISTS kategoriak (
    \n\tid INTEGER PRIMARY KEY AUTO_INCREMENT,
    \n\tnev TEXT NOT NULL
\n);
\n
\nCREATE TABLE IF NOT EXISTS aruk (
    \n\tid INTEGER PRIMARY KEY AUTO_INCREMENT,
    \n\tnev TEXT NOT NULL,
    \n\tkategoriaId INTEGER,
    \n\tleiras TEXT,
    \n\tkeszlet INTEGER,
    \n\tar INTEGER,
    \n\tkepUrl TEXT,
    \n\tFOREIGN KEY(kategoriaId) REFERENCES kategoriak(id)
\n);
</p>
