<h2> Adatbázis: viragbolt (utf8_hungarian_ci)</h2>
<p>CREATE TABLE IF NOT EXISTS kategoriak (
    id INTEGER PRIMARY KEY AUTO_INCREMENT,
    nev TEXT NOT NULL
);

CREATE TABLE IF NOT EXISTS aruk (
    id INTEGER PRIMARY KEY AUTO_INCREMENT,
    nev TEXT NOT NULL,
    kategoriaId INTEGER,
    leiras TEXT,
    keszlet INTEGER,
    ar INTEGER,
    kepUrl TEXT,
    FOREIGN KEY(kategoriaId) REFERENCES kategoriak(id)
);
</p>
