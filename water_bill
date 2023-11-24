namespace waterbill__calc
{
    internal class Program
    {
        static void Main(string[] args)
        {
            do
            {
                Console.WriteLine("\t\t\t=============================================");
                Console.WriteLine("\t\t\t\twelcome to waterbill calculator");
                Console.WriteLine("\t\t\t=============================================");
                Console.Write("enter water consumption in (cubic metres): ");
                if (!double.TryParse(Console.ReadLine(), out double waterconsumption)||waterconsumption<0)
                {
                    Console.WriteLine("invalid entry");
                    return;
                }
                Console.WriteLine("type your  usagetype between: ");
                Console.WriteLine("1: residential \n2: commercial \n3:indurstrial");
                Console.Write("usage type is: ");
                string usagetype = Console.ReadLine().ToLower();
                double rate = 0;
                switch (usagetype)
                {
                    case "residential":
                        rate = 25.00; break;
                    case "commercial":
                        rate = 30.50; break;
                    case "indurstrial":
                        rate=35.75; break;
                    default:
                        Console.WriteLine("your choice is invalid");
                        return;
                }
                double totalbill = rate*waterconsumption;
                Console.WriteLine("\t YOUR MONTHLY WATERBILL IS:");
                Console.WriteLine($"\tyour waterconsumption is:{waterconsumption} cubic metres");
                Console.WriteLine($"\tyour usagetype is:{usagetype}");
                Console.WriteLine($"\tyour totalbill is:{totalbill}");
                Console.WriteLine("do you want to continue (Y: yes N: no): ");
            }while (Console.ReadLine().ToUpper()=="Y");
            Console.WriteLine("bye!");
        }
    }
}
