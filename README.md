# grade_average

import java.util.Scanner;

/*
Not Ortalaması Hesaplayan Program
Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı yazın.

AlıştırmA
Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.
Not : If ve Else kullanılmayacak...
 */

public class Not_Ortalamasi_Hesaplayan_Program {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Lütfen notlarınızı ilgili kısımlara giriniz.");
        System.out.print("Matematik: ");
        int mat = input.nextInt();
        
        System.out.print("Fizik: ");
        int fiz = input.nextInt();
        
        System.out.print("Kimya: ");
        int kim = input.nextInt();
        
        System.out.print("Türkçe: ");
        int tur = input.nextInt();
        
        System.out.print("Tarih: ");
        int tar = input.nextInt();
        
        System.out.print("Müzik: ");
        int muz = input.nextInt();

        double result = ((mat+fiz+kim+tur+tar+muz)/6);

        System.out.println("Ortalamanız :" + result);


        boolean compare = result >= 60;

        String str = compare ? "Sınıfı Geçtiniz." : "Sınıfta Kaldınız.";
        System.out.println(str);

    }
}
