Console.Write("Az intervallum also vegpontja: ");
int alj = int.Parse(Console.ReadLine());

Console.Write("Az intervallum felso vegpontja: ");
int fent = int.Parse(Console.ReadLine());

int paros = 0;

for (int i = alj; i <= fent; i++)
{
    if (i % 2 == 0)
    {
        paros = paros + i;
    }
}
Console.WriteLine($"A paros szamok osszege: {paros}");

Console.Write("Add meg a csoki gyartasi sorszamat: ");
int gyszam = int.Parse(Console.ReadLine());

if (gyszam <= 1)
{
    Console.WriteLine("Sajnálom nem nyert!");
}
bool igaz = true;
if (gyszam > 1) {
    for (int i = 2; i * i <= gyszam; i++)
    {
        Console.WriteLine("Nem léptem be");
        if (gyszam % i == 1)
        {
            Console.WriteLine("Beléptem");
            igaz = false;
            break;
        }
        ;
    }
    ;
}

if (igaz == true)
{
    Console.WriteLine("Gratulalok, nyertel!");
}
else
{
    Console.WriteLine("Sajnos nem nyert!");
}

for (int sor = 1; sor <= 10; sor++)
{
    for (int oszlop = 1; oszlop <= 10; oszlop++)
    {
        Console.Write(sor * oszlop + " ");
    }

    Console.WriteLine();
}