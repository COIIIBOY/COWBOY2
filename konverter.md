# COWBOY2
               static void Main(string[] args)
        {
            Console.WriteLine("Введите длину в миллиметрах");
            string mm = Console.ReadLine();
            double mil;
            bool parsed = Double.TryParse(mm, out mil);
            double sm = mil / 10;
            double dz = sm / 10;
            double metr = dz / 10;
            double km = metr / 1000;
            if ( mil > 0)
            {

                Console.WriteLine($"Введеная длина равна {sm} см");
                Console.WriteLine($"Введеная длина равна {dz} дц");
                Console.WriteLine($"Введеная длина равна {metr} м");
                Console.WriteLine($"Введеная длина равна {km} км");
            }
            if (mil < 0)
            {
                Console.WriteLine("Длина не может быть отрицательной");
            }
            else
            {
                Console.WriteLine("Вы ввели нуль");
            }
            Console.ReadLine();




        }
    }
}
