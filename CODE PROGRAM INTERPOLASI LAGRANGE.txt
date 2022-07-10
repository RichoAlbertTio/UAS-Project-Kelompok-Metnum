program baru;
uses crt;
//Mendeklarasikan variabel 
var x, x0, x1, x2, x3, pers1, pers2, pers3, pers4, cara1, cara2, cara3, cara4, hasil : real;
// Mendeklarasikan y hasil dari 10 log x
const y0 =2.4771;
	  y1 =2.4829;
	  y2 =2.4843;
	  y3 =2.4871;

begin
clrscr;
writeln;
write('--Mencari Persamaan Linier--');
writeln; writeln;
// Memasukan data x
write('    Masukan nilai x[0] = '); readln(x0);
write('    Masukan nilai x[1] = '); readln(x1);
write('    Masukan nilai x[2] = '); readln(x2);
write('    Masukan nilai x[3] = '); readln(x3);
writeln;
// yang di cari ialah 10 log 301 = x= 301
write('>> Masukan nilai x yang akan dicari : ');
readln(x);
pers1   := ((x-x1)*(x-x2)*(x-x3))/((x0-x1)*(x0-x2)*(x0-x3));
pers2   := ((x-x0)*(x-x2)*(x-x3))/((x1-x0)*(x1-x2)*(x1-x3));
pers3   := ((x-x0)*(x-x1)*(x-x3))/((x2-x0)*(x2-x1)*(x2-x3));
pers4   := ((x-x0)*(x-x1)*(x-x2))/((x3-x )*(x3-x1)*(x3-x2));
cara1   := (y0*pers1); 
cara2   := (y1*pers2);
cara3   := (y2*pers3);
cara4   := (y3*pers4);
writeln('>> cara kerjanya :',cara1:4:4,' + ',cara2:4:4,'', cara3:4:4,' + ',cara4:4:4);
hasil   :=cara1 + cara2 + cara3 + cara4; 
writeln;
write('>> Hasil Perhitungan y(x) dari 10 log 301 adalah : ','y(x)=', hasil:4:4);
readln;
end.
