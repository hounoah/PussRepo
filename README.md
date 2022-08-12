# PussRepo
The goal is to take a powershell script and invoke it with C#...

The documentation that I gathered is that we add a script using Powershell.Create() .AddCommand("<script gose here>")
However I still can not get the actual powershell window to come up. 
Example:

/* using (PowerShell powershell = PowerShell.Create().AddCommand("get-process")) <------- [This line is going to be our main usage]
{
    Console.WriteLine("PowerShell is loading");
    Console.Write("--------------------------------");

    // Invoke the command synchronously and display the  
    // ProcessName and HandleCount properties of the 
    // objects that are returned.
    foreach (PSObject result in powershell.Invoke())
    {
        Console.WriteLine(
                    "{0,-20} {1}",
                    result.Members["ProcessName"].Value,
                    result.Members["HandleCount"].Value);
    }
}

System.Console.WriteLine("Hit any key to exit...");
System.Console.ReadKey();

*/

