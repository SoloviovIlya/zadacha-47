//Задайте двумерный массив размером m×n, заполненный случайными вещественными числами.

//m = 3, n = 4.

//0,5 7 -2 -0,2

//1 -3,3 8 -9,9

//8 7,8 -7,1 9

Console.WriteLine("Введите количество строк: ");

int m = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Введите количество столбцов: ");

int n = Convert.ToInt32(Console.ReadLine());

double[,] a = new double[m,n];

for (int i = 0; i < m;i++)

{

    for (int j =0; j<n; j++)
    
    {
    
        a[i,j] = new Random().Next(-10,11);
        
        Console.Write(string.Format("{0} ", a[i, j]));
        
    }
    
    Console.Write(Environment.NewLine + Environment.NewLine);
    
}
