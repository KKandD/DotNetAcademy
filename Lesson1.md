1. Czym jest programowanie:
    Programowanie jest procesem tworzenia zbioru instrukcji,
    które mówią komputerowi jak wykonać określone zadanie.

    Programowanie obiektowe to paradygmat programowania,
    który opiera się na tworzeniu struktur zwanych obiektami,
    posiadającymi własne cechy (atrybuty) oraz zachowania (metody).

2. Dlaczego C# i .NET:
    https://dotnet.microsoft.com/en-us/platform/why-choose-dotnet

3. Historia .NET'a:
    https://time.graphics/line/593132

4. Visual Studio:

5. 
    TYP   ROZMIAR OPIS
    sbyte	8	-128 do 127
    short	16	od -32 768 do 32 767.
    int	32	od -2,147,483,648 do 2 147 483 647
    long	64	–9, 223, 372, 036, 854, 775 808 do 9,223,372,036,854,775,807
    byte	8	Od 0 do 256
    ushort	16	0 do 65 535.
    uint	32	0 do 4 294 967 295
    ulong	64	0 do 18,446,744,073,709,551,615. Jedna z najlepszych możliwości do przechowywania dużych pozytywnych liczb całkowitych.
    float	32	Liczby zmiennoprzecinkowe.
    double	64	Liczby zmiennoprzecinkowe.
    decimal	128	Większa precyzja, ale mniejszy zakres. Wykorzystywany w aplikacjach finansowych
    char	16	Znaki unicode
    bool	4	Wartości logiczne

    const int bb = 10; // stała na poziomie kompilacji, nie może być modyfikowana
    var aa = "10" // Słowo var kluczowe instruuje kompilator, aby wywnioskował typ zmiennej z wyrażenia po prawej stronie instrukcji inicjowania.

    +, -, *, /, %, !, &&, ||, ==, !=, is, is not, <, >, <=, =>
    int z = 0;
    z++; // post-increment
    z--; // post-decrement
    ++z; // pre-increment
    --z; // pre-decrement

6. List, Array, Dictionary
    TABLICA JEDNOWYMIAROWA
        int[] h0;
        int[] h = new int[3];
        h[0] = 1;
        h[1] = 2;
        h[2] = 3;
        int[] h2 = new int[] {1,2,3};
        int[] h3 = {1,2,3};
        System.out.println(h[1] + h[2]);

    TABLICA WIELOWYMIAROWE
        string[,] x = new string[9, 7];
        x[0, 0] = "00"; x[0, 1] = "01";
        x[1, 0] = "10"; x[1, 1] = "11";
        string[,] y = { { "00", "01" }, { "10", "11" } };

7. 

    SWITCH
        string day = "Friday";
        switch (day)
        {
            case Monday: System.Console.Write("Today is Monday"); break;
            case Tuesday: System.Console.Write("Today is Tuesday"); break;
            case Wednesday: System.Console.Write("Today is Wednesday"); break;
            case Friday:
                System.Console.Write("Today we drink");
                break;
            default: System.Console.Write("Are you still drunk?");
                    break;
        }

        DO WYKONA SIĘ CHOCIAŻ RAZ, W WHILE WARUNEK JEST SPRAWDZANY PRZED ROZPOCZĘCIEM
        while (i < 5) { System.Console.Write(i++); }
        do { System.Console.Write(i++); } while (i < 10);

        BREAK, CONTINUE w pętlach

9. Metody, Class, Interface, static, public, private, sealed, namespace

    METODY
        Coś zwracają przy użyciu RETURN chyba że void,
        Mogą przyjmować wiele parametrów,
        Opcjonalne parametry,

    KLASA
        Jest to szablon używany do tworzenia obiektów.
        Inicjalizacja przy użyciu słowa new,
        Klasa może mieć wiele konstruktorów
        Klasa może być statyczna, nie trzeba jej inicjalizować
        Klasa może dziedziczyć po jednej klasie za to może dziedziczyć wiele interfejsów

    INTERFEJS
        Jest to specyficzny kontrakt, który jest implementowany przez klasy.
        Kontrakt ten zawiera tylko informacje o co dana metoda ma się zwrócić i co ma ona przyjąć.
        Definicja działania jest już określona w klasie.

        public, = wszędzie dostępny
        protected, = dostępny na poziomie klasy lub klasy pochodnej
        internal, = dostępny na poziomie biblioteki
        protected internal, = dostępny na poziomie klasy lub klasy pochodnej lub wewnątrz biblioteki
        private. = dostępny tylko dla klasy


10. Zadanie domowe:
    kalkulator? Stworzyć repo w Git i udostępnić

    TIP DO UŻYCIA GITA
        Your Identity
        The first thing you should do when you install Git is to set your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating:

        $ git config --global user.name "John Doe"
        $ git config --global user.email johndoe@example.com
        Again, you need to do this only once if you pass the --global option, because then Git will always use that information for anything you do on that system. If you want to override this with a different name or email address for specific projects, you can run the command without the --global option when you’re in that project.

        Many of the GUI tools will help you do this when you first run them.
