# palindromNumbers
public class Main {
    static boolean isPalindrom(int number) {
        int temp = number, reverseNumber = 0, lastNumber;
        while (temp != 0) {
            System.out.println("NUmber => " + temp);
            lastNumber = temp % 10;
            System.out.println("Son Basamak => " + lastNumber);
            reverseNumber = (reverseNumber * 10) + lastNumber;
            System.out.println("Yeni sayi => " + reverseNumber);
            temp /= 10;
        }
        if (number == reverseNumber) {
            System.out.println(number + " is palindrom");
        } else {
            System.out.println(number + " is NOT palindrom");
        }
        return true;
    }
    public static void main(String[] args) {
        isPalindrom(3431);
    }
}
