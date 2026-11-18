# Prog-final-exam

// Question 1//

import java.util.*;
import java.util.Scanner;

import static java.util.Arrays.fill;

public class MattressSales {
    public static void main(String[] args) {

        //Declaration of variables//



        //Cozy night mattress sales//
        System.out.println("Enter the number of sales for month 1 for Cozy Nights Monarch mattress: ");
        System.out.println("Enter the number of sales for month 2 for Cozy Nights Monarch mattress: ");
        System.out.println("Enter the number of sales for month 3 for Cozy Nights Monarch mattress: ");

        // Restonic mattress sales//
        System.out.println();
        System.out.println("Enter the number of sales for month 1 for Restonic Barbados mattress: ");
        System.out.println("Enter the number of sales for month 2 for Restonic Barbados mattress: ");
        System.out.println("Enter the number of sales for month 3 for Restonic mattress: ");

        //Sealy mattress saless//
        System.out.println();
        System.out.println("Enter the number of sales for month 1 for Sealy Phuket mattress: ");
        System.out.println("Enter the number of sales for month 2 for Sealy Phuket mattress: ");
        System.out.println("Enter the number of sales for month 3 for Sealy Phuket mattress: ");
        System.out.println();

        Scanner input = new Scanner(System.in);

        System.out.println("PRODUCT SALES REPORT - 2026");
        System.out.println();
        System.out.println("********************************************");

        // Question 1.2//
        class Product{
            public interface IProduct{
                default int GetTotalProductsSold() {
                    return 0;
                }

                default double GetAverageProductsSold() {
                    return 0;
                }

                default String GetMostPopularProduct() {
                    return null;
                }
            }



        }


        //Question 1.3//
        class PrintProduct{


        }






    }
}



// Question 2//

import javax.swing.*;

public class CompanyMatressSalesApp {
    public static void main(String[] args) {
        JFrame frame = new JFrame();
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        // The declaration of the arrays//
        final int NUMBER_OF_ITEMS = 1;
        String[] CustomerName = {"Joe Bloggs"};
        double[] price = {3500};
        double[] VAT = {525.0};
        double[] Commisson = {175.0};
        double[] Total = {4200.0};

        String strItem;
        double itemPrice = 0.0;
        double itemVAT = 0.0;
        double itemCommisson = 0.0;
        double itemTotal = 0.0;

        // Validates the item price//
        boolean isValidItemPrice = false;
        strItem = JOptionPane.showInputDialog(null, " Enter Price: ");
        itemPrice = Double.parseDouble(strItem);

        //Validates the customer name//
        boolean isValidCustomerName = false;
        strItem = JOptionPane.showInputDialog(null, " Customer Name: ");
        CustomerName = strItem.split("Joe Bloggs");

        for (double i : price) {
            if (CustomerName[0].equals(CustomerName[1])) {
                itemPrice = i;
                isValidCustomerName = true;
            }
        }
        if (!isValidCustomerName) {
            JOptionPane.showMessageDialog(null, "Customer Name is invalid");

        }

        //Question 2.5//

    }

    private interface IProductCalculations {
        default double GetVat() {
            return 0;
        }

        default double GetCommisson() {
            return 0;
        }

        double GetTotal();
        default double GetAverageProductsSold() {
            return 0;
        }
    }
}






