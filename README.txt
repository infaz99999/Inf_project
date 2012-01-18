/*
 * To change this template, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication2;

/**
 *
 * @author INF
 */
public class NewClass {
    public static void main(String[] args) {
    Vehicle v=new Vehicle();
    Car c=new Car();
    v.drive();
    c.drive();
    v=c;
    v.drive();
  
}

    
}

class Vehicle{
    public void drive(){
        System.out.println("I am driving a vehicle");
    }
    
}

class Car extends Vehicle{
    public void drive(){
        System.out.println("I am driving a car");
       
    }
    public void stop(){
        System.out.println("Break");
    }
}

