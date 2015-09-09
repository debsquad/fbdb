fbdb


fbdb is a little tool to handle a database of books watched, or ToRead
It requires sqlalchemy, and requests ; prettytables is optionnal

It records :
Title of the book | Autor |  date_of_beginning | date_of_end_reading | note you give | comments | date_of_insert_in_database | Read or Not

you need to inform in your ~/.database_rc_file (adjust in fbdb this name) :

//
[fbdb]
url = sqlite:///path/to/sqlite_fmdb.sql   # or whatever sql db you'd like
//

add a book to database :
fbdb add -t "title [-d YYYYmmdd] [-n x.x] [-c ""]
	-t : title of the book
	-a : autor
	-d : date of beginning
	-e : end of reading
	-n : note, on a scale from 0 to 10
	-c : comments
	-R : Read
	-N : Not read   (default : book read)

author: Franck Labadille
