program interpolasi_linier;
uses crt;
// Mendeklarasikan variabel
var x1, x2, y1, y2, hasil :real;
const x=9;
begin
clrscr;
writeln('====Interpolasi Linier====');
// Memasukan data
write('Masukan x1 : '); readln(x1);
write('Masukan y1 : '); readln(y1);
write('Masukan x2 : '); readln(x2);
write('Masukan y2 : '); readln(y2);
//rumus 
hasil:=y1 +(x-x1)/(x2-x1)*(y2-y1);
// Menampilkan hasil
writeln('Jadi hasil yang interpolasi liniernya adalah ',hasil:2:0);
readln;
end.
