Download Link: https://assignmentchef.com/product/solved-csc-355-database-systems-assignment-6-student
<br>
<table class="highlight tab-size js-file-line-container" data-tab-size="8">

 <tbody>

  <tr>

   <td id="L7" class="blob-num js-line-number" data-line-number="7"></td>

   <td id="LC7" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L8" class="blob-num js-line-number" data-line-number="8"></td>

   <td id="LC8" class="blob-code blob-code-inner js-file-line">Problems:</td>

  </tr>

  <tr>

   <td id="L9" class="blob-num js-line-number" data-line-number="9"></td>

   <td id="LC9" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L10" class="blob-num js-line-number" data-line-number="10"></td>

   <td id="LC10" class="blob-code blob-code-inner js-file-line">1. (PL/SQL Programming) Consider the table STUDENT with attributes ID, Name, Mid, Fin, and HW, and the table PERCENTAGES with attributes MidPercent, FinalPercent, and HWPercent defined and populated by the following script:</td>

  </tr>

  <tr>

   <td id="L11" class="blob-num js-line-number" data-line-number="11"></td>

   <td id="LC11" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L12" class="blob-num js-line-number" data-line-number="12"></td>

   <td id="LC12" class="blob-code blob-code-inner js-file-line">DROP TABLE STUDENT CASCADE CONSTRAINTS;</td>

  </tr>

  <tr>

   <td id="L13" class="blob-num js-line-number" data-line-number="13"></td>

   <td id="LC13" class="blob-code blob-code-inner js-file-line">CREATE TABLE STUDENT</td>

  </tr>

  <tr>

   <td id="L14" class="blob-num js-line-number" data-line-number="14"></td>

   <td id="LC14" class="blob-code blob-code-inner js-file-line">(</td>

  </tr>

  <tr>

   <td id="L15" class="blob-num js-line-number" data-line-number="15"></td>

   <td id="LC15" class="blob-code blob-code-inner js-file-line">ID CHAR(4),</td>

  </tr>

  <tr>

   <td id="L16" class="blob-num js-line-number" data-line-number="16"></td>

   <td id="LC16" class="blob-code blob-code-inner js-file-line">Name VARCHAR2(20),</td>

  </tr>

  <tr>

   <td id="L17" class="blob-num js-line-number" data-line-number="17"></td>

   <td id="LC17" class="blob-code blob-code-inner js-file-line">HW NUMBER(3,0) CHECK (HW&gt;=0 AND HW&lt;=100),</td>

  </tr>

  <tr>

   <td id="L18" class="blob-num js-line-number" data-line-number="18"></td>

   <td id="LC18" class="blob-code blob-code-inner js-file-line">Mid NUMBER(3,0) CHECK (Mid&gt;=0 AND Mid&lt;=100),</td>

  </tr>

  <tr>

   <td id="L19" class="blob-num js-line-number" data-line-number="19"></td>

   <td id="LC19" class="blob-code blob-code-inner js-file-line">Fin NUMBER(3,0) CHECK (Fin&gt;=0 AND Fin&lt;=100),</td>

  </tr>

  <tr>

   <td id="L20" class="blob-num js-line-number" data-line-number="20"></td>

   <td id="LC20" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L21" class="blob-num js-line-number" data-line-number="21"></td>

   <td id="LC21" class="blob-code blob-code-inner js-file-line">PRIMARY KEY (ID)</td>

  </tr>

  <tr>

   <td id="L22" class="blob-num js-line-number" data-line-number="22"></td>

   <td id="LC22" class="blob-code blob-code-inner js-file-line">);</td>

  </tr>

  <tr>

   <td id="L23" class="blob-num js-line-number" data-line-number="23"></td>

   <td id="LC23" class="blob-code blob-code-inner js-file-line">INSERT INTO STUDENT VALUES ( ‘4145’, ‘Seinfeld’, 98, 85, 90 );</td>

  </tr>

  <tr>

   <td id="L24" class="blob-num js-line-number" data-line-number="24"></td>

   <td id="LC24" class="blob-code blob-code-inner js-file-line">INSERT INTO STUDENT VALUES ( ‘9009’, ‘Costanza’, 80, 74, 72 );</td>

  </tr>

  <tr>

   <td id="L25" class="blob-num js-line-number" data-line-number="25"></td>

   <td id="LC25" class="blob-code blob-code-inner js-file-line">INSERT INTO STUDENT VALUES ( ‘1233’, ‘Kramer’, 91, 94, 89 );</td>

  </tr>

  <tr>

   <td id="L26" class="blob-num js-line-number" data-line-number="26"></td>

   <td id="LC26" class="blob-code blob-code-inner js-file-line">INSERT INTO STUDENT VALUES ( ‘1111’, ‘Benes’, 93, 99, 91 );</td>

  </tr>

  <tr>

   <td id="L27" class="blob-num js-line-number" data-line-number="27"></td>

   <td id="LC27" class="blob-code blob-code-inner js-file-line">INSERT INTO STUDENT VALUES ( ‘6676’, ‘Newman’, 84, 78, 84 );</td>

  </tr>

  <tr>

   <td id="L28" class="blob-num js-line-number" data-line-number="28"></td>

   <td id="LC28" class="blob-code blob-code-inner js-file-line">INSERT INTO STUDENT VALUES ( ‘8889’, ‘Banya’, 50, 52, 65 );</td>

  </tr>

  <tr>

   <td id="L29" class="blob-num js-line-number" data-line-number="29"></td>

   <td id="LC29" class="blob-code blob-code-inner js-file-line">SELECT * FROM STUDENT;</td>

  </tr>

  <tr>

   <td id="L30" class="blob-num js-line-number" data-line-number="30"></td>

   <td id="LC30" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L31" class="blob-num js-line-number" data-line-number="31"></td>

   <td id="LC31" class="blob-code blob-code-inner js-file-line">DROP TABLE PERCENTAGES CASCADE CONSTRAINTS;</td>

  </tr>

  <tr>

   <td id="L32" class="blob-num js-line-number" data-line-number="32"></td>

   <td id="LC32" class="blob-code blob-code-inner js-file-line">CREATE TABLE PERCENTAGES</td>

  </tr>

  <tr>

   <td id="L33" class="blob-num js-line-number" data-line-number="33"></td>

   <td id="LC33" class="blob-code blob-code-inner js-file-line">(</td>

  </tr>

  <tr>

   <td id="L34" class="blob-num js-line-number" data-line-number="34"></td>

   <td id="LC34" class="blob-code blob-code-inner js-file-line">HWPercent NUMBER(2,0) CHECK (HWPercent&gt;=0 AND HWPercent&lt;=100),</td>

  </tr>

  <tr>

   <td id="L35" class="blob-num js-line-number" data-line-number="35"></td>

   <td id="LC35" class="blob-code blob-code-inner js-file-line">MidPercent NUMBER(2,0) CHECK (MidPercent&gt;=0 AND MidPercent&lt;=100),</td>

  </tr>

  <tr>

   <td id="L36" class="blob-num js-line-number" data-line-number="36"></td>

   <td id="LC36" class="blob-code blob-code-inner js-file-line">FinPercent NUMBER(2,0) CHECK (FinPercent&gt;=0 AND FinPercent&lt;=100)</td>

  </tr>

  <tr>

   <td id="L37" class="blob-num js-line-number" data-line-number="37"></td>

   <td id="LC37" class="blob-code blob-code-inner js-file-line">);</td>

  </tr>

  <tr>

   <td id="L38" class="blob-num js-line-number" data-line-number="38"></td>

   <td id="LC38" class="blob-code blob-code-inner js-file-line">INSERT INTO PERCENTAGES VALUES ( 40, 30, 30 );</td>

  </tr>

  <tr>

   <td id="L39" class="blob-num js-line-number" data-line-number="39"></td>

   <td id="LC39" class="blob-code blob-code-inner js-file-line">SELECT * FROM PERCENTAGES;</td>

  </tr>

  <tr>

   <td id="L40" class="blob-num js-line-number" data-line-number="40"></td>

   <td id="LC40" class="blob-code blob-code-inner js-file-line">COMMIT;</td>

  </tr>

  <tr>

   <td id="L41" class="blob-num js-line-number" data-line-number="41"></td>

   <td id="LC41" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L42" class="blob-num js-line-number" data-line-number="42"></td>

   <td id="LC42" class="blob-code blob-code-inner js-file-line">Write a script file Problem1.sql containing an anonymous PL/SQL block that will do the following:</td>

  </tr>

  <tr>

   <td id="L43" class="blob-num js-line-number" data-line-number="43"></td>

   <td id="LC43" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L44" class="blob-num js-line-number" data-line-number="44"></td>

   <td id="LC44" class="blob-code blob-code-inner js-file-line">First, report the three percentages found in the PERCENTAGES table. (You may assume that the PERCENTAGES table contains only one record.) Next, output the name of each student in the STUDENT table and their overall score, computed as x percent Homework, y percent Midterm, and z percent Final, where x, y, and z are the corresponding percentages found in the PERCENTAGES table.(You may assume that x+y+z=100.) Also convert each student’s overall score to a letter grade by the rule 90-100=A, 80-89.99=B, 70-79.99=C, 60-60.99=D, 0-59.99=F, and include the letter grade in the output. Output each student’s information on a separate line. For the sample data given above, the output should be:</td>

  </tr>

  <tr>

   <td id="L45" class="blob-num js-line-number" data-line-number="45"></td>

   <td id="LC45" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L46" class="blob-num js-line-number" data-line-number="46"></td>

   <td id="LC46" class="blob-code blob-code-inner js-file-line">Weights are 40, 30, 30</td>

  </tr>

  <tr>

   <td id="L47" class="blob-num js-line-number" data-line-number="47"></td>

   <td id="LC47" class="blob-code blob-code-inner js-file-line">4145 Seinfeld 91.7 A</td>

  </tr>

  <tr>

   <td id="L48" class="blob-num js-line-number" data-line-number="48"></td>

   <td id="LC48" class="blob-code blob-code-inner js-file-line">9009 Costanza 75.8 C</td>

  </tr>

  <tr>

   <td id="L49" class="blob-num js-line-number" data-line-number="49"></td>

   <td id="LC49" class="blob-code blob-code-inner js-file-line">1233 Kramer 91.3 A</td>

  </tr>

  <tr>

   <td id="L50" class="blob-num js-line-number" data-line-number="50"></td>

   <td id="LC50" class="blob-code blob-code-inner js-file-line">1111 Benes 94.2 A</td>

  </tr>

  <tr>

   <td id="L51" class="blob-num js-line-number" data-line-number="51"></td>

   <td id="LC51" class="blob-code blob-code-inner js-file-line">6676 Newman 82.2 B</td>

  </tr>

  <tr>

   <td id="L52" class="blob-num js-line-number" data-line-number="52"></td>

   <td id="LC52" class="blob-code blob-code-inner js-file-line">8889 Banya 55.1 F</td>

  </tr>

  <tr>

   <td id="L53" class="blob-num js-line-number" data-line-number="53"></td>

   <td id="LC53" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L54" class="blob-num js-line-number" data-line-number="54"></td>

   <td id="LC54" class="blob-code blob-code-inner js-file-line">Of course, this is just an example – your PL/SQL block should work in general, not just for the given sample data.</td>

  </tr>

  <tr>

   <td id="L55" class="blob-num js-line-number" data-line-number="55"></td>

   <td id="LC55" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L56" class="blob-num js-line-number" data-line-number="56"></td>

   <td id="LC56" class="blob-code blob-code-inner js-file-line">2. (Triggers) Consider the JOB and CONTRACT tables defined by the following script, which also populates the JOB table:</td>

  </tr>

  <tr>

   <td id="L57" class="blob-num js-line-number" data-line-number="57"></td>

   <td id="LC57" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L58" class="blob-num js-line-number" data-line-number="58"></td>

   <td id="LC58" class="blob-code blob-code-inner js-file-line">DROP TABLE CONTRACT CASCADE CONSTRAINTS;</td>

  </tr>

  <tr>

   <td id="L59" class="blob-num js-line-number" data-line-number="59"></td>

   <td id="LC59" class="blob-code blob-code-inner js-file-line">DROP TABLE JOB CASCADE CONSTRAINTS;</td>

  </tr>

  <tr>

   <td id="L60" class="blob-num js-line-number" data-line-number="60"></td>

   <td id="LC60" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L61" class="blob-num js-line-number" data-line-number="61"></td>

   <td id="LC61" class="blob-code blob-code-inner js-file-line">CREATE TABLE JOB</td>

  </tr>

  <tr>

   <td id="L62" class="blob-num js-line-number" data-line-number="62"></td>

   <td id="LC62" class="blob-code blob-code-inner js-file-line">(</td>

  </tr>

  <tr>

   <td id="L63" class="blob-num js-line-number" data-line-number="63"></td>

   <td id="LC63" class="blob-code blob-code-inner js-file-line">JobID CHAR(3),</td>

  </tr>

  <tr>

   <td id="L64" class="blob-num js-line-number" data-line-number="64"></td>

   <td id="LC64" class="blob-code blob-code-inner js-file-line">Title VARCHAR2(20),</td>

  </tr>

  <tr>

   <td id="L65" class="blob-num js-line-number" data-line-number="65"></td>

   <td id="LC65" class="blob-code blob-code-inner js-file-line">ContractCount NUMBER(1,0) DEFAULT 0,</td>

  </tr>

  <tr>

   <td id="L66" class="blob-num js-line-number" data-line-number="66"></td>

   <td id="LC66" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L67" class="blob-num js-line-number" data-line-number="67"></td>

   <td id="LC67" class="blob-code blob-code-inner js-file-line">CONSTRAINT PK_JOB</td>

  </tr>

  <tr>

   <td id="L68" class="blob-num js-line-number" data-line-number="68"></td>

   <td id="LC68" class="blob-code blob-code-inner js-file-line">PRIMARY KEY (JobID)</td>

  </tr>

  <tr>

   <td id="L69" class="blob-num js-line-number" data-line-number="69"></td>

   <td id="LC69" class="blob-code blob-code-inner js-file-line">);</td>

  </tr>

  <tr>

   <td id="L70" class="blob-num js-line-number" data-line-number="70"></td>

   <td id="LC70" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L71" class="blob-num js-line-number" data-line-number="71"></td>

   <td id="LC71" class="blob-code blob-code-inner js-file-line">CREATE TABLE CONTRACT</td>

  </tr>

  <tr>

   <td id="L72" class="blob-num js-line-number" data-line-number="72"></td>

   <td id="LC72" class="blob-code blob-code-inner js-file-line">(</td>

  </tr>

  <tr>

   <td id="L73" class="blob-num js-line-number" data-line-number="73"></td>

   <td id="LC73" class="blob-code blob-code-inner js-file-line">JobID CHAR(3),</td>

  </tr>

  <tr>

   <td id="L74" class="blob-num js-line-number" data-line-number="74"></td>

   <td id="LC74" class="blob-code blob-code-inner js-file-line">WorkerID CHAR(7),</td>

  </tr>

  <tr>

   <td id="L75" class="blob-num js-line-number" data-line-number="75"></td>

   <td id="LC75" class="blob-code blob-code-inner js-file-line">Payment NUMBER(6,2),</td>

  </tr>

  <tr>

   <td id="L76" class="blob-num js-line-number" data-line-number="76"></td>

   <td id="LC76" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L77" class="blob-num js-line-number" data-line-number="77"></td>

   <td id="LC77" class="blob-code blob-code-inner js-file-line">CONSTRAINT PK_CONTRACT</td>

  </tr>

  <tr>

   <td id="L78" class="blob-num js-line-number" data-line-number="78"></td>

   <td id="LC78" class="blob-code blob-code-inner js-file-line">PRIMARY KEY (JobID, WorkerID),</td>

  </tr>

  <tr>

   <td id="L79" class="blob-num js-line-number" data-line-number="79"></td>

   <td id="LC79" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L80" class="blob-num js-line-number" data-line-number="80"></td>

   <td id="LC80" class="blob-code blob-code-inner js-file-line">CONSTRAINT FK_CONTRACT_JOB</td>

  </tr>

  <tr>

   <td id="L81" class="blob-num js-line-number" data-line-number="81"></td>

   <td id="LC81" class="blob-code blob-code-inner js-file-line">FOREIGN KEY (JobID)</td>

  </tr>

  <tr>

   <td id="L82" class="blob-num js-line-number" data-line-number="82"></td>

   <td id="LC82" class="blob-code blob-code-inner js-file-line">REFERENCES JOB (JobID)</td>

  </tr>

  <tr>

   <td id="L83" class="blob-num js-line-number" data-line-number="83"></td>

   <td id="LC83" class="blob-code blob-code-inner js-file-line">);</td>

  </tr>

  <tr>

   <td id="L84" class="blob-num js-line-number" data-line-number="84"></td>

   <td id="LC84" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L85" class="blob-num js-line-number" data-line-number="85"></td>

   <td id="LC85" class="blob-code blob-code-inner js-file-line">INSERT INTO JOB (JobID, Title) VALUES ( ‘100’, ‘Security’ );</td>

  </tr>

  <tr>

   <td id="L86" class="blob-num js-line-number" data-line-number="86"></td>

   <td id="LC86" class="blob-code blob-code-inner js-file-line">INSERT INTO JOB (JobID, Title) VALUES ( ‘299’, ‘Infrastructure’ );</td>

  </tr>

  <tr>

   <td id="L87" class="blob-num js-line-number" data-line-number="87"></td>

   <td id="LC87" class="blob-code blob-code-inner js-file-line">INSERT INTO JOB (JobID, Title) VALUES ( ‘757’, ‘Compliance’ );</td>

  </tr>

  <tr>

   <td id="L88" class="blob-num js-line-number" data-line-number="88"></td>

   <td id="LC88" class="blob-code blob-code-inner js-file-line">SELECT * FROM JOB;</td>

  </tr>

  <tr>

   <td id="L89" class="blob-num js-line-number" data-line-number="89"></td>

   <td id="LC89" class="blob-code blob-code-inner js-file-line">COMMIT;</td>

  </tr>

  <tr>

   <td id="L90" class="blob-num js-line-number" data-line-number="90"></td>

   <td id="LC90" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L91" class="blob-num js-line-number" data-line-number="91"></td>

   <td id="LC91" class="blob-code blob-code-inner js-file-line">The ContractCount attribute of JOB should store a count of how many workers have signed contracts to work on that job – that is, the number of records in CONTRACT with that JobID – and its value should never exceed 4. Your task is to write three triggers that will maintain the value of the ContractCount attribute in JOB as changes are made to the CONTRACT table.</td>

  </tr>

  <tr>

   <td id="L92" class="blob-num js-line-number" data-line-number="92"></td>

   <td id="LC92" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L93" class="blob-num js-line-number" data-line-number="93"></td>

   <td id="LC93" class="blob-code blob-code-inner js-file-line">Write a script file Problem2.sql containing definitions of the following three triggers:</td>

  </tr>

  <tr>

   <td id="L94" class="blob-num js-line-number" data-line-number="94"></td>

   <td id="LC94" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L95" class="blob-num js-line-number" data-line-number="95"></td>

   <td id="LC95" class="blob-code blob-code-inner js-file-line">1. The first trigger, named NewContract, will fire when a user attempts to INSERT a row into CONTRACT. This trigger will check the value of ContractCount for the corresponding job. If ContractCount is less than 4, then there is still room in the job for another worker, so it will allow the INSERT to occur and will increase the value of ContractCount by one. If ContractCount is equal to 4, then the job is full, so it will cancel the INSERT and display an error message stating that the job is full.</td>

  </tr>

  <tr>

   <td id="L96" class="blob-num js-line-number" data-line-number="96"></td>

   <td id="LC96" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L97" class="blob-num js-line-number" data-line-number="97"></td>

   <td id="LC97" class="blob-code blob-code-inner js-file-line">2. The second trigger, named EndContract, will fire when a user attempts to DELETE one or more rows from CONTRACT. This trigger will update the values of ContractCount for any affected jobs to make sure they are accurate after the rows are deleted, by decreasing the value of ContractCount by one each time a worker is removed from a job.</td>

  </tr>

  <tr>

   <td id="L98" class="blob-num js-line-number" data-line-number="98"></td>

   <td id="LC98" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L99" class="blob-num js-line-number" data-line-number="99"></td>

   <td id="LC99" class="blob-code blob-code-inner js-file-line">3. The third trigger, named NoChanges, will fire when a user attempts to UPDATE one or more rows of CONTRACT. The trigger will cancel the UPDATE and display an error message stating that no updates are permitted to existing rows of CONTRACT.</td>

  </tr>

  <tr>

   <td id="L100" class="blob-num js-line-number" data-line-number="100"></td>

   <td id="LC100" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L101" class="blob-num js-line-number" data-line-number="101"></td>

   <td id="LC101" class="blob-code blob-code-inner js-file-line">NewContract and EndContract should be row-level triggers; NoChanges should be a statement-level trigger.</td>

  </tr>

  <tr>

   <td id="L102" class="blob-num js-line-number" data-line-number="102"></td>

   <td id="LC102" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L103" class="blob-num js-line-number" data-line-number="103"></td>

   <td id="LC103" class="blob-code blob-code-inner js-file-line">Run the script to define your triggers and test them to make sure they work by doing a few INSERTS, DELETES, and UPDATES on the CONTRACT table.</td>

  </tr>

  <tr>

   <td id="L104" class="blob-num js-line-number" data-line-number="104"></td>

   <td id="LC104" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L105" class="blob-num js-line-number" data-line-number="105"></td>

   <td id="LC105" class="blob-code blob-code-inner js-file-line">Include a comment at the top of each of your script files giving your name, the course number and section, the assignment number, and the date of submission, e.g.:</td>

  </tr>

  <tr>

   <td id="L106" class="blob-num js-line-number" data-line-number="106"></td>

   <td id="LC106" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

  <tr>

   <td id="L107" class="blob-num js-line-number" data-line-number="107"></td>

   <td id="LC107" class="blob-code blob-code-inner js-file-line"></td>

  </tr>

 </tbody>

</table>