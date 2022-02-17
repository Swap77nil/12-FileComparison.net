# 12-FileComparison.net
//C# Program to Perform File Comparison.//<br>
using System;<br>
using System.IO;<br>
namespace Exercises<br>
{<br>
 class FileRead<br>
 {<br>
 public static void Main()<br>
 {<br>
 string file1;<br>
 string file2;<br>
 Console.Write("Enter the first file path:");<br>
 file1 = Console.ReadLine();<br>
 Console.Write("Enter the second file path:");<br>
 file2 = Console.ReadLine();<br>
 if (!File.Exists(file1))<br>
 {<br>
 Console.WriteLine("First file does not exist!");<br>
 }<br>
 else if (!File.Exists(file2))<br>
 {<br>
 Console.WriteLine("Second file does not exist!");<br>
 }<br>
 else if (File.ReadAllText(file1) == File.ReadAllText(file2))<br>
 {<br>
 Console.WriteLine("Both files contain the same content");<br>
 }<br>
 else<br>
 {<br>
 Console.WriteLine("Contents of files are not same");<br>
 }<br>
 }<br>
 }<br>
}<br>
