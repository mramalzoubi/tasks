# tasks
using System;

class Program
{
    static void Main()
    {

        int[][] jaggedArray = new int[3][];
        jaggedArray[0] = new int[] { 1, 2, 3 };
        jaggedArray[1] = new int[] { 4, 5 };
        jaggedArray[2] = new int[] { 6, 7, 8, 9 };

    
        int[,] rectangularArray = new int[3, 4]
        {
            { 1, 2, 3, 4 },
            { 5, 6, 7, 8 },
            { 9, 10, 11, 12 }
        };

     
        Console.WriteLine("Jagged Array:");
        for (int i = 0; i < jaggedArray.Length; i++)
        {
            Console.Write("Row " + i + ": ");
            for (int j = 0; j < jaggedArray[i].Length; j++)
            {
                Console.Write(jaggedArray[i][j] + " ");
            }
            Console.WriteLine();
        }

  
        Console.WriteLine("\nRectangular Array:");
        for (int i = 0; i < rectangularArray.GetLength(0); i++)
        {
            Console.Write("Row " + i + ": ");
            for (int j = 0; j < rectangularArray.GetLength(1); j++)
            {
                Console.Write(rectangularArray[i, j] + " ");
            }
            Console.WriteLine();
        }
    }
}
