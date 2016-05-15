# SQLiteJDBCHW4
CSC 675 SQLite JDBC App

For	this	assignment	you	will	write	a	Java	program	that	interfaces	with	the	Chinook	database (from	HW2)
using	JDBC to	provide a simple	online	music	store. (You	may	use	Python,	Perl,	or	C++ instead	of	Java	for	
this	assignment.)
Part	1:	Recall	that	the	Chinook	database	is	an	SQLite	database,	so	you	will	need	SQLite	JDBC	Driver.	The	
latest	version	of	the	driver	can	be	downloaded	from:	https://bitbucket.org/xerial/sqlite-jdbc/downloads		
Add	the	downloaded	jar	file	to	your	class	path.
Please	refer	to	the	following	two	resources	to	see	how	to	connect	to	a	database	from	a	Java	program,	
and	how	to	query	and	update	database	objects	from	a	Java	program.
• Online	tutorial	about	connecting	to	a	SQLite	database	from	a	Java	program:	
http://www.tutorialspoint.com/sqlite/sqlite_java.htm
• Material	from	JDBCTest.java	(Note:	Python	and	Perl	examples	are	also	on	ilearn)
Note: This Java	program	connects	to	a	MySQL	database,	so	you	can’t	use	code	snippets as	is.	
Part	2:	Write	an	interactive	Java	program	(GUI	not	needed)	with the	following	functionalities.	The	
program	should	start	by	providing	the	user	with	following	5	options.
1. (25 points)	Obtain Album	title(s) based	on	Artist	name.
When	this	option	is	selected the	user	should	be	prompted	for	an	Artist	name.	The	program	
should	search	the	appropriate	table(s)	of	the	Chinook	database for	album	titles	by	this	artist.	
The	output should	consist	of	Album	title	and	Album	ID	pairs.	
The	output	may	be	empty, and	if	so	the	user	should	receive	a	message	to	that	effect.
If	there	are	multiple	artists	with	the	specified	name	then	the	results	for all	the	matching	artists
should	be	displayed separated	by	headers	containing	artist’s	ID.
		
2. (Optional)	Obtain	Track(s) of	an	Album title.
When	this	option	is	selected the	user	should	be	prompted	for	an	Album	title.	The	program	
should	search	the	appropriate	table(s) of	the	Chinook	database for	all	the	tracks	in	this	album.	
The	output should	consist	of	Track	name,	Track	ID,	Genre	name,	and	UnitPrice.	
The	output	may	be	empty	and	the	user	should	receive	a	message	to	that	effect.
If	there	are	multiple	albums with	the	specified	title then	the	results	for	all	the	matching	album	
should	be	displayed	separated	by	headers	containing	album	ID.
If the	output	is	not	empty	then	the	user	should	be	given	the	option	of	purchasing one	of	the	
listed	tracks.
If	this	option	is	selected then	prompt	the	user	for	the	ID	of	the	Track	and	the	quantity	
that	they	wish to	purchase.	
Check	if	the	entered	Track	ID	is	valid,	that	is,	has	to	be	one	of	the	Track	IDs	from	the	last	
output.
Check	if	the	quantity	is	valid	– greater	than	0.
If	the	inputs are	valid then	update	the	appropriate	tables	to	record	the	purchase.
Assume	that	the	customer	making	this	purchase	has	ID:	25	(Victor	Stevens)	
3. (25	points)	Purchase	History	for	a	Customer
When	this	option	is	selected	the	user	should	be	prompted	for	a	Customer	ID.	The	program	
should	search	the	appropriate	table(s)	of	the	Chinook	database this customer’s	purchase	
history.		The	output should	consist	of	Track	name,	Album	name,	Quantity,	and	Invoice	date	for	
the	qualifying	records.	
The	output	may	be	empty	and	the	user	should	receive	a	message	to	that	effect.
4. (25	points)	Update	Track	Price	– Individual
When	this	option	is	selected	the	user	should	be	prompted	for	a	Track ID.	The	current	unit	price
for	this	track should	be	displayed.	Then	prompt	the	user	for	the	new	price,	update	the	
appropriate	record,	and	display	the	updated	record.
5. (Optional)	Update	Track	Price	– Batch
When	this	option	is	selected	the	user	should	be	prompted	for	a	percentage	value.	The	valid	
range	for	the	user	input	is	-100%	to	100%.	The	unit	price	of	every	track	should	be	updated	
according	to	the	specified	percentage	value.	For	example,	if	the	current price	of	a	track	is	$0.99	
and	if	the	user	specifies	-30%	then	the	updated	price	of	this	track	should	be	$0.693.	Display	the	
following	information	after	the	update:	Track	ID,	Name,	Previous	Unit	price,	Updated	Unit	price.
Upload	to	ilearn	your	Java	project	containing	the	code.	
Note: Your	code	should	be	correct, complete,	and	well-documented to	receive	full	points.	
