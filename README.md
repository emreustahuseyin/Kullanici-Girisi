# Kullanici-Girisi



     
     import java.util.Scanner;
    public class kullaniciGirisi {
         public static void main(String[] args) {
            String userName, password;

        Scanner inp= new Scanner(System.in);

        System.out.println("Kullanıcı Adınız: ");
        userName= inp.nextLine();

        System.out.println("Şifreniz : ");
        password= inp.nextLine();


        if (userName.equals("patika") && password.equals("java123")) {
            System.out.println("Giriş Yaptınız !");
        }else{
            System.out.println("Bilgileriniz Yanlış!");

            System.out.println("Şifrenizi Sıfırlamak istiyor musunuz(evet ise E'ye basın)");
            String answer = inp.nextLine();

            if (answer.equals("E")){
                System.out.println("Yeni Şifrenizi Giriniz");
                String newPassword= inp.nextLine();

                if(newPassword.equals("java123")){
                    System.out.println("Yeni Şifre İle Eski Şifre Aynı Olamaz");
                }else{
                    System.out.println("Şifre Oluşturuldu");
                 }

              }

           }

        }
     }
