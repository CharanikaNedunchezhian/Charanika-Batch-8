create database BooksDB;
create table BooksDB.Books(
     Books_id int primary key auto_increment,
     Books_Title varchar(50),
     Books_Author varchar(50),
     Books_genre varchar(100),
     publication_year int ,
     Book_price int );
create table BooksDB.Author(
     SI_NO int primary key auto_increment,
	 Author_name varchar(50),
     Book_Title varchar(50),
     foreign key(SI_NO) References Books(Books_id));
select * from BooksDB.Books;
select * from BooksDB.Author;
insert into BooksDB.Books values
     (1,"PS","Kalki","Historical",1930,1000),
     (2,"The tempist","shakesphere","Drama",1623,1050),
	 (3,"Mr.Bean","Mr.Bean","Comedy",1851,1001),
	 (4,"War And Peace","Tolstoy","History",1869,299),
     (5,"7 Stages of life","Shakesphere","Poetry",1610,500);
insert into BooksDB.Author values
     (1,"Mahatma Gandhi","The Story of Truth"),
     (2,"R.K.Narayan","The Giude"),
     (3,"Rohinton Mistry","A Fine Balance"),
     (4,"Salman Rushidie","Midnights Cildren"),
     (5,"Vikram Seth","A Suitable Boy");
--select distinct Books_Title from BooksDB.Books;
--select distinct Book_Title from BooksDB.Author;
update BooksDB.Books set Books_Title="National anthem" where Books_id=5;
update BooksDB.Books set Books_Author="Tagore" where Books_id=5;
delete from BooksDB.Author where SI_NO=5;
--use BooksDB;
select (Books.Books_id,Books.Books_Title,Books.Books_Author,Books.Books_genre,Books.publication_year,Books.Book_price)
     from Books inner join Author on Books.Books_id=Author.SI_NO;
select * from BooksDB.Books;
select * from BooksDB.Author;
--use BooksDB;
select Books.Books_id,Books.Books_Title,Books.Books_Author,Books.Books_genre,Books.publication_year,Books.Book_price
     from Books left join Author on Books.Books_id=Author.SI_NO;
--use BooksDB;
select Books.Books_id,Books.Books_Title,Books.Books_Author,Books.Books_genre,Books.publication_year,Books.Book_price
     from Books right join Author on Books.Books_id=Author.SI_NO;
