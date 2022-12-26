# Ujian-Akhir-Semester
# Ujian Akhir Semester 
<br>Mata Kuliah 	:Dasar Pemrograman
<br> Nama		:Muhammad Fadhiil Hidayatullah
<br>NIM		:	1227050087
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
 Transpose array pada c++ merupakan teknik untuk menukar kolom menjadi baris dan sebaliknya baris menjadi kolom, hal ini digunakan untuk memepermudah dan mempercepat edit data.
## Source Code
#include <iostream>
using namespace std;

void identitas();
int main() {
   int a[10][10], transpose[10][10], row, column, i, j;
   
	identitas();
   cout << "Input baris dan kolom matriks: ";
   cin >> row >> column;

   cout << "\nInput elemen matriks\n";

   // Storing matrix elements
   for (int i = 0; i < row; ++i) {
      for (int j = 0; j < column; ++j) {
         cout << "baris " << i + 1 <<" kolom " << j + 1<< " : ";
         cin >> a[i][j];
      }
   }

   // Printing the a matrix
   cout << "\nMatriks yang diinput: " << endl;
   for (int i = 0; i < row; ++i) {
      for (int j = 0; j < column; ++j) {
         cout << " " << a[i][j];
         //if (j == column - 1)
           
      }
       cout << endl << endl;
   }

   // Computing transpose of the matrix
   for (int i = 0; i < row; ++i)
      for (int j = 0; j < column; ++j) {
         transpose[j][i] = a[i][j];
      }

   // Printing the transpose
   cout << "\nTranspose matriks: " << endl;
   for (int i = 0; i < column; ++i)
      for (int j = 0; j < row; ++j) {
         cout << " " << transpose[i][j];
        if (j == row - 1)
            cout << endl << endl;
      }

   return 0;
}
void identitas(){
	cout<<"==============================================\n";
	cout<<"Nama:	Muhammad Fadhiil Hidayatullah\n";
	cout<<"NIM:	1227050087\n";
	cout<<"==============================================\n\n";
}

## Output

<img width="960" alt="image" src="https://user-images.githubusercontent.com/121006802/209502879-e58fb14f-2899-4c27-a5a4-84245cd67738.png">


