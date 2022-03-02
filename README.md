package com.company;

public class Main {

    public static void main(String[] args) {

        int age = -25;
        int temp = -25;
        int temp1 = 30;
        int age1 = 45;

        int random_number1 = age + (int) (Math.random() * age1); // Генерация 1-го числа
        System.out.println(random_number1);

        int random_number2 = temp + (int) (Math.random() * temp1); // Генерация 2-го числа
        System.out.println(random_number2);




        System.out.println(human(20,27));

        System.out.println(human(23,20));

        System.out.println(human(2,19));

        System.out.println(human(3,14));

        System.out.println(human(5,15));


    }

    public static String human (int temperature ,int age){
        String NUM = "можно итди гулять";
        String NUM2 = "нельзя итди гулять"; //ок
        String NUM3 = "оставайтесь дома";
        String NUM4 = "можноли итди гулять";
        if(age >= 20 && age <= 45 && temperature >= -25 && temperature <= 30) {
            return NUM;
        } else if (age <= 20 && temperature > 0 && temperature <=28){
            return NUM;
        } else {
            return NUM3;
        }
    }
}
