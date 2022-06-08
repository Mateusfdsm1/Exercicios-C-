//Desenvolver um sistema que quando a nota de um aluno for menor que 60, o sistema vai escrever REPROVADO//

using System;
using System.Globalization;

namespace Exercicio
{
    class Program
    {
        static void Main(string[] args)
        {
            double nota1, nota2, NF;

            nota1 = double.Parse(Console.ReadLine(), CultureInfo.InvariantCulture);
            nota2 = double.Parse(Console.ReadLine(), CultureInfo.InvariantCulture);

            NF = nota1 + nota2;

            if (NF >= 60)
            {
                Console.WriteLine("NOTA FINAL = " + NF.ToString("F1", CultureInfo.InvariantCulture));
            }
            else
            {
                Console.WriteLine("NOTA FINAL = " + NF.ToString("F1", CultureInfo.InvariantCulture));    
                Console.WriteLine("REPROVADO ");
            }            
        }
    }
}
