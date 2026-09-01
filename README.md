# Index.java
import java.util.Scanner;
public class Index {
    public static void main(String [] args){
        Scanner read=new Scanner(System.in);
        double credit=-1;
        double grade =-1;
        double sumC=0;
        double sumG=0;
        double points=0;
        double Fresult=0;
        int counter=1;
        while(counter<=20 && counter!=0 && grade!=0 && credit!=0){
            //Enter 0 in grade and credit if you want to end
            System.out.println("Enter your grade in the subject number "+counter);
            grade=read.nextDouble();
            System.out.println("Enter your credits in subject number "+counter);
            credit=read.nextDouble();
            points=credit*grade;
            sumG+=points;
            sumC+=credit;
            Fresult=sumG/sumC;
            counter++;

        }
        System.out.println("The sum points of all the subjects:"+sumG);
        System.out.println("The sum credits of each subject"+sumC);
        System.out.println("The final result which it means the GPA:"+Fresult);

    }
}




