# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
### Step1:
```
Step1:
Start the program.

Step2:
Create a jagged array of 4arrays.

Step3:
Give the sample CPU usage in the jagged array.

Step4:
Print the sample CPU usage in the jagged array.

Step5:
End the program.
```

## Program:
```
using System;
namespace jagged_array
{
    class Program
    {
        static void Main(string[] args)
        {
            int[][] cpu = new int[4][];
            {
                cpu[0] = new int[3];
                cpu[1] = new int[2];
                cpu[2] = new int[2];
                cpu[3] = new int[4];
                for (int i = 0; i < 4; i++)
                {
                    for (int j = 0; j < cpu[i].Length; j++)
                    {
                        cpu[i][j] = i * j + 70;
                    }
                }
                for (int i = 0; i < cpu.Length; i++)
                {
                    for (int j = 0; j < cpu[i].Length; j++)
                    {
                        Console.WriteLine("CPU usage at node {0} is {1}", i, cpu[i][j]);
                    }
                    Console.WriteLine();
                }


            }


        }
    }
}
```

## Output:



![image](https://github.com/KathirvelAIDS/Ex05-Rec-JaggedArray/assets/94911373/bb7aa285-3d2a-4fae-a1ad-ba3bc61b617b)



## Result:


Thus,C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
