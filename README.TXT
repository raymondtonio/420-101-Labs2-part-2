Project: better-ticket-machine
Authors: David Barnes and Michael Kölling

This project is part of the material for the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling
   Pearson Education

It is discussed in chapter 2.

Purpose of project: To illustrate conditional statements.
How to start this project: Create one or more TicketMachine objects.

Part III: better-ticket-machine project

47. 

48.- I predict that it will show it will show 0
   - there seems to be differences before and after the change.

49. public void insertMoney(int amount)
    {
        if(amount <=0) {
            System.out.println("Use a positive amount rather than: " + amount);        }
        else {
            balance = balance + amount;
        }
    }
    
50. yes — it was very well suited, because there are only two possible states. True or False

51. In better-ticket-machine, it prints as
      - You must insert at least xyz more cents.
    In naive-ticket-machine, it prints as 
      - ##################
        # The BlueJ Line
        # Ticket
        # 100 cents.
        ##################
    better ticket-machine also has a if or else option for greater than or equal to price.

52. -Yes it is possible and the code still compiles
    -without inserting any money, it does not print.
    
53. No because it only subtracts the price when there’s at least as much money as the price in the balance.

54. unable to access textbook Appendix C

55. saving = price * discount;

56. mean = total / count;

57. public void affordable(int budget)
    {
        if(price > budget)
            System.out.println("Too expensive");
        else {
            System.out.println("Just right");
        }
    }

58. if(price > budget)
            System.out.println("Too expensive: your budget is " + budget)
            
    this one is more easier for me to understand.
    
59. -because the new code wipes out the balance and returns to 0
    -to demonstrate that it does not give the same results as the original, you can use the test int refund balance.

60. the code does not compile because any code written after a return statement will never run. 

61.- the difference is that in the unoriginal version, it's written as int price, however the original version is just price.
   - Yes this version compiles
   - the ticketmachine does not show the value given to it when inspected, because this declares a new local variable called price inside the constructor. 

62. public int emptyMachine()
{   
    int amountEmptied = total;
    total = 0;                 
    return amountEmptied;      
}    

63. public void printTicket()
{
    int amountLeftToPay = price - balance;

    if (amountLeftToPay <= 0) {
    
        System.out.println("##################");
        System.out.println("# The BlueJ Line");
        System.out.println("# Ticket");
        System.out.println("# " + price + " cents.");
        System.out.println("##################");
        System.out.println();

        // Update the total collected with the price.
        total = total + price;
        // Reduce the balance by the price.
        balance = balance - price;
    }
    else {
        
        System.out.printf("You must insert at least %d more cents.%n", amountLeftToPay);
    }
    
64.public void discountedPrice()
    {
        price = price / 2;
        discountedPrice = price;
    }
    
    -(i know this one is wrong, i didn't fully understand this)

