using System;
using System.IO;

namespace archivo
{
    class Program
    {
        static void Main(string[] args)
        {
            // crear un archivo de texto
            TextWriter archivo;
            archivo = new StreamWriter("K020.text");
            string mensaje;
            Console.WriteLine("Introduce un mensaje");
            mensaje = Console.ReadLine();
            archivo.WriteLine(mensaje);
            archivo.Close();
            Console.WriteLine("Texto guardado");
            Console.ReadKey();
        }
    }
}
