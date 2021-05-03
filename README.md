# WordCount-using-Hadoop-MapReduce
WordCount program code using RStudio.

The WordCount.java file when executed performs MapReduce funtion on large amounts of text.




Execution:
Create a root folder (lets name it Bigdata for example)
In Bigdata folder create another src/folder
Store all the java files in the src/folder.
Create an input folder and store the input file(Sherlock.txt) in this.
Include the build.xml file in your root folder. This file is customized. You will need to update the hadoop.base.path, hadoop.version and hadoop.core.file property defined at the beginning of the file.

Open Terminal.
In the root directory.
bash:ant clean dist
Upon successful execution, it creates a dist folder in the root folder which contains the WordCount.jar file.

bash: hadoop-local jar /dist/WordCount.jar WordCount input out
If successful, it creates an out folder in the root folder.
The out folder contains 2 files. 
part-r-00000 and _SUCCESS

The output of the MapReduce program is stored in the part-r-00000.



