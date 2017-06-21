using System;

namespace Distance
{
    class Distance
    {
        static void Main(string[] args)
        {
            int speed = int.Parse(Console.ReadLine());
            int firstTime = int.Parse(Console.ReadLine());
            int secondTime = int.Parse(Console.ReadLine());
            int thirdTime = int.Parse(Console.ReadLine());

            double distance = speed * (firstTime / 60.00);
            double secondSpeed = speed * 1.10;
            distance += secondSpeed * (secondTime / 60.00);
            double thirdSpeed = secondSpeed * 0.95;
            distance += thirdSpeed * (thirdTime / 60.00);

            Console.WriteLine($"{distance:f2}");
        }
    }
}
