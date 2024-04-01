// // // See https://aka.ms/new-console-template for more information
// // Console.WriteLine("Hello, World!");

// // задача № 3


// Random random = new Random();

// void FillArrayRecursively(int[] array, int index)
// {
//     if (index < array.Length)
//     {
//         array[index] = random.Next(100);
//         Console.Write(array[index] + " ");
//         FillArrayRecursively(array, index + 1);
//     }
// }

// void ReversePrint(int[] arr, int index)
// {
//     if (index >= 0)
//     {
//         Console.Write(arr[index] + " ");
//         ReversePrint(arr, index - 1);
//     }
// }

// Console.Write("Введите размер массива: ");
// int size = int.Parse(Console.ReadLine() ?? "0");
// int[] myArray = new int[size];

// Console.WriteLine("Сгенерированный массив: ");
// FillArrayRecursively(myArray, 0);
// Console.WriteLine("nПеревернутый массив: ");
// ReversePrint(myArray, myArray.Length - 1);
// Console.WriteLine();


// задача № 2

// using System;

// class Program
// {
//     static int Ackermann(int m, int n)
//     {
//         if (m == 0)
//         {
//             return n + 1;
//         }
//         else if (m > 0 && n == 0)
//         {
//             return Ackermann(m - 1, 1);
//         }
//         else if (m > 0 && n > 0)
//         {
//             return Ackermann(m - 1, Ackermann(m, n - 1));
//         }
//         else
//         {
//             return -1; // обработка некорректных входных данных
//         }
//     }

//     static void Main(string[] args)
//     {
//         int m = 3;
//         int n = 2;
//         int result = Ackermann(m, n);
//         Console.WriteLine($"Ackermann({m}, {n}) = {result}");

//         /*
//          * Пример вывода:
//          * Ackermann(3, 2) = 29
//          */
//     }
// }


// задача №1

// using System;

// class Program
// {
//     static void Main(string[] args)
//     {
//         Console.Write("Введите значение M: ");
//         int m = int.Parse(Console.ReadLine());

//         Console.Write("Введите значение N: ");
//         int n = int.Parse(Console.ReadLine());

//         PrintNaturalNumbers(m, n);

//         Console.ReadLine();
//     }

//     static void PrintNaturalNumbers(int m, int n)
//     {
//         if (m <= n)
//         {
//             Console.WriteLine(m);
//             PrintNaturalNumbers(m + 1, n);
//         }
//     }
