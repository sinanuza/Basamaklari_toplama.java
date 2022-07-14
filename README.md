# Basamaklari_toplama.java
www.patika.dev basamak_degeri_toplama



        import java.util.Scanner;

        public class bas_top {
        public static void main(String[] args) {
        int sonuc=0,basamaksayisi=0,basamakdegeri,n=0;
        int number;
        System.out.println("Lutfen sayi giriniz:");
        Scanner input =new Scanner(System.in);
        number=input.nextInt();
        int tempnumber=number;
        while (tempnumber!=0){
            tempnumber/=10;
            basamaksayisi++;
        }
        tempnumber=number;
        while (tempnumber!=0){
            basamakdegeri=tempnumber%10;
            //System.out.println(basamakdegeri);
            tempnumber/=10;
            sonuc+=basamakdegeri;
        }
        System.out.println(sonuc);
    }
}
