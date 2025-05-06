Cultural Heritage Data Management System 🏛️
This project is an academic initiative designed for managing cultural heritage data. It includes both a server and client component along with a command-based interface for searching and managing cultural heritage entries.

📋 Requirements
Java 17+

Maven 3.6+

Data file: Archeologia---Storia-e-Tradizioni---Regione-Marche.csv

All text files must be encoded in UTF-8

🚀 Installation
Clone the repository and build the project using Maven:

bash
Copy
Edit
# Clone repository
git clone https://github.com/yourusername/cultural-heritage-system.git
cd cultural-heritage-system

# Build project
mvn clean package
🖥️ Usage
Start Server
Run the server with the following command:

bash
Copy
Edit
java -jar target/heritage-server.jar
Start Client
Run the client with the following command:

bash
Copy
Edit
java -jar target/heritage-client.jar
Connection Defaults
Parameter	Value
Server Address	localhost
Port	12345

⌨️ Command Reference
Basic Commands
Command	Description
HELP	Show command reference
END	Disconnect from server

Search Operations
Search commands follow this syntax:

bash
Copy
Edit
SEARCH [OPTION] "QUERY"
Option	Search Type	Example
-n	Exact name	SEARCH -n "Castelldimezzo"
-c	Exact city	SEARCH -c Ancona
-t	Exact type	SEARCH -t Archeologia
-a	Exact address	SEARCH -a "Via Ferretti"
--n	Partial name	SEARCH --n castle
--c	Partial city	SEARCH --c piceno
--t	Partial type	SEARCH --t paesaggio
--a	Partial address	SEARCH --a piazza
-o	Opening days	SEARCH -o lunedì

📊 Data Format
The system expects data in the following format:

mathematica
Copy
Edit
ImageURL;Caption;Type;Name;City;Address;Number;Phone;Email;Website;Latitude;Longitude;OpeningHours
🛠️ Troubleshooting
Common Issues
Error	Solution
Connection failed	Verify the server is running
Invalid command format	Check the command syntax
Index out of bounds	Use a valid index (0 ≤ index < dataset size)

