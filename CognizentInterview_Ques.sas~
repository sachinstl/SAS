Title 'Que Number 1: 2nd max salary from emp table';
data e;
input Name $ salary;
datalines;
a 3000
b 4000
c 5000
d 2500
e 3500
;

proc sql;
select distinct(salary) from e as e1 where 3=(select count(distinct Salary) from e as e2 where e1.salary<=e2.salary);
title;



title 'Que Number 2: Give the output in two line for below table';

data Customer;
input Name $ LandlineNumber Mobilenumber;
datalines;
A1 2345 45
A2 . 45
A3 4523 .
A4 . 45
;
title;



title 'Que Number 3:Sum and + difference';
data student;
input ID Math E H S;
datalines;
101 50 25 70 .
102 60 40 . 35
103 . 40 60 50
104 40 60 50 50
;

data B; set student;
total_s= sum(math, E, H, S);
Total_T=math+E+H+S;


proc print data=B;
title;



title 'Que Number 4: How to join the address';
data address;
input address $10.;
datalines;
ABC s D 1234
ABC s 123
AB s 12
;

data A;
set address;

call scan(s,,,);
title;



Title 'Que Number 5: How to create one column from two columns without missing values?'
data s1;
infile datalines dlm=',' missover;
input name $ landlineNumber $ MobileNumber $;
datalines;
a1,l1,m1
a2, ,m2
a3,l3,  
a4, ,m4
;


data s3;
set s1(rename=landlineNumber=R) s1(rename=MobileNumber=R);
drop landlineNumber MobileNumber;
run;


proc print data=s3;
where R is not missing;

title;
