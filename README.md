CSV Read Write

C# Developer find difficulties in writting and reading csv file.

The code here how you can serialize object to CSV and vice versa.

Here are step to Write Object CSV file.

Pre Requisite : CSV file Headings should match to propery of type

To Read CSV File

Step 1: Install Nuget Package using following command

Install-Package CSVReadWrite -Version 1.0.0

Step 2: Create Instance of CSVReader Class

ICSVReader reader = new CSVReader();  

Step 3: Call read method ICSVReader, to Read Method you should have following parameter filepath and encoding type.

There two overloaded method one is taking file path other is taking file stream.

reader.Read<Employee>("Filepath", Encoding.UTF8);
reader.Read<Employee>(FileStream, Encoding.UTF8);
  
This Read function will read CSV file and return the list of type.



  










