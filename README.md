# Taximeter

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        
        //Müşterinin Gideceği mesafeyi girmesi için veri girişi yapılacak
        
        Scanner inp=new Scanner(System.in);
        
        double km,minTutar=20,tutar = 0,acılıs=10,sbt=2.20,sonT;

        System.out.println("Lütfen Gideceğiniz Mesafeyi Km Olarak Giriniz: ");
        
        km = inp.nextDouble();

        tutar=acılıs+(km*sbt);
        
        sonT=tutar > minTutar ? tutar : minTutar ;
        
        System.out.println("Taksimetre Km Ücreti: "+sonT);
    }
}