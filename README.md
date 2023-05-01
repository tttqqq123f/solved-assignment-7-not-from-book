Download Link: https://assignmentchef.com/product/solved-assignment-7-not-from-book
<br>
The purpose of this assignment is to provide you with experience in creating C++ applications that perform file I-O operations. This problem is not from the book.

Develop a class called <strong>instructor_file_processor. </strong>This class read a file and displays the contents of the file. The tester program will create 3 instances of the object to display contents of the following 3 files:




<table width="624">

 <tbody>

  <tr>

   <td width="208"><strong>file_MayaTolappa.txt</strong></td>

   <td width="208"><strong>file_AmyChaaban.txt</strong></td>

   <td width="208"><strong>file_TimMoriarty.txt</strong></td>

  </tr>

  <tr>

   <td width="208">Maya-TolappaCIS115CIS120CIS130CIS101</td>

   <td width="208">Amy-ChaabanCIS110CIS185WEB110WEB230WEB230WEB255</td>

   <td width="208">Tim-MoriartyCIS115CIS136CIS150CIS250CIS296</td>

  </tr>

 </tbody>

</table>




The UML diagram of the class is as follows:

<strong>Constructor function:</strong>

The class constructor takes in the name of the file to be processed and stored it in the class private variable

<strong>print function</strong>

In the print function, the file is opened and the first record read from the file and printed out. The remaining records from the file are read and printed out. A running counter of number of records read is maintained and printed out after the file has been processed.

The pseudo-code for the constructor is shown above. (it is not complete. I have provided ideas on how the constructor is to be implemented)

<strong>Other functions:</strong>

I have chosen not to implement accessor and mutator function in order to keep the class simple.

Implement the class in 2 files. This will result in your solution containing 3 files – class .h, class .cpp and class tester cpp file. Use my class tester file. The solution looks like this:

asn7_class_tester.cpp file

#include &lt;iostream&gt;<strong>using</strong> namespace std;#include “instructor_file_processor.h”

<strong>int</strong> main(){instructor_file_processor inst_maya(“file_MayaTolappa.txt”);instructor_file_processor inst_amy(“file_AmyChaaban.txt”);instructor_file_processor inst_tim(“file_TimMoriarty.txt”);

inst_maya.print();inst_amy.print();inst_tim.print();

<strong>return</strong> 0;}

Output from my implementation of the assignment

<table width="624">

 <tbody>

  <tr>

   <td width="624">Name of datafile    : file_MayaTolappa.txtName of Instructor  : Maya-Tolappa1.      CIS1152.      CIS1203.      CIS1304.      CIS101# of classes taught : 4——————————– Name of datafile    : file_AmyChaaban.txtName of Instructor  : Amy-Chaaban1.      CIS1102.      CIS1853.      WEB1104.      WEB2305.      WEB2306.      WEB255# of classes taught : 6——————————– Name of datafile    : file_TimMoriarty.txtName of Instructor  : Tim-Moriarty1.      CIS1152.      CIS1363.      CIS1504.      CIS2505.      CIS296# of classes taught : 5——————————– Press any key to continue . . .</td>

  </tr>

 </tbody>

</table>




<h1>Submit Instructions</h1>

When developing the assignment  program, please refer to the programming standards document. The link to this file is as follows:

<ul>

 <li><a href="https://docs.google.com/document/d/17YhQo1bbmfAS08Dvnwe6p5WcE7Dj9f1Ef1RbuDecsds/edit?usp=sharing">Programming Standards Document</a></li>

</ul>




Your program should form to the rules specified in Sections I, II , III and IV. Failure to do so will result in 0 points for the assignment. Rather than create function names with <strong>get</strong> as the start phrase, use the function names suggested by the problem specs.




Turn in one of the following via BlackBoard’s submission tool.

<ul>

 <li>Zip file with the assignment .h and .cpp files</li>

 <li>Zipped version of the solution folder created by Visual Studio</li>

</ul>




<h1>Sample program for this week</h1>

<strong>Sample programs do not have to be turned in for points. However, it is a good idea to key them and see if they work correctly.</strong>




The sample program for the week is a combination of the following programs written as 1 program with 3 functions:

<ul>

 <li>Problem #1, page 911</li>

 <li>Problem #2, page 911</li>

 <li>Problem #4, page 911.</li>

</ul>




Problem descriptions are as follows:




<table width="624">

 <tbody>

  <tr>

   <td width="624"><strong>1. File Previewer</strong>Write a program that asks the user for the name of a text file. The program should display the first 10 lines of the file on the screen. If the file has fewer than 10 lines, the entire file should be displayed along with a message indicating the entire file has been displayed. <strong>2. File Display Program</strong>Write a program that asks the user for the name of a file. The program should display the contents of the file on the screen. If the file’s contents won’t fit on a single screen, the program should display <span style="text-decoration: line-through;">24 </span><strong>19 </strong>lines of output at a time, and then pause. Each time the program pauses, it should wait for the user to type a key before the next <span style="text-decoration: line-through;">24 </span><strong>19 </strong>lines are displayed. <strong>4. Tail of a File</strong>Write a program that asks the user for the name of a text file. The program should display the last 10 lines of the file on the screen (the “tail” of the file). If the file has less than 10 lines, the entire file is displayed, with a message that the entire file has been displayed. <span style="text-decoration: line-through;">The program should do this by seeking to the end of the file and then backing up to the tenth line from the end</span>.</td>

  </tr>

 </tbody>

</table>




Additional Specifications

<ul>

 <li>Implement the solution in a class called week7_sample_FileReader.</li>

 <li>This class takes in the name of a text file via its constructor</li>

 <li>It provides methods to perform file display operations</li>

</ul>




The UML diagram for this class is shown below.

<h2>Files used to test week7_sample_FileReader</h2>

I used 2 files to test the week7_sample_FileReader class. These are shown below, in rather small text. Download these from BlackBoard if you wish to work on the sample program. The content was taken from http://en.wikipedia.org/wiki/Programming_language. The current contents of the website are different from the content in the following files.

<table width="681">

 <tbody>

  <tr>

   <td width="328"><strong>week7_sample_program_long.txt</strong></td>

   <td width="353"><strong>week7_sample_program_short.txt</strong></td>

  </tr>

  <tr>

   <td width="328">A programming language is an artificial language designedto communicate instructions to a machine, particularlya computer. Programming languages can be used to createprograms that control the behavior of a machine and/or toexpress algorithms precisely.The earliest programming languages predate the inventionof the computer, and were used to direct the behavior ofmachines such as Jacquard looms and player pianos.Thousands of different programming languages have beencreated, mainly in the computer field, with many beingcreated every year. Most programming languages describecomputation in an imperative style, i.e., as a sequenceof commands, although some languages, such as those thatsupport functional programming or logic programming, usealternative forms of description.The description of a programming language is usually splitinto the two components of syntax (form) and semantics (meaning).Some languages are defined by a specification document (for example,the C programming language is specified by an ISO Standard),while other languages, such as Perl 5 and earlier, have adominant implementation that is used as a reference.The term computer language is sometimes used interchangeablywith programming language.However, the usage of bothterms varies among authors, including the exact scope of each.One usage describes programming languages as a subsetof computer languages.</td>

   <td width="353">This introductory course in C++ programming includes object-oriented,event-driven, interactive programming techniques. Topics includedata types, pointers, arrays, stacks, recursion, string processing,searching and sorting algorithms, classes and objects, referencesand memory addresses, scope, streams and files, and graphics. A widevariety of business-oriented problems are solved by writing C++ programs.  </td>

  </tr>

 </tbody>

</table>

<h2></h2>

<h2>week7_sample_FileReader.h</h2>

#pragma once#include &lt;iostream&gt;#include &lt;fstream&gt;#include &lt;iomanip&gt;#include &lt;string&gt;

using namespace std;class week7_sample_FileReader{private:string filename;int numrecords;

public:week7_sample_FileReader(string _filename);void displayFirst10records();void displayLast10records();void displayAllRecords();};

<h2></h2>

<h2>week7_sample_FileReader.cpp</h2>




#include “week7_sample_FileReader.h”

week7_sample_FileReader::week7_sample_FileReader(string _name){numrecords = 0;string oneRec;filename = _name;ifstream ifile(_name);

if(!ifile){cout &lt;&lt; “File open failed..program terminating..
”;system(“pause”);exit(0);}getline(ifile, oneRec);while (!ifile.eof()){numrecords++;getline(ifile, oneRec);}ifile.close();}

void week7_sample_FileReader::displayFirst10records(){ifstream ifile(filename);int recnum = 0;string arec;cout &lt;&lt; filename &lt;&lt; ” has ” &lt;&lt; numrecords &lt;&lt; ” records 
”;cout &lt;&lt;“
” &lt;&lt; filename &lt;&lt; ” ——- First 10 records in file —–

”;

getline(ifile, arec);

while (!ifile.eof() &amp;&amp; recnum &lt; 10){cout &lt;&lt; arec &lt;&lt; endl;getline(ifile, arec);recnum++;}cout &lt;&lt; “
———————————

”;}

void week7_sample_FileReader::displayLast10records(){ifstream ifile(filename);int recToSkip;string arec;

if(numrecords &lt; 10){recToSkip = 0;getline(ifile, arec);}elserecToSkip = numrecords – 9;

cout &lt;&lt; filename &lt;&lt; ” has ” &lt;&lt; numrecords &lt;&lt; ” records 
”;cout  &lt;&lt;“
” &lt;&lt; filename &lt;&lt; “—- Last 10 records in file —–

”;for(int i=0; i &lt; recToSkip; i++){getline(ifile, arec);}

while(!ifile.eof()){cout &lt;&lt; arec &lt;&lt; endl;getline(ifile, arec);}ifile.close();cout &lt;&lt; “
—————————————–

”;}

void week7_sample_FileReader::displayAllRecords(){ifstream ifile(filename);int lines=0;string arec;

cout &lt;&lt; filename &lt;&lt; ” has ” &lt;&lt; numrecords &lt;&lt; ” records 
”;cout &lt;&lt;“
” &lt;&lt; filename &lt;&lt; “——- All records in file ———–

”;

getline(ifile, arec);while (!ifile.eof()){if(lines &gt;= 19){cout &lt;&lt; endl;system(“pause”);lines=0;}cout &lt;&lt; arec &lt;&lt; endl;lines++;getline(ifile, arec);}

cout &lt;&lt; “
—————————————–

”;ifile.close();}




<h2>mtolappa_week7_sample_tester.cpp</h2>

#include &lt;iostream&gt;#include &lt;iomanip&gt;#include &lt;fstream&gt;#include &lt;string&gt;using namespace std;#include “week7_sample_FileReader.h”

void display_file(string fname);int main(){display_file(“week7_sample_program_long.txt”);display_file(“week7_sample_program_short.txt”);

return 0;}

void display_file(string fname){week7_sample_FileReader myfile(fname);

myfile.displayFirst10records();

cout &lt;&lt; “Press any key to continue..
”;cin.get();

myfile.displayLast10records();

cout &lt;&lt; “Press any key to continue..
”;cin.get();

myfile.displayAllRecords();

cout &lt;&lt; “Press any key to continue..
”;cin.get();}

<h2></h2>

<h2></h2>

<h2>Output from Sample program execution</h2>

The output is shown below. Places where I pressed the enter key upon receiving the “Press any key to continue..” message are shown in blue.




When processing the week7_sample_program_long.txt file, the screen pauses after every 19 records, allowing the user to view the screen before proceeding.




week7_sample_program_long.txt has 26 records




week7_sample_program_long.txt ——- First 10 records in file —–




A programming language is an artificial language designed

to communicate instructions to a machine, particularly

a computer. Programming languages can be used to create

programs that control the behavior of a machine and/or to

express algorithms precisely.

The earliest programming languages predate the invention

of the computer, and were used to direct the behavior of

machines such as Jacquard looms and player pianos.

Thousands of different programming languages have been

created, mainly in the computer field, with many being




———————————




<strong>Press any key to continue..</strong>




week7_sample_program_long.txt has 26 records




week7_sample_program_long.txt—- Last 10 records in file —–




into the two components of syntax (form) and semantics (meaning).

Some languages are defined by a specification document (for example,

the C programming language is specified by an ISO Standard),

while other languages, such as Perl 5 and earlier, have a

dominant implementation that is used as a reference.

The term computer language is sometimes used interchangeably

with programming language.However, the usage of both

terms varies among authors, including the exact scope of each.

One usage describes programming languages as a subset

of computer languages.




—————————————–




<strong>Press any key to continue..</strong>




week7_sample_program_long.txt has 26 records




week7_sample_program_long.txt——- All records in file ———–




A programming language is an artificial language designed

to communicate instructions to a machine, particularly

a computer. Programming languages can be used to create

programs that control the behavior of a machine and/or to

express algorithms precisely.

The earliest programming languages predate the invention

of the computer, and were used to direct the behavior of

machines such as Jacquard looms and player pianos.

Thousands of different programming languages have been

created, mainly in the computer field, with many being

created every year. Most programming languages describe

computation in an imperative style, i.e., as a sequence

of commands, although some languages, such as those that

support functional programming or logic programming, use

alternative forms of description.

The description of a programming language is usually split

into the two components of syntax (form) and semantics (meaning).

Some languages are defined by a specification document (for example,

the C programming language is specified by an ISO Standard),




<strong>Press any key to continue..</strong>




while other languages, such as Perl 5 and earlier, have a

dominant implementation that is used as a reference.

The term computer language is sometimes used interchangeably

with programming language.However, the usage of both

terms varies among authors, including the exact scope of each.

One usage describes programming languages as a subset

of computer languages.




—————————————–




<strong>Press any key to continue..</strong>




week7_sample_program_short.txt has 6 records




week7_sample_program_short.txt ——- First 10 records in file —–




This introductory course in C++ programming includes object-oriented,

event-driven, interactive programming techniques. Topics include

data types, pointers, arrays, stacks, recursion, string processing,

searching and sorting algorithms, classes and objects, references

and memory addresses, scope, streams and files, and graphics. A wide

variety of business-oriented problems are solved by writing C++ programs.




———————————




<strong>Press any key to continue..</strong>




week7_sample_program_short.txt has 6 records




week7_sample_program_short.txt—- Last 10 records in file —–




This introductory course in C++ programming includes object-oriented,

event-driven, interactive programming techniques. Topics include

data types, pointers, arrays, stacks, recursion, string processing,

searching and sorting algorithms, classes and objects, references

and memory addresses, scope, streams and files, and graphics. A wide

variety of business-oriented problems are solved by writing C++ programs.




—————————————–




<strong>Press any key to continue..</strong>




week7_sample_program_short.txt has 6 records




week7_sample_program_short.txt——- All records in file ———–




This introductory course in C++ programming includes object-oriented,

event-driven, interactive programming techniques. Topics include

data types, pointers, arrays, stacks, recursion, string processing,

searching and sorting algorithms, classes and objects, references

and memory addresses, scope, streams and files, and graphics. A wide

variety of business-oriented problems are solved by writing C++ programs.

—————————————–

<strong>Press any key to continue..</strong>