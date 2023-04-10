# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
## Step 1:
Start the C# program in visual studio 2022.

## Step 2:
Declare a Jagged Array for four element.

## Step 3:
Initialize the elements.

## Step 4:
Accessing the elements.

## Step 5:
Finish the program and Run the prgram.

## Program:
using System;
class CPUactivity
{
    public static void Main(String[] args)
    {
        int[][] cpu = new int[4][];
        cpu[0] = new int[3];
        cpu[1] = new int[5];
        cpu[2] = new int[6];
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
                Console.WriteLine("CPU usage at node" + i + " is " + cpu[i][j] );

                Console.WriteLine();
            }
        }
    }
}


## Output:

![Screenshot 2023-04-10 143423](https://user-images.githubusercontent.com/94828147/230871564-0c878ae9-a211-467b-be97-a844d3402869.png)


## Result:

Thus, the C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
