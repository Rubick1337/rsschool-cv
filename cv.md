# Name and surname

Aleksey Gusev.

![avatar](images/photo_2023-10-26_17-26-17.jpg)

# Contacts for communication

- mail - poss1337@gmail.com,
- discord - Тактика 212 #2621,
- phone number - +375(33) 694-53-96,
- telegram - @AlexeyGuse.

# Brief information about yourself

I want to learn programming languages, create interesting projects and learn everything new because it's very interesting for me.

# Skills

I know programming languages c# and a little python. Worked on the framework .Net version 6.0. The development tools I used: pycharm and Visual Studio.

# Code Examples

```C#
using System;

class Program
{
    static int[,] InputArray(int str, int stolb)
    {
        int[,] array = new int[str, stolb]; ;
        Random random = new Random();
        for (int i = 0; i < array.GetLength(0); i++)
        {
            for (int j = 0; j < array.GetLength(1); j++)
            {
                array[i, j] = random.Next(-10, 10);
            }
        }
        return array;
    }
    static void OutPutArray(int[,] array)
    {
        for (int i = 0; i < array.GetLength(0); i++)
        {
            for (int j = 0; j < array.GetLength(1); j++)
            {
                Console.Write($"\t{array[i, j]}");
            }
            Console.WriteLine();
        }
    }
    static int FindZeroElement(int[,] array)
    {
        int count = 0;
        for (int i = 0; i < array.GetLength(0); i++)
        {
            for (int j = 0; j < array.GetLength(1); j++)
            {
                if (array[i, j] == 0)
                {
                    count++;
                }
            }
        }
        return count;
    }
    static int[,] SwapStr(int[,] array)
    {
        int str1 = 0;
        int str2 = 0;
        if (array.GetLength(0) % 2 == 0)
        {
            str1 = array.GetLength(0) / 2; // центр
            str2 = array.GetLength(0) / 2 - 1; // строчка под ней
        }
        else
        {
            str1 = array.GetLength(0) / 2; // центр
        }
        for (int j = 0; j < array.GetLength(0) - 1; j++)
        {
            int temp = array[str1, j];
            array[str1, j] = array[str2, j];
            array[str2, j] = temp;
        }
        return array;
    }
    static void Main()
    {
        Console.WriteLine("Введите кол-во строк.");
        int row = int.Parse(Console.ReadLine());
        Console.WriteLine("Введите кол-во столбцов.");
        int col = int.Parse(Console.ReadLine());
        int[,] array = InputArray(row, col);
        int[,] array_copy = new int[row, col];
        Array.Copy(array,array_copy,array.Length);
        Console.WriteLine("Кол-во нулевых элементов");
        Console.WriteLine(FindZeroElement(array));
        Console.WriteLine("Первоначальный массив");
        OutPutArray(array);
        Console.WriteLine("Переобразованный массив");
        SwapStr(array_copy);
        OutPutArray(array_copy);
    }
}
```

# Education

I am studying at the university.Specialization in Automated Information Processing Systems and Rss-school.

# Work experience

I have no work experience

# English language

English was taught at school and is taught at the university.

# My projects

- [Valentine-card](https://github.com/Rubick1337/Valentine-card)
- [Gallery](https://github.com/Rubick1337/Gallery)
- [VideoPlayer](https://github.com/Rubick1337/VideoPlayer)
- [Gallery](https://github.com/Rubick1337/Gallery)
- [Solar](https://github.com/Rubick1337/Course-work-on-the-web2)
