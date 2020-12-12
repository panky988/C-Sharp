using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.IO; //fájlbeolvasáshoz szükséges

namespace Program1
{
    class Program
    {
        static void Main(string[] args)
        {
            int i = 0; //sorok létetésére használjuk
            string[] autok = {"Mazda", "Ford", "Suzuki", "Honda"};
            StreamWriter kiir = new StreamWriter("szoveg.txt"); //Fájlkiírás
            for(i=0;i<autok.Length;i++) //léptetjük i-vel az autok tömb végéig
            {
                kiir.WriteLine("{0}. {1}", i+1, autok[i]); //kiiratás soronként
            }
            kiir.Close(); //kiírás bezárása
            Console.ReadKey();
        }
    }
}
