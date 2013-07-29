Hi!

This is a little porject made by me . It´s about change parameters in a string. 
This is something like to change the {1}, {2} in a string, 
but using the same marks and an array as parameters, 
and you can tell since which index you want to start to change the string.

You can download the .dll from Github and use it. It´s free!

What we need: We need to mark the places with “{-}”. 
This symbols will be changed with our parameters.

In C# you can use:

string name = "Oscar"
Console.WriteLine("Hello {1}!", name);

The output will be:

Hello Oscar!

I wanted to do something liek this, but taking a array, something like this:

string[] temp = { "Oscar", "Bralo", "28"};
parameterString p = new parameterString();
string result = p.paramString("Hi, my name is {-} {-}, and I am {-} years old", temp, 0);
Console.WriteLine(result);

The output will be:

"Hi, my name is Oscar Bralo, and I am 28 years old"