/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

 package com.mycompany.dollars.java;

 /**
  *
  * @author sidelele
  */
 import java.util.Scanner;
 public class DollarsJava {
 
     public static void main(String[] args) {
         Scanner conversion=new Scanner(System.in);
         
         System.out.print("Enter the amount in dollars");
         int amount = conversion.nextInt();
         
         int twenties = amount / 20;
         amount %= 20;
         
         int tens = amount / 10;
         amount %= 10;
         
         int fives = amount / 5;
         amount %= 5;
         
         int ones = amount /1;
         amount &= 1;
         
         System.out.println("Currency breakdown:");
         System.out.println("$20 bills:" + twenties);
         System.out.println("$10 bills:" + tens);
         System.out.println("$5 bills:" + fives);
         System.out.println("$1 bills:" + ones);
         
         
     
     }
 }


