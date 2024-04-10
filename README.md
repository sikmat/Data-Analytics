# DATA ANALYTICS

## WEEK 1: MODULE 1
## CH.1 DATA ANALYST

### WHAT IS DATA ANALYTICS
Responsibilities and Roles:
1. Data collection and preparation
2. Data analysis
3. Data visualization and storytelling
4. Decision support
5. Collaboration and communication
6. Continous learning and adaptation

This helps an organization make informed decisions and improve operations, drive strategies and create competitive advantage.
Must understand how to aqcuire, clean and transform data to meet organization's needs.
Create powerful visualizations to display the collected and analyzed data to decision-makers, stakeholders.

Analytics is made possible by modern DATA, STORAGE and COMPUTING capabilities, the three pillars.
- There is a huge amount of data in the world.
- The cost of storage has dropped drastically over time, making storage easily available/affordable
- Continous advancement in computing power has benefited analytics. Supercomputers needed for analytics use to be expensive and a scarce resource. Now there is enough computing power on a single laptop to perform analytics tasks.
These three trends—the massive volume of data generated by our businesses on a daily basis, the availability of inexpensive storage to retain that data, and the cloud's promise of virtually infinite computing power—come together to create fertile ground for data analytics.

### ANALYTICS PROCESS:
1. Data Acquisition
2. Cleaning and manipulation
3. Analysis
4. Visualization
5. Reporting and Communication
- The process is iterative, a set of interrelated actions that may be revisited frequently while working with a dataset. Like noticing unusual data points in a dataset and having to go back to cleaning the data and rerun analysis with the newly cleaned data, and having to return to data acqusition stage as well.

Analysis Techniques:
1. Descriptive
2. Predictive
3. Prescriptive

ML, AI and Deep Learning

Machine Learning: Uses algorithms to discover knowledge in datasets that can be applied to make informed decisions about the future. Useful in the following:

- Segmenting customers and determining the marketing messages that will appeal to different customer groups.
- Discovering anomalies in system and application logs that may be indicative of a cybersecurity incident.
- Forecasting product sales based on market and environmental conditions.
- Recommending the next movie that a customer might wish to watch based on their past activity and the preferences of similar customers.
- Setting prices for hotel rooms far in advance based on forecasted demand

Artificial Intelligence 
- Techniques used to get a computer to imitate human behavior, to try and behave as if they are intelligent.

Machine Learning 
- Is also a subset of AI techniques, attempting to apply statistics to data problems in an effort to discover new knowledge. It is AI techniques designed to learn.

Deep Learning
- Is a further subdivision of ML that uses complex techniques, known as neural networks, to discover knowledge in a particular way. It is a highly specialized field of ML, mostly used for image, video and sound analysis

### DATA GOVERNANCE
- Ensures that an organization has high-quality data and is able to effectively control that data. Using Master Data Management programs to maintain and improve the quality of the data.

Analytics Tool
- Automate much of the heavy workload of analysis, improving the analyst's ability to acquire, clean, manipulate, visualizer and analyze data. As well as assistance in reporting and communicating results. Examples of these tools are Excel spreadsheet, Google sheets.

## CH.2 UNDERSTANDING DATA
### DATA TYPES
- A data element is an attribute about a person, place, or thing containing data within a range of values. Data elements also describe characteristics of activities, including orders, transactions, and events.

A data type limits the values a data element can have
- Individual data types support structured, unstructured, and semi-structured data

Tabular Data
- Tabular data is data organized into a table, made up of columns and rows. A table represents information about a single topic. Each column represents a uniquely named field within a table, also called a variable, about a single characteristic.
- The contents of each column contain values for the data element as defined by the column header.
- It is helpful to think of tabular data as rectangular data. It is easy to draw a rectangle around the data. The top of the rectangle is defined by columns, while rows define the left side of the rectangle.
- Spreadsheets, including Microsoft Excel, Google Sheets, and Apple Numbers, are practical tools for representing tabular data. A relational database management system (RDMS), commonly called a database, extends the tabular model. Instead of having all data in a single table, a database organizes related data across multiple tables. The connection between tables is known as a relationship. Oracle, Microsoft SQL Server, MySQL, and PostgreSQL are examples of database software. Tabular data is the concept that underpins both spreadsheets and relational databases.

### STRUCTURED DATA TYPES
- Structured data is tabular in nature and organized into rows and columns. Think of a spreadsheet for example. With clearly defined column headings, spreadsheets are easy to work with and understand.

Character
- Limits data entry to only valid characters.
- Characters can include the alphabet that you might see on your keyboard, as well as numbers.
- Depending on your needs, multiple data types are available that can enforce character limits.

Alphanumeric 
- Most widely used data type for storing character-based data.
- As the name implies, alphanumeric is appropriate when a data element consists of both numbers and letters.
- The alphanumeric data type is ideal for storing product stock-keeping units (SKUs). It is common in the retail clothing space to have a unique SKU for each item available for sale. If you sell jeans, you may stock products from Armani Jeans, Diesel, Lee Jeans, Levi's, and Wrangler. To keep track of all the manufacturer, size, color, and fit combinations in your inventory. Tracking inventory at the SKU level allows you to manage availability in your online and in-store systems, all courtesy of the alphanumeric data type.

Text
- There are times when it is necessary to impose even stricter limits on character-related data to exclude numbers. Excluding numbers can be achieved using the text data type.
- Closely related to the alphanumeric data type, but more stringent. It is helpful to think of text as a subset of alphanumeric, only allowing the storage of alphabetic characters.
- Improves the overall data quality. For example, consider the “State” data element in Figure 2.1. If the system contains state names from the United States, it would be appropriate to select a text data type.

- Consider a data entry example. Suppose you operate an online retail system. To deliver orders, you need address information for the intended recipients. This information comes from the customers themselves since they can specify where orders should be shipped. Any time a person interacts with a computer, there is the potential for a data entry error. Suppose someone wanted to enter “Montana” for the state component of their address.

Take a look at the positioning of the O and 0 keys in Figure 2.3, depicting the U.S. QWERTY keyboard layout. These two keys are very close together. Many people press these keys with the fourth finger of their right hand, making a data entry error that much more likely. A person could supply the value “M0ntana” instead of the intended “Montana.” With “State” as a text data type, trying to input the erroneous value would result in an error. However, with “State” implemented as alphanumeric, nothing would prevent that mistake from making its way into the database.

Each database software has its unique method of implementing character data types to handle the nuances related to character data. The most significant difference has to do with how much data a particular data element can contain. Table 2.2(LMS) shows a sampling of how the three most popular databases provide data types for character data.

All of the data types shown in Table 2.2(LMS) support alphanumeric data. Where they differ is in how much data they can handle. 
- Before defining a column as alphanumeric, you need to determine how long your longest-possible text value will be.
- You also need to realize that while data types may have the same names, they are implemented differently by software vendors. There are also individual data types, like CLOB and LONGTEXT, that are vendor-specific.
- Finally, you need to be aware of the absolute limits imposed by the database you are using.

- With spreadsheets, configuring a given cell or range of cells as a text-only data type takes more effort than when using a database. It is not possible to accomplish this with one of the native data types provided by the software. Instead, limiting it to just text requires a formula. Suppose a person tries to input a value containing numbers or symbols into a cell where the formula is active. 

Character Sets
- When considering alphanumeric and text data types, you need to think about the character set you are using to input and store data when using a database. Databases use character sets to map, or encode, data and store it digitally. The ASCII encoding standard is based on the U.S. English alphabet. ASCII accommodates both the upper and lowercase English alphabet and numbers, mathematical operators, and symbols.
- Many languages include accent marks, extending the Latin alphabet. For example, Akrapovič is a Slovenian manufacturer. To store the č in Akrapovič, you need to encode that value appropriately. In addition, there are many languages, including Arabic, Chinese, Japanese, and Korean, which use symbols as opposed to extending the Latin alphabet. For example, the Arabic word for “cat.” Several encoding standards exist that accommodate non-Latin characters. One of the most common is Unicode Transformation Format-8 (UTF-8), which allows non-Latin characters to be input by a user and stored in a file or database.
- It is necessary to realize that individual characters may consume multiple bytes, impacting the length of a character string you can store in a character data type.

Numeric
- Exclusively numbers making up the values of a data attribute, integer and numeric data types used in databases
  
Whole Numbers
- Integer and all its subtypes are for storing whole numbers. Value ranges for smallint and shortinteger are the same. Same for int and integer, as well as bigint and longinteger. different names, but same functionality.
  
Rational Numbers??? (LMS EXPLANATION NOT ENOUGH)
- In all its variants, the numeric data type is for rational numbers that include a decimal point.
- Each DB vendor has different implementation on how they support rational numbers.
- There is a data type called numeric in both SQL Server and MySQL that is functionally equivalent to the decimal type.
- Data types are incosistently named across databases, you must consider the ultimate range of values a given data element handles.
  
Date and Time
- DBs have various data types for handling date- and time related info, depending on the data you need to store pertaining to time, date or both.
  
Currency
- To display the stored value as a currency you must apply data formatting so it displays as required for the specific purpose. Data formatting is common with currency and dates data types.
- Microsoft SQL Server DB has data types specifically for storing currency.
- It is better to use numeric data type to store currency related data, to avoid rounding errors. Limiting a calculation to four digits of precision after the deicmal point can lead to rounding errors.

You should recognize the difference between storing a data type and formatting it to facilitate human interpretation. Take care not to automatically infer a data type based on formatting.

Strong And Weak Typing
Data types define values placed in columns. 
- Strong typing is when technology rigidly enforces data types. Databases, discussed in Chapter 3, use strong typing. A database column defined as numeric only accepts numerical values. You will get an error if you attempt to enter characters into a numeric column.
- Weak typing loosely enforces data types. Spreadsheets use weak typing to help make it easier for people to accomplish their work. Spreadsheets default to an “automatic” data type and accommodate practically any value. When a person specifies a data type, it is loosely enforced compared to a database. For example, with a numeric spreadsheet cell, the software does not stop you from entering and storing characters.

### UNSTRUCTURED DATA TYPES
- Any data that does not fit neatly into the tabular model. Ex: Digital images, Audio, Video, Open-ended survey responses.
- Analyzing unstructured data gives a lot of insight and useful information, better understanding.

Binary
- Common for storing unstructured data, supports any type of file.
- When choosing which binary type to use, size tends to be the limoiting factor. You must select data type that is as large as the largest file you plan to store.
- Most common types of unstructured data are audio, image and video data.
- Spreadsheets are designed to manage highly structured data, but are not good at storing binary data, which is unstructured. Google sheets does allow storing of binary data within a cell, excel is not good at it.
- DBs are better equiped and sophisticated enough to handle a collection of data types for storing binary data.

Audio
- Recording/Capturing, (digitizing ), storing, and analyzing audio data leads to better decision-making and responsiveness in the real world.
- Audio in its raw form takes up more storage space, its better encode it with a compression algoritm to reduce the space it uses.
- Storing audio requires a data type designed to handle raw binary data.
- Quality of the audio affects the file size, hence more storage required.

Images
- AI alogorithms for image processing over a set of digital photos allow us to be able search and find specific objects in an image, or an image containing that object. Used for X-rays, Insurance.
- Image Resolution is an important factor, that governs the size of the image file and how much space is required to store it. Images of higher quality, more detail and greater resolution will need more storage space.
- Images can also be compressed to take up less space.
- Storing in a DB needs a data type designed to handle raw binary data, like varbinary or BLOB.

Video
- Image processing algorithms are also applied on videos..
- Resolution, Length/Duration of the video also affect the size of the file and storage

Large Text
- Their data type names differ among DB vendors
- Oracle has varchar/varchar2 text data type, that is limited to 4000 bytes. But has the CLOB proprietary data type, which supports up to 128TB of text data.
- Microsoft implements varchar differently, supporting up to 2GB

### CATEGORIES OF DATA
- Not all data can be categorized as structured or unstructured, as a result semi-structured data represents the space between the two. Semi represents the space between structured spreadsheets and unstructured videos.

Quantitative vs Qualitative Data
- Data is either qualitative or quantitative
- Quantitative consists of numeric values, like counting or measuring values. Answers questions like "How many?" and "How much?".
- Qualitative Consists of frequent text values. From data elements whose values describe characteristics, traits and attitudes. Ex: Pet Name, Animal Type, Breed name. Answers questions like, "Why?" and "What?"

Discrete vs Continous Data
- Numeric data comes in two different forms: discrete and continous.
Discrete data represents measurements that can't be subdivided.
- For example, if a fundraising organization sells chickens in half-chicken increments, you can buy 1.5 chickens. However, you can't buy .25 chickens.
- Another way to think about it is that discrete data is useful when you have things you want to count. For example, a veterinary clinic may be interested in the number of dogs and cats under its care. Figure 2.16 shows the aggregation of the pet from Table 2.1. The Total data element is an example of discrete data, as it contains the value 5 for Dog and 1 for Cat. A veterinary practice would not care for 5.5 dogs or 2.25 cats.
Instead of counting, when you measure things like height and weight, you are collecting continuous data.
- While whole numbers represent discrete data, continuous data typically need a decimal point. Two dogs in Table 2.1 have their height recorded to the tenth of an inch. Similarly, weight is recorded to the tenth of an inch for three dogs and one cat. Figure 2.17 shows the continuous measure of average height and weight information by animal.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/39c3e1a7-1971-477a-965b-8474b94273ad)

Qualitative data is discrete, but quantitative data can be either discrete or continuous data. For example, age is a continuous variable, but you may treat a person's age in years as discrete. A good rule of thumb is that discrete applies when counting while continuous applies when measuring.

Categorical Data
- Text data with a known, finite number of categories is categorical. When considering an individual data element, it is possible to determine whether or not it is categorical. Animal Type is a good example of categorical data. As represented, this column separates the data into two categories: dog and cat. As additional dogs or cats enter into care, they fall within the existing categories. That said, the range of accepted values for a given category can change over time. You can also use categories to enforce data validation when someone is first entering data.
- Category enforcement has the effect of improving data quality. For example, suppose the veterinarian decides to only care for cats and dogs. To streamline operations, the veterinarian has a website built so that clients can schedule appointments online. Suppose the intent is to limit online appointments only for dogs and cats. In that case, the website can implement a drop-down menu where the only options for the animal type are “dog” and “cat.” If someone had a mouse, hamster, or gerbil, the validation check prevents the scheduling of an appointment.

Dimensional Data
- Dimensional modeling is an approach to arranging data to facilitate analysis.
- Dimensional modeling organizes data into fact tables and dimension tables.
- Fact tables store measurement data that is of interest to a business. A veterinary practice may want to answer some questions about appointments. A table holding appointment data would be called a fact table. Dimensions are tables that contain data about the fact. For appointment data, the veterinarian's office manager may want to understand who was at an appointment and if any procedures were performed. In Figure 2.18, the Appointments table is the fact table. The Veterinarians, Owners, Procedures, and Pets tables are all dimensions that can answer questions about appointments.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/7d898361-c749-4de6-b870-64de006951bc)

- Dimensional data contains groupings of individual attributes about a given subject. For example, taken as a whole, the pets dataset from Table 2.1 can be called the “pets” dimension. You can imagine that the “owners” dimension in Figure 2.18 contains biographic information about a pet's owner, identifying who was present at an appointment. When combined with data from additional dimensions, data elements from each dimension add detail about the facts in the fact table.

### COMMON DATA STRUCTURES
In order to facilitate analysis, data needs to be stored in a consistent, organized manner.
It is common to use multiple tools to analyze data. Improved integration and interoperability between tools make it easier for analysts to be productive. As a result, several concepts have become standardized.

Structured Data
- Tabular data is structured data, with values stored in a consistent, defined manner, organized into columns and rows.
- Data is consistent when all entries in a column contain the same type of value. This method of organization facilitates aggregation. For example, you can add each attribute value in the column to get the total of all entities. Structured data also makes summarization easy, since you can compute an average of a value of the entities. It is common to perform summarization across groups.

- However, structured data does not translate directly to data quality. For example, suppose a new dog named Thor became a patient. When Thor's data was input into the system, a person transposed the Pet Name and Animal Type values, as highlighted in table below. 

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/542fbed9-c8c1-42ea-85ce-d3f37f6b1077)

- Since both Pet Name and Animal Type are character data types, nothing from a structural standpoint prevents this mistake. However, if you were to perform the same summarization as in Figure 2.16, the result would be what is represented by Figure 2.20. A person looking at the summary in Figure 2.20 would immediately know that something is amiss from a data quality standpoint, as “Thor” is not a type of animal.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/5c96a99a-97f9-4c69-a681-9547768cc115)

 - It is a best practice to specify a key that uniquely identifies all values for a given row.
 - In Figure 2.19, no column enforces uniqueness across rows. Consider this possible, though unlikely, scenario: a Labradoodle named Hazel, born on 7/3/2016, measuring 23 inches tall and weighing 61 pounds, becomes a new patient.
 - Since all of her information is identical to an existing animal, nothing in the structure exists to differentiate the two. Figure 2.21 illustrates how to address this storage issue.
 - The Pet ID column has a data type of integer and contains a unique number for each row.
 - With Pet ID as the key, we can differentiate between the Hazel in rows 3 and 8.

Unstructured Data
- Unstructured data is qualitative, describing the characteristics of an event or an object.
- Images, phrases, audio or video recordings, and descriptive text are all examples of unstructured data.
- There is very little that is common about different kinds of unstructured data.
- Since the data is highly variable, its organizational and storage needs are different from structured data.
- Unstructured data also represents a significant opportunity. A Forbes study shows that over 90 percent of businesses need to manage and derive value from unstructured data.

**Machine data** is a common source of unstructured data. 
- Machine data has various sources, including Internet of Things devices, smartphones, tablets, personal computers, and servers. 
- As machines operate, they create digital footprints of their activity.
- This data is unstructured and can identify machine-to-machine interaction. Although some may think of machine data as digital exhaust, it is a treasure trove just waiting to be exploited by organizations.

A wide variety of technologies has emerged to facilitate the storage of unstructured data. Operationally, these technologies are similar to how a key in a tabular dataset identifies its associated values. With unstructured data, the key is a unique identifier, whereas the value is the unstructured data itself.

Consider the log entry shown in Figure 2.22. As an example of machine data, it represents a single entry within a log file generated when accessing a specific image on the Internet. The log entry contains a mix of seemingly random strings, time stamps, IP addresses, URLs, and browser metadata.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/2e903f83-2138-4de0-acdd-6c002bb60627)

**Object storage** facilitates the storage of unstructured data. The key-value concept underpins the design of object storage. The key is a unique identifier, and the value is the unstructured data itself. In Figure 2.23, the key is the filename, and the value is the contents of the file itself. Note that in this figure, each file is of a different type. The word document.docx is a Microsoft Word file, textfile.txt contains plain-text data, and the png image.png and lp_image-8.jpeg objects are digital images.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/2573a4db-3e27-4516-b6f4-1c3865c594a1)

**Semi-Structured Data**
- Semi-structured data is data that has structure and that is not tabular. Email is a well-known example of semi-structured data.
- Every email message has structural components, including recipient, sender, subject, date, and time.
- However, the body of an email is unstructured text, while attachments could be anything type of file.

The need to make semi-structured data easier to work with has led to the emergence of semi-structured formatting options. These formatting options use separators or tags to provide some context around a data element.

### COMMON FILE FORMATS
Common file formats facilitate data exchange and interoperability. You need to recognize the formats and be familiar with their use cases.

**Text Files**
- Consist of plain text, limited to in scope to alphanumeric data.
- They are popular due to their compatibility with any OS without the need for proprietary software.
- When machines generate code, it is commonly stored in a textfile.
- A delimiter is used to facilitate the transmission of structured data via a textfile. The delimiter separates indiviual fields, such as comma or a tab.
- Delimited files are commonly CSV, delimited witha comma and another delimited file is TSV(Tab)
- Structured data fits well into CSV files, a popular format for exchanging data via files.

**Fixed-Width Files**
- Before delimited files were more commonly used, flat-files were fixed width.
- But fixed-width files require too much to be created, needing some extra steps. You must pad values that are shorter and for numbers by prepending a leading zero. For alphanumerics or text fields you use space.

**Javascript Object Notation(JSON)**
- Designed to add structure to a file format without incurring significant overhead
- Easily readable and easily parsed by modern languages.
- Lightweight and becoming the popular choice for AJAX techniques, for interaction between web browser and a remote server.
- Better option when you need to incorporate additional metadata or represent a complex data structure, or XML

**Extensible Markup Language(XML)**
- Markup language that facilitates structuring of data in a text file.
- Incurs more overhead than JSON because of extensive use of tags. Tags describe a data element and enclose each value for each element.
- XML file is almost double the size of JSON and that can be massive for data in Gigs and Terras

**HyperText Markup Language(HTML)**
- Markup language for documents designed to be displayed in a web browser. Also tag based.
- HTML pages are the foundation for interacting with the world wide web.

## 5 POINT SUMMARY
### 1. Consider the values of what you will store before selecting data types
Data types are used to store different kinds of values. When dealing with numeric information, the best option is a numeric data type that can accommodate decimals. For sequences of whole numbers, an integer data type is a good choice. Be wary of using currency-specific data types—that can lead to calculation errors. For text values, the alphanumeric data type is the optimal choice. When dealing with dates, you will want to consider whether you need to store the time as well. For binary data, including audio, video, and images, you should use a BLOB data type.

### 2. You can format data after storing it
While data types determine how data gets stored, formatting data governs how data will be displayed to a person. You may wish to store numeric data to many decimal places but round to the hundredths for display purposes. Similarly, numeric data can be formatted and displayed as a currency. Dates are possibly the most commonly formatted data type, since the same information may need to be displayed differently depending on cultural norms.

### 3. Consider the absolute limits of values that you will store before selecting data types
When selecting data types, consider the range of values that a data element can contain. Suppose the values need to fall within a given, defined range. In that case, you must select a data element that can support discrete data. If the data element's range is unknown, a data element that supports continuous data is necessary.

### 4. Difference between structured and unstructured data
Individual data elements fall along the structured data continuum. At one end, there is highly structured, rectangular data. Structured data is organized into columns and rows. Each column has a consistent data type, and each row contains data about one data subject. Unstructured data does not fit neatly into a column. Looking for similarities or differences in unstructured data requires more advanced analytical techniques than structured data.

### 5. Differences in common file formats
Common file formats make it easy for people to read a file's contents and facilitate interoperability between tools. Delimiters separate variable-length fields in a file. The comma and the resultant CSV file are among the most commonly used formats for exchanging text files. To provide additional metadata about data values and support more complex data structures, XML and JSON were developed. JSON is a preferred format, given its low overhead, especially when compared with XML.\

# MODULE 2
## CH.3 UNDERSTANDING DATABASES AND DATA ACQUISITION

### Exploring DBs

**Relational DB**
- Mainly for storing and processing structured data
- Deals with tabular data as tabular data is highly structured
- In F.Codds's relational model an entity(Nouns= People, Places, Things) contains data about a single object.
- Benefits: Consistencey with option to rollback, Stored procedures(Ability to write multiple blocks of functions of code that you can reuse), Locking and Concurrency

**Entity Relationship Diagram(ERD)**
- Is visual artifact of the data modelling process. It shows the connection/relationship between related entities.
- Serves as a blueprint for, and helps you understand the structure of relational DB
- Helps you visualize the connections, especially when dealing with muliple tables.
  
- **Cardinaity**  is the relationship between two entities, showing how many instances of one entity relate to instance of another entity. We use cardinality symbols, with different line endings to illustrate these relationship combinations.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/592b5732-ad12-4ba6-a569-c09fc03ceb6c)


- **Unary relationship** is when an entity has a relationship with itself.

![image](https://github.com/sikmat/Data-Analytics/assets/111583727/8fe22088-5895-4c52-99b8-de973b9587f5)

- **Binary relationship** connects two entities. Most common and easy to explore.
- **Ternary** connects three entities. For example a ticket entity could connect a venue, performing artist, and a price. More complex and rare.

Relational DBs are pieces of software that let you make an operational system out of an ERD. You start with a relational model and create a physical design. Relational entities correspond to DB tables, and entity attributes correspond to table columns. When an attribute becomes a column you assign it a data type. The result of all this is schema diagram, it's like an ERD with the additional details needed to create a database.

Two entities can become three tablea, by creating an a third table to resolve a many-to-many relationship with an associative table.
- An **Associative** table is both a table and a relationship.
- **Primary key(PK)** is one or more attributes that uniquely identify a specific row. Best to use -- - **Synthetic primary keys** which are attributes whose only purpose is to contain unique values for each row.
- **Foreign key(FK)** is one or more columns in one table that points to corresponding columns in a related table. Frequently it references another table's PK. It is used to link two tables.
Every row in a RDB must be unique

- In DBs we use Structured Query Language(SQL) to compose queries that will perfom specific CRUD functions on a DB.
- A DB join is performed to retrieve data to use, using data values from one table to retrieve associated data in another table, typically using a FK.
- FKs enforce referential integrity, or data consistency and hence data quality.
- **Composite PK** is a PK composed of more than one column
-**Database Admin(DBA)** is someone highly skilled and knowledgeable on how DB software interact with hardware. They look at how it uses storage, memory and processor resources assigned to the DB. Trying to find processes that slow the DB down, in order to find solutions and improve performance.

**Non-Relational DB**
- Deals with unstructured data
