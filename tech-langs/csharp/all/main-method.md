# Main method

C# recognizes a static method called `Main` as signaling the default entry point of execution.

Optionally, `Main` may
- return a `ubyte` to indicate error code to system environment
- accept an array of strings as *argv* parameter


The `Main` method may optionally return an integer (rather than void) in order
to return a value to the execution environment (zero for successful execution or intigers bigger then zero for misc errors. There is no agreed upon convention how to interpred these error codes - one must consult program's doumentation. If a program is CLI, one possible way to get the explanation of program's error codes, is to run it with a `--help` switch).

The `Main` method can also optionally accept an array of strings as a parameter. This array will be populated with any arguments passed to the executable, with the element 0 being the name of the program.

```cs
class Example {
  static void Main(string[] args) {
    System.Console.WriteLine (FeetToInches (30));
    System.Console.WriteLine (FeetToInches (100));
  }

  static int FeetToInches (int feet) {
    int inches = feet * 12;
    return inches;
  }
}
```
