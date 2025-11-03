# tugas-5
import java.util.Scanner;

public class RataRataNilai {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan jumlah siswa: ");
        int jumlahSiswa = input.nextInt();

        if (jumlahSiswa <= 0) {
            System.out.println("Jumlah siswa harus lebih dari 0!");
        } else {
            double totalNilai = 0;

            // Loop untuk memasukkan nilai setiap siswa
            for (int i = 1; i <= jumlahSiswa; i++) {
                System.out.print("Masukkan nilai siswa ke-" + i + ": ");
                double nilai = input.nextDouble();
                totalNilai += nilai;
            }

            // Menghitung rata-rata
            double rataRata = totalNilai / jumlahSiswa;

            System.out.println("Rata-rata nilai siswa adalah: " + rataRata);
        }

        input.close();
    }
}Program ini digunakan untuk **menghitung rata-rata nilai siswa**.

1. Pengguna memasukkan **jumlah siswa**.
2. Jika jumlah ≤ 0, program menampilkan pesan error.
3. Jika valid, program meminta **nilai tiap siswa** dengan perulangan `for`.
4. Semua nilai dijumlahkan, lalu dihitung rata-ratanya dengan rumus:
   [
   \text{rata-rata} = \frac{\text{total nilai}}{\text{jumlah siswa}}
   ]
5. Hasil rata-rata ditampilkan ke layar, lalu `Scanner` ditutup.

