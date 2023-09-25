# 02-01-01-circle

Készítsen osztályt kör objektumok kezelésére. Az osztályt a Models rétegben hozza létre. A kör létrehozásakor meg kell adni a sugarát. A sugár módosítható tulajdonság legyen. A kör osztályban a terület és a kerület leolvasható tulajdonság legyen. Ha a kör adatait karakterlánccá alakítja, akkor felhasználóbarát módon jelenítse meg a kör sugarát, területét és kerületét.
Példányosítson két kört és a nagyobb területű körnek jelenítse meg a kerületét!  

A Program.cs kódja:
```
            Circle c1 = new Circle(2.25);
            Console.WriteLine(c1);
            Circle c2 = new Circle(4);
            c2.Radius = 4.05;
            Console.WriteLine(c2);

            if (c1.Area > c2.Area)
                Console.WriteLine("A nagyobb területű kör kerülete:" + c1.Perimeter);
            else if (c2.Area > c1.Area)
                Console.WriteLine("A nagyobb területű kör kerülete:" + c2.Perimeter);
            else
                Console.WriteLine("A két kör területe megegyezik! Kerületük: " + c1.Perimeter);

```

A teszt kód a következő kimenetet adja:
```
2,25 sugarú kör területe 15,9, kerülete 14,14.
4,05 sugarú kör területe 51,53, kerülete 25,45.
A nagyobb területű kör kerülete: 25,446900494077322
```
[második rész]  
Biztosítsa, hogy negatív vagy nulla sugarú kört ne lehessen létrehozni. A sugár módosításakor se lehessen negatív vagy nulla sugarú kört megadni. Ilyen anomália keletkezésekor dobjon saját kivételt! A kivétel neve legyen *ExceptionCircleRadiusNegativOrZero*!
Kivételkezeléssel biztosítsa, hogy a kivétel legyen elkapva, a kivétel üzenete az outputon is legyen olvasható!  
