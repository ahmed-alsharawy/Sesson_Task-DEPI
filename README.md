# Sesson_Task-DEPI

using System;
namespace ConsoleApp1
{
    class Program
    {
        static void Main(string[] args)
        {

           
           
                Console.WriteLine("Enter the type (1 for  Number of  Month, 2 For  Name of  month,3 for Temperature, 4  For Grade): ");
                int type = int.Parse(Console.ReadLine());

                if (type == 1)
                {
                    Console.WriteLine("Enter the month number (1-12): ");
                    int month = int.Parse(Console.ReadLine());

                    switch (month)
                    {
                        case 12:
                        case 1:
                        case 2:
                            Console.WriteLine("Season: Winter");
                            break;
                        case 3:
                        case 4:
                        case 5:
                            Console.WriteLine("Season: Spring");
                            break;
                        case 6:
                        case 7:
                        case 8:
                            Console.WriteLine("Season: Summer");
                            break;
                        case 9:
                        case 10:
                        case 11:
                            Console.WriteLine("Season: Autumn");
                            break;
                        default:
                            Console.WriteLine("Invalid month!");
                            break;
                    }
                }
           else if (type == 2)
            {
                Console.WriteLine("Enter the month Name  (January : December): ");
                string month_name = Console.ReadLine();

                switch (month_name)
                {
                    case "December":
                    case "January":
                    case "February":
                        Console.WriteLine("Season: Winter");
                        break;
                    case "March":
                    case "April":
                    case "May":
                        Console.WriteLine("Season: Spring");
                        break;
                    case "June":
                    case "July":
                    case "August":
                        Console.WriteLine("Season: Summer");
                        break;
                    case "Septemper":
                    case "October":
                    case "November":
                        Console.WriteLine("Season: Autumn");
                        break;
                    default:
                        Console.WriteLine("Invalid month!");
                        break;
                }
            }
            else if (type == 3)
                {
                    Console.WriteLine("Enter the temperature: ");
                    int temperature = int.Parse(Console.ReadLine());

                    if (temperature <= 10)
                        Console.WriteLine("Season: Winter");
                    else if (temperature > 10 && temperature <= 20)
                        Console.WriteLine("Season: Autumn");
                    else if (temperature > 20 && temperature <= 30)
                        Console.WriteLine("Season: Spring");
                    else
                        Console.WriteLine("Season: Summer");
                }
            else if (type == 4)
            {
                Console.WriteLine("Enter the Grade Number (1:100): ");
                double Grade = double.Parse(Console.ReadLine());

                if (Grade <= 50)
                    Console.WriteLine("Evaluation : Fail");
                else if (Grade > 50 && Grade <= 65)
                    Console.WriteLine("Evaluation: Accept");
                else if (Grade > 65 && Grade <= 75)
                    Console.WriteLine("Evalution: Good");
                else if (Grade > 75 && Grade <= 85)
                    Console.WriteLine("Evalution: Very Good");
                else
                    Console.WriteLine("Evalution: Excelent");
            }
            else
            {
                Console.WriteLine("Invalid type!");

            }
                




        }
    }
}
