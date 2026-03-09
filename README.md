# Struktur-Data
Tugas 1 dari mata kuliah Struktur Data yaitu Selection Short
```
package pt2;

public class pt2a{
    public static void main(String[] args){
        int[] x = {20, 15, 90, 13, 26};
        int n = x.length;
        
        // Cetak arry awal
        System.out.print("Data Asli: [");
        for (int i = 0; i < n; i++) {
            System.out.print(x[i]);
            if (i < n - 1) System.out.print(", ");
        }
        System.out.println("]");
        
        // Selection sort
        for (int i = 0; i < n - 1; i++) {
            int min = i;
            // Mencari elemen terkecil
            for (int j = i + 1; j < n; j++) {
                if (x[j] < x[min]) {
                    min = j;
                }
            }
            // menukar nilai jika min bukan i
            if (min != i) {
                int temp = x[i];
                x[i] = x[min];
                x[min] = temp;
            }
            
            // Menampilkan iterasi
            System.out.print("Iterasi " + (i + 1) + ": [");
            for (int o = 0; o < n; o++) {
                System.out.print(x[o]);
                if (o < n - 1) System.out.print(", ");
            }
            System.out.println("]");
        }
    }
}
```
Hasil atau output dari Codingan diatas

<img width="371" height="152" alt="Screenshot 2026-03-09 094623" src="https://github.com/user-attachments/assets/9c44c391-f101-40c4-909b-e956ff47117c" />
