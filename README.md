# Interest-on-savings-calculator
This program takes in the amount of money and the intrest rate an calculates how money the person will recieve

Console.WriteLine("Enter number of bank accounts.");
int nofb = Int32.Parse(Console.ReadLine());

int bc = nofb;


for (int i = bc; i != 0; i--)
{
bc--;

Console.WriteLine("What is the amount of money you wish to save ?");
Double mts = Double.Parse(Console.ReadLine());

Console.WriteLine("What is the interest rate ?");
Double ir = Double.Parse(Console.ReadLine());

Double c1 = mts*100;
Double c2 = c1 * ir;
Double c3 = c2 + mts;

float fn = Convert.ToSingle(c3);

Console.WriteLine("========================================================");
Console.WriteLine("The interest on this account is " + "-=" + fn + "=-");
Console.WriteLine("========================================================");

if(bc != 0)
{
Console.WriteLine("You have " + bc + " More accounts to go through");
Console.WriteLine("=================================================");
}

else
{
Console.WriteLine("Thank you for using this service.");
}

}
