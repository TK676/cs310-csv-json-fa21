# cs310-csv-json-fa21

This project was completed for my CS310 (Software Engineering 1) class. I was tasked with creating converters to translate a specific data set to and from equivalent CSV and JSON formats. I had to fork my professors repository on GitHub and work from the files of code we were given. We had conversion methods that were given to us and we had to complete them and make sure the ConverterTest.java file successfully ran all four tests.

Starting with the csvToJson converter, it first creates a CSVReader and iterator to read and iterate the CSV data to prepare it for conversion. It then creates JSON objects and arrays for the column and header data once it's converted. It adds the column header elements and then iterates through the CSV rows to convert the data. After it's all done it adds rows to the data and defines the results so that the program can output the converted data. Lastly, it returns the results so that the user can read the data and see if it correctly converted the data or not.

Moving on to the jsonToCsv converter, it is very similar in the way that it works. It starts by creating a Writer to write the data in the appropriate format and then creates a JSON Parser and parses the JSON Data. It then creates a String[] array for the column headers and then procedes to copy and write them into a JSONArray along with the row data. Lastlym it defines the results and returns them to the output for the user to read.

The ConverterTest.java file does what it says, it tests the converters to make sure that they work as intended. First it creates two private Strings; csvString and jsonString. It then creates a private JSONParser and JSONObject. After that is gets the CSV data and reads it, then goes on to convert the CSV data to a string. Then it gets the JSON data and reads it, and then it converts the data to a string as well. After all of this, it then tests the converters. It first tests converting CSV to JSON, then JSON to CSV, then JSON to CSV to JSON, and finally CSV to JSON to CSV. If it all passses, then the project works as intended.
