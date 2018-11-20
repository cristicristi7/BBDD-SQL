#mySQL

(We make tables of series, characters and relations).
~~~mySQL
CREATE TABLE CHARACTERS(
   ID             INT PRIMARY KEY ,
   NAME           CHAR(50) ,
   SURNAME        CHAR(50) ,
   NICKNAME       CHAR(20) ,
   POWER          CHAR(50) ,
   WORK           CHAR(50) ,
   AGE            INT      ,
   SEX            CHAR(1)
);

CREATE TABLE SERIES(
   ID                   INT PRIMARY KEY   NOT NULL,
   TITLE                CHAR(50)          NOT NULL,
   DESCRIPTION          CHAR(200)         NOT NULL,
   YEAR                 YEAR              NOT NULL,
   START                CHAR(3)           NOT NULL,
   NSEASONS             CHAR(3)           NOT NULL
);

CREATE TABLE RELATIONS(
    ID INT PRIMARY KEY,
    ID_SERIE INT,
    ID_CHARACTER INT
);

INSERT INTO RELATIONS VALUES (1, 1, 2);
INSERT INTO RELATIONS VALUES (2, 1, 4);
INSERT INTO RELATIONS VALUES (3, 1, 1);
INSERT INTO RELATIONS VALUES (4, 2, 1);
INSERT INTO RELATIONS VALUES (5, 3, 4);
INSERT INTO RELATIONS VALUES (6, 3, 5);
INSERT INTO RELATIONS VALUES (7, 4, 6);
INSERT INTO RELATIONS VALUES (8, 5, 7);
INSERT INTO RELATIONS VALUES (9, 5, 8);
INSERT INTO RELATIONS VALUES (10, 5, 9);
INSERT INTO RELATIONS VALUES (11, 5, 10); 



INSERT INTO SERIES VALUES (1, 'Defenders', 'They denfend things', 2016, 'S3', 5);
INSERT INTO SERIES VALUES (2, 'Iron Fist', 'They love iron', 2011, 'S2', 2);
INSERT INTO SERIES VALUES (3, 'Daredevil', 'They are pretty much evil', 2009, 'S1', 3);
INSERT INTO SERIES VALUES (4, 'Punisher', 'Punish in the ass', 2016, 'S2', 5);
INSERT INTO SERIES VALUES (5, 'Jessica Jones', 'Girls adventures', 2011, 'S1', 1);
INSERT INTO SERIES VALUES (6, 'Luke Cage', 'Luke is awesome', 2010, 'S2', 2);


INSERT INTO CHARACTERS VALUES (1, 'jessica', 'jones', 'jj', 'invisibilidad', 'secretaria', 18, 'M');
INSERT INTO CHARACTERS VALUES (2, 'trish', 'walker', 'walky', 'super fuerza', 'bombera', 22, 'M');
INSERT INTO CHARACTERS VALUES (3, 'malcom', 'ducasse', 'duque', 'super inteligencia', 'fontanero', 34, 'H');
INSERT INTO CHARACTERS VALUES (4, 'jeri', 'hogarth', 'jota', 'idiosincracia', 'influencer', 27, 'M');
INSERT INTO CHARACTERS VALUES (5, 'luke', 'cage', 'condon', 'volar', 'programador' , 48, 'H');
INSERT INTO CHARACTERS VALUES (6, 'clare', 'temple', 'clarita de huevo', 'respirar bajo el agua','sirena', 50, 'M');
INSERT INTO CHARACTERS VALUES (7, 'danny', 'ran', 'forest', 'correr mucho', 'atleta', 15, 'H');
INSERT INTO CHARACTERS VALUES (8, 'collen', 'wing', 'alita pollo', 'planear bajo', 'azafato', 29, 'H');
INSERT INTO CHARACTERS VALUES (9, 'matt', 'murdoc', 'murdok', 'inmortal', 'pensionista', 79, 'H');
INSERT INTO CHARACTERS VALUES (10, 'karen', 'pages', 'carita paginas', 'cambiar de cara', 'politica', 22, 'M');
INSERT INTO CHARACTERS VALUES (11, 'foggy', NULL, 'gustavo', 'croar', 'abogado', 53, 'H');
INSERT INTO CHARACTERS VALUES (12, 'frank', 'castle', NULL, NULL, NULL, 12, 'H');
~~~
