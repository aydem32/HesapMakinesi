import java.util.Scanner;

public class HesapMakinesi {

    public static void main(String[] args){

        int number1;
        int number2;
        int select;

        Scanner input = new Scanner(System.in);

        System.out.println("Birinci sayıyı giriniz?");
        number1 = input.nextInt();
        System.out.println("İkinci Sayıyı giriniz?");
        number2 = input.nextInt();

        System.out.println("Hangi işlemi yapmak istiyorsunuz");
        System.out.println("1.Toplama");
        System.out.println("2.Çıkarma");
        System.out.println("3.Çarpma");
        System.out.println("4.Bölme");

        select = input.nextInt();

        switch (select){
            case 1:
                System.out.println("Toplama : " +(number1+number2));
                break;
            case 2:
                System.out.println("Çıkarma : " +(number1 - number2));
                break;
            case 3:
                System.out.println("Çapma : " +(number1*number2));
                break;
            case 4:
                if (number2 != 0){
                    System.out.println("Bölne : " +(number1/number2));
                } else {
                    System.out.println("2. sayı 0 olamaz");
                }
                break;
            default:
                System.out.println("Geçersiz Değer");
        }

    }

}
