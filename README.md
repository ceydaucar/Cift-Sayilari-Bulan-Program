# Girilen-Sayiya-Kadar-Olan-Cift-Sayilari-Bulan-Program
Patika.dev > Java101 > Döngüler > Pratik1 - Girilen Sayıya Kadar Olan Çift Sayıları Bulan Program

Java döngüler ile kullanıcının girdiği sayıya kadar çift olan sayıları bulan programı yazıyoruz.

### Ödev

Java döngüler ile 0'dan girilen sayıya kadar olan sayılardan 3 ve 4'e tam bölünen sayıların ortalamasını hesaplayan programı yazınız.


      import java.util.*;

      public class cift_sayilari_bulan_program {

        public static void main(String[] args) {

          Scanner sc = new Scanner(System.in);
          System.out.print("Please enter a number: ");
          int n = sc.nextInt();

          int count = 0;
          int sum = 0;
          for (int i = 1; i <= n; i++) {
            if(i % 12 == 0) {
              sum += i;
              count++;
            }
          }

          System.out.print("Average of numbers divisible by 3 and 4: " + (sum/count));

          }
      }
