## How to store data?

Depending on the *type* and *size* of the data there are several formats and libraries from which one can choose. Other factors such as 
 * the *fragmentation* of the information that is stored in the data 
 * the amount of *metadata* 
 * or the way we need to *access* the data (sequentially or randomly)
also matters in our choice of datastorage.

For smaller datasets (< 1 GB) all of the data can be read into the memory, so any operation on it will be cheap and the emphasis is more on the logic how the data is organized.
In case of larger datasets we need to optimize for quick accessibilty and build functions around it that will reconstruct the logical structure again.

One way to store data is to create a relational database with a database management system (DBMS) (e.g. MySQL). This has the benefit of saving space by utlizing the relations within the data and minimizing redundancy. A DBMS can also serve multiple users at the same time. Obviously DBMS won't help much if data is not related at all (e.g. in case of timeseries). 




## Topics
 1. [File formats](File_formats.md)
    * Historical overview of file formats
    * Advantages and disadvantages of various file formats
    * Algorithms for searching for data
 2. [Openscience](OS.md)
    * Version control systems
    * Publishing with code and data

3. [Handling large datasets](Large_data.md)
