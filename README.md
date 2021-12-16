# student
package com.company;
public class Student {
    private String surname;
    private double grade1, grade2;

    public Student(String surname, double grade1, double grade2) {
        this.surname = surname;
        this.grade1 = grade1;
        this.grade2 = grade2;
    }

    public void setGrade(double grade){
       if(grade1 >=1 && grade1 <=6){
            this.grade1=grade;
        }
    }

    public void setGrade(double grade1, double grade2){
        if(grade1>=1 && grade1<=6)
        {
            this.grade1=grade1;
            if(grade2>=1 && grade2<=6){
                this.grade2=grade2;
            }

        }
    }

    public double average(){
        return (grade1 + grade2) / 2;
    }

    public String toString() {
        return "Student: " + surname +", oceny: "+ grade1 + " " + grade2;
    }
}
