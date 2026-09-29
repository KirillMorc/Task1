# Task1
using System; using System.Collections.Generic; using System.Linq; using System.Text; using System.Threading.Tasks;

namespace ConsoleApp2

{ internal class Program { static bool Foo() => true; static void Main(string[] args)

    {
        #region   Блок 1

        // Задача 1: x = 17 / 5; y = 17 % 5;
        int x = 17 / 5;
        int y = 17 % 5;
        Console.WriteLine($"Задача 1: x = {x}, y = {y}");

        // Задача 2: ++a * 2
        int a = 5;
        int res = ++a * 2;
        Console.WriteLine($"Задача 2: res = {res} (a = {a})");

        // Задача 3: a++ * 2
        int a2 = 5;
        int res2 = a2++ * 2;
        Console.WriteLine($"Задача 3: res = {res2} (a = {a2})");

        // Задача 4: 7 / 2 и 7.0 / 2
        int divInt = 7 / 2;
        double divDouble = 7.0 / 2;
        Console.WriteLine($"Задача 4: {divInt}, {divDouble}");

        // Задача 5: -15 % 4
        int remNegative = -15 % 4;
        Console.WriteLine($"Задача 5: {remNegative}");

        // Задача 6: x = x++ + ++x
        int x2 = 10;
        x2 = x2++ + ++x2;
        Console.WriteLine($"Задача 6: x2 = {x2}");

        // Задача 7: checked(max + 1)
        //int max = int.MaxValue;
        //int res1 = checked(max + 1);

        //Задача 8:unchecked(max + 1)
        int max1 = int.MaxValue;
        int res3 = unchecked(max1 + 1);
        res3 = int.MinValue;

        // Задача 9: 1.0 / 0.0 и 0.0 / 0.0
        double inf = 1.0 / 0.0;
        double nan = 0.0 / 0.0;
        Console.WriteLine($":{inf}, {nan}");

        // Задача 10: a - b * 2 + a / b
        int a1 = 8, b = 3;
        int c = a1 - b * 2 + a1 / b;
        Console.WriteLine($" {a1} - {b * 2} + {a1 / b} = 4");
        #endregion

        #region  Блок 2
        // Задача 1: 5 > 3 и 5 >= 5
        bool comp1 = 5 > 3;
        bool comp2 = 5 >= 5;
        Console.WriteLine($"Задача 1: {comp1}, {comp2}");

        // Задача 2: "hello" == "hello"
        bool strEqual = "hello" == "hello";
        Console.WriteLine($"Задача 2: {strEqual}");

        // Задача 3: double.NaN == double.NaN
        bool nanEqual = double.NaN == double.NaN;
        Console.WriteLine($"Задача 3: {nanEqual}");

        // Задача 4: object a == object b
        object objA = new int[] { 1 };
        object objB = new int[] { 1 };
        bool objEqual = objA == objB;
        Console.WriteLine($"Задача 4: {objEqual}");

        // Задача 5: 10 != 10.0
        bool doubleEqual = 10 != 10.0;
        Console.WriteLine($"Задача 5: {doubleEqual}");

        // Задача 6: null == null
        bool nullComp = null == null;
        Console.WriteLine($"Задача 6: {nullComp}");

        // Задача 7: (3 < 5) == (10 >= 20)
        bool exprComp = (3 < 5) == (10 >= 20);
        Console.WriteLine($"Задача 7: {exprComp}");

        // Задача 8: 4 <= 4 && 5 > 2
        bool resAnd = 4 <= 4 && 5 > 2;
        Console.WriteLine($"Задача 8: {resAnd}");

        // Задача 9: 'b' > 'a'
        char c2 = 'b';
        bool charComp = c2 > 'a';
        Console.WriteLine($"Задача 9: {charComp}");

        // Задача 10: -0.0 == 0.0
        bool zeroComp = -0.0 == 0.0;
        Console.WriteLine($"Задача 10: {zeroComp}");
        #endregion

        #region   Блок 3
        // Задача 1: !true || false && true
        bool logic1 = !true || false && true;
        Console.WriteLine($"Задача 1: {logic1}");

        // Задача 2: false && Foo()
        bool logic2 = false && Foo();
        Console.WriteLine($"Задача 2: {logic2}");

        // Задача 3: false & Foo()
        bool logic3 = false & Foo();
        Console.WriteLine($"Задача 3: {logic3}");

        // Задача 4: true ^ false ^ true
        bool logic4 = true ^ false ^ true;
        Console.WriteLine($"Задача 4: {logic4}");

        // Задача 5: !(5 > 2 || 3 < 1)
        bool logic5 = !(5 > 2 || 3 < 1);
        Console.WriteLine($"Задача 5: {logic5}");

        // Задача 6: a && !b || b && !a
        bool a6 = true, b26 = false;
        bool logic6 = a6 && !b26 || b26 && !a6;
        Console.WriteLine($"Задача 6: {logic6}");

        // Задача 7: true || (x / 0 == 1)
        int x7 = 5;
        bool logic7 = true || (x7 / 0 == 1);
        Console.WriteLine($"Задача 7: {logic7}");

        // Задача 8: false & (10 / 0 == 1) -> вызовет исключение
        bool logic8 = false & (10 / 1 == 1);
        Console.WriteLine(logic8);

        // Задача 9: Законы де Моргана
        bool A = true, B = false;
        bool deMorgan1 = !(A && B) == (!A || !B);
        Console.WriteLine($"Задача 9.1: {deMorgan1}");
        bool deMorgan2 = !(A || B) == (!A && !B);
        Console.WriteLine($"Задача 9.2: {deMorgan2}");

        // Задача 10: 5 & 3
        int bitAnd = 5 & 3;
        Console.WriteLine($"Задача 1: {bitAnd}");
        #endregion

        #region   Блок 4
        // Задача 1: 5 | 3
        int bitOr = 5 | 3;
        Console.WriteLine($"{bitOr}");

        // Задача 2: 5 ^ 3
        int bitXor = 5 ^ 3;
        Console.WriteLine($"Задача 3: {bitXor}");

        // Задача 3: ~0
        int bitNot = ~0;
        Console.WriteLine($"Задача 4: {bitNot}");

        // Задача 4: 1 << 4
        int bitShift = 1 << 4;
        Console.WriteLine($"Задача 5: {bitShift}");

        // Задача 5: 40 >> 2
        int bitShiftRight = 40 >> 2;
        Console.WriteLine($"Задача 6: {bitShiftRight}");

        // Задача 6: Проверка 3-го бита (n & (1 << 3))
        int n37 = 15;
        bool hasBit3 = (n37 & (1 << 3)) != 0;
        Console.WriteLine($"Задача 7: {hasBit3}");

        // Задача 7: Установка 2-го бита
        int n38 = 0;
        n38 |= (1 << 2);
        Console.WriteLine($"{n38}");

        // Задача 8: Сброс 4-го бита
        int n39 = 16;
        n39 &= ~(1 << 4);
        Console.WriteLine($"З{n39}");

        // Задача 9: (-16) >> 2
        int bitShiftNegative = (-16) >> 2;
        Console.WriteLine($"{bitShiftNegative}");

        // Задача 10: x += 5
        int x1 = 5;
        x1 += 5;
        Console.WriteLine($"{x1}");
        #endregion

        #region  Блок 5
        // Задача 1: a *= 2 + 3
        int a3 = 10;
        a2 *= 2 + 3;
        Console.WriteLine($"{a2}");

        // Задача 2: x >>= 2
        int x3 = 12;
        x3 >>= 2;
        Console.WriteLine($"{x3}");

        // Задача 3: x ??= y
        int? x4 = null;
        x4 = 42;
        Console.WriteLine($"{x4}");

        // Задача 4: str ??= "default"; str ??= "custom";
        string str = null;
        str = str ?? "default";
        str = str ?? "custom";
        Console.WriteLine($"{str}");

        // Задача 5: byte b = 1; b += 2;
        byte b6 = 1;
        b6 += 2;
        Console.WriteLine($"{b6}");

        // Задача 6: c = a = b;
        int a7 = 5, b7 = 10, c7 = 0;
        c7 = a7 = b7;
        Console.WriteLine($"{c7}");

        // Задача 7: mask <<= 3; mask |= 2;
        int mask = 1;
        mask <<= 3;
        mask |= 2;
        Console.WriteLine($"{mask}");

        // Задача 8: x %= 4;
        int x9 = 15;
        x9 %= 4;
        Console.WriteLine($"{x9}");

        // Задача 9: x ^= 7;
        int x10 = 7;
        x10 ^= 7;
        Console.WriteLine($"Задача 10: {x10}");

        // Задача 10: score >= 60 ? "Pass" : "Fail"
        int score = 75;
        string res4 = score >= 60 ? "Pass" : "Fail";
        Console.WriteLine($"Задача 1: {res4}");
        #endregion

        #region  Блок 6
        // Задача 1: (x > 10) ? 100 : (x > 2) ? 50 : 0
        int x5 = 5;
        int y1 = (x5 > 10) ? 100 : (x5 > 2) ? 50 : 0;
        Console.WriteLine($"Задача 2: {y1}");

        // Задача 2: true ? 10 : 15.5
        var task3Result = true ? 10 : 15.5;
        Console.WriteLine($"Задача 3: {task3Result.GetType().Name}");

        // Задача 3: s?.Length
        string s4 = null;
        Console.WriteLine($"Задача 4: {s4?.Length}");

        // Задача 4: Тип s?.Length
        string s5 = null;
        Type typeOfLength = typeof(int?);
        Console.WriteLine($"Задача 5: {typeOfLength}");

        // Задача 5: name ?? "Anonymous"
        string name = null;
        string res6 = name ?? "Anonymous";
        Console.WriteLine($"Задача 6: {res6}");

        // Задача 6: a ?? b ?? c
        //string a4 = null, b2 = "User", c1 = "Admin";
        //string res7 = a ?? b ?? c1;
        //Console.WriteLine($"Задача 7: {res7}");

        // Задача 7: false ? (10 / 0) : 42
        int res8 = false ? (10 / 1) : 42;
        Console.WriteLine($"Задача 8: {res8}");

        // Задача 8: count?.GetHashCode() ?? -1
        int? count = null;
        int res10 = count?.GetHashCode() ?? -1;
        Console.WriteLine($"Задача 9: {res10}");

        //Задача 9: int? count = null; int res = count?.GetHashCode() ?? -1;
        //int? count = null;
        //int res = count?.GetHashCode() ?? -1;
        #endregion

        #region  Блок 7
        // Задача 1: obj is string
        object obj1 = "Hello";
        bool check1 = obj1 is string;
        Console.WriteLine($"Задача 1: {check1}");

        // Задача 2: obj as string
        object obj2 = 123;
        string s2 = obj2 as string;
        Console.WriteLine($"Задача 2: {(s2 == null ? "null" : s2)}");

        // Задача 3: (string)obj
        try
        {
            object obj3 = 123;
            string s3 = (string)obj3;
        }
        catch (InvalidCastException ex)
        {
            Console.WriteLine($"Задача 3: {ex.GetType().Name}");
        }

        // Задача 4: typeof(int) == typeof(Int32)
        Console.WriteLine($"Задача 4: {typeof(int) == typeof(Int32)}");

        // Задача 5: sizeof(long)
        Console.WriteLine($"Задача 5: {sizeof(long)}");

        // Задача 6: null is string
        Console.WriteLine($"Задача 6: {null is string}");

        // Задача 7: x is null
        object x8 = null;
        bool b8 = x8 is null;
        Console.WriteLine($"Задача 7: {b8}");

        // Задача 8: (int)3.99
        Console.WriteLine($"Задача 8: {(int)3.99}");

        // Задача 9: Pattern matching
        object o9 = 42;
        bool blockExecuted = false;
        if (o9 is int val && val > 40)
        {
            blockExecuted = true;
        }
        Console.WriteLine($"Задача 9: {blockExecuted}");

        // Задача 10: default(int) и default(string)
        int defInt = default(int);
        string defStr = default(string);
        Console.WriteLine($"Задача 10: {defInt}, {(defStr == null ? "null" : defStr)}");
        #endregion

        #region Блок 8
        Console.WriteLine("1: " + ((5 > 3) && !(10 <= 2) || (4 == 5)));
        Console.WriteLine("2: " + (!(true && false) ^ (true || false && false)));
        Console.WriteLine("3: " + ((10 & 6) == 2 && (10 | 6) == 14));
        Console.WriteLine("4: " + ((15 >> 1 == 7) && (7 << 2 == 28)));
        Console.WriteLine("5: " + ((8 > 5) && (3 + 2 * 4 == 11) && !(false || !true)));
        Console.WriteLine("6: " + ((true || false) && (false || true) ^ (true && !false)));
        Console.WriteLine("7: " + ((100 / 10 == 10) && (100 % 30 == 10) && !(5 - 5 != 0)));
        Console.WriteLine("8: " + ((4 ^ 4) == 0 && (4 ^ 0) == 4 && (0 ^ 0) == 0));

        // В задании 9: (10 / 0 == 1) не вызовет ошибку, так как слева true, сработает короткое замыкание
        Console.WriteLine("9: " + (!(5 != 5) && ((3 >= 3) || (10 / 1 == 1))));

        // В задании 10: false && (...) не вызовет ошибку из-за короткого замыкания
        Console.WriteLine("10: " + ((false && (10 / 1 == 1)) || (true && (20 > 15))));

        Console.WriteLine("11: " + ((12 & 10) > 5 || (12 | 10) < 15 && !(3 == 3)));
        Console.WriteLine("12: " + (((20 >> 2) == 5) ^ ((5 << 1) == 11)));
        Console.WriteLine("13: " + (!(!(true || false) && (true && !false))));
        Console.WriteLine("14: " + ((7 > 2 ? 10 : 20) == 10 && (3 < 1 ? 5 : 15) == 15));
        Console.WriteLine("15: " + ((5 & 1) == 1 && (6 & 1) == 0 && (7 & 1) == 1));
        Console.WriteLine("16: " + (((10 > 5 ? true : false) ^ (3 > 8 ? true : false)) && !false));
        Console.WriteLine("17: " + (!((5 > 2 && 10 > 20) || (3 == 3 && 4 <= 4))));
        Console.WriteLine("18: " + (((1 << 3) == 8) && ((16 >> 4) == 1) && ((2 << 2) == 8)));
        Console.WriteLine("19: " + (((10 & 7) == 2) || ((10 | 7) == 15) ^ !(4 > 1)));
        Console.WriteLine("20: " + (false || true && false || true && !false));
        Console.WriteLine("21: " + ((25 % 4 == 1) && (17 / 3 == 5) && (17 % 3 == 2)));
        Console.WriteLine("22: " + (((5 ^ 3 ^ 3) == 5) && ((10 ^ 0) == 10)));
        Console.WriteLine("23: " + ((true ? (false ? 1 : 2) : (true ? 3 : 4)) == 2));
        Console.WriteLine("24: " + (!(true && !(false || !false))));
        Console.WriteLine("25: " + (((~0 == -1) && (~(-1) == 0))));
        Console.WriteLine("26: " + (((8 & 4) == 0) && ((8 | 4) == 12) && ((8 ^ 4) == 12)));
        Console.WriteLine("27: " + (!(10 >= 10) || (5 < 3) && (2 == 2) || !(false)));
        Console.WriteLine("28: " + (((15 & ~1) == 14) && ((14 | 1) == 15)));
        Console.WriteLine("29: " + (((true || false) ? (false && true ? 10 : 20) : 30) == 20));
        Console.WriteLine("30: " + (((10 > 2) && (5 < 9)) ^ (!(4 >= 5) && (6 != 7))));
        Console.WriteLine("31: " + ((7 & 3 & 1) == 1 && (7 | 3 | 1) == 7));
        Console.WriteLine("32: " + (((10 > 5 && 3 < 1) || (8 == 8 && !(5 > 10))) && (4 + 4 == 8)));
        Console.WriteLine("33: " + (!((!(true && false) || !(true || false)) && !false)));
        Console.WriteLine("34: " + (((32 >> 3 == 4) && (4 << 3 == 32)) ^ ((15 & 7) == 7 && (15 | 7) == 15)));
        Console.WriteLine("35: " + (((5 > 3 ? (2 > 1 ? true : false) : false) && !((10 > 20) || (30 < 15)))));
        #endregion




    }
}
}
