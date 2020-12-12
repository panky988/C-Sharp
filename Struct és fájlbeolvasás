// A fájl tartalma:
//Peti;23;Budapest
//Gabi;14;Szeged
//Kata;43;Szolnok
//János;27;Keszthely
//-----------------------------

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
        struct szemelyek //felvesszük a struktúrát
        {
            public string nev;
            public int kor;
            public string varos;
        }
        static void Main(string[] args)
        {
            int i = 0; //sorok létetésére használjuk
            szemelyek[] adatok = new szemelyek[1000]; //tegyük fel, hogy a fájl 1000 sort tartalmaz
            StreamReader olvas = new StreamReader("szoveg.txt", Encoding.UTF8); //Fájlbeolvasás + UTF8 kódolás
            while (!olvas.EndOfStream) //fut az olvasás, amíg nem ér a végére
            {
                string egysor = olvas.ReadLine(); //egy sor beolvasása
                string[] egysordarabolva = egysor.Split(';'); //az egysor feldarabolása ';'-vel
                adatok[i].nev = egysordarabolva[0]; //eltároljuk a nevet
                adatok[i].kor = Convert.ToInt32(egysordarabolva[1]); //eltároljuk a kort
                adatok[i].varos = egysordarabolva[2]; //eltároljuk a várost
                i++; //léptetés
            }
            olvas.Close(); //olvasás bezárása
            int db = i; //a sorok száma lesz a db, így az i felszabadul léptetésnek
            Console.WriteLine(db + "db sor van a fájlban.");
            Console.ReadKey();
        }
    }
}
