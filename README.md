# Uitilities Extension Packages

 
![Plugin Banners](https://github.com/user-attachments/assets/1147e680-7be5-4845-87f9-795f1615993c)


## C#_extensions #
A C# package that provides handy extensions and helper functions, designed to simplify and speed up development, making coding more efficient and streamlined.

## Types of Extensions #
```
📊  Web Utils
📅  Date Handling
✍️  String Utilities
📋  File Enhancements
🎨  Color Conversion
🔢  Number Utilities
🛠  Int Extensions
 ```
## Usage
- Set the desired password length.
- Customize the inclusion of these character types.

```
public class Program
{
    public static void Main(string[] args)
    {
       
        var passwordBuilder = new PasswordBuilder()
           .WithLength(12)
           .WithLowercase()
           .WithUppercase()
           .WithNumbers()
           .WithSymbols();

        string password = passwordBuilder.Generate();
        Console.WriteLine($"Generated Password: {password}");

        var passwordGroup = passwordBuilder.GenerateMultiple(5);
        Console.WriteLine("Batch Generated Passwords:");
        foreach (var pwd in passwordGroup)
        {
            Console.WriteLine(pwd);
        }


    }

}


