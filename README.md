<div align="center">
    <h1> The T# Programming Language</h1>
</div>

[![T# Build](https://github.com/ibukiyoshidaa/Tsharp/actions/workflows/tsharp-ci.yml/badge.svg)](https://github.com/ibukiyoshidaa/Tsharp/actions/workflows/tsharp-ci.yml)

WARNING! THIS LANGUAGE IS A WORK IN PROGRESS! ANYTHING CAN CHANGE AT ANY MOMENT WITHOUT ANY NOTICE!

<!---- Compile to C. ---->

### Install

> Install
```
$ make

If it doesn't work, run the next command

$ gcc -o tsharp.exe src/*.c
```

### Run

> Run
```
$ ./tsharp.out <filename>.t#

or

$ ./tsharp.exe <filename>.t#
```

> Hello World
```pascal
func main() do
    print("Hello World");
end;
```

> Function call
```pascal
func SampleFunc() do
    print("Function call!");
end;

func main() do
    SampleFunc();
end;
```

> Variable
```pascal
func main() do
    name = "T#";
    print(name);
end;
```

> Call variables from other functions
```pascal
func SampleFunc() do
    name = "T#";
end;

func main() do
    SampleFunc();
    print(SampleFunc.name);
end;
```

> If statement
```pascal
func main() do
    if 10 == 10 do
        print("Hello World!");
    end;

    if 10 != 10 do
        print("Hello World!");
    else
        print("T# Programming Language");
    end;

    if 3 < 2 do
        print("Hello World!");
    end;

    if 3 > 2 do
        print("Hello World!");
    end;

    if ("Foo" == "Foo") == ("T#" == "T#") do
        print("T# Programming Language!");
    end;
end;
```

> While loop
```pascal
func main() do
    num = 0;
    while num < 101 do
        print(num);
        num++;
    end;
end;
```

> FizzBuzz
```pascal
func main() do
    i = 1;
    while i < 101 do
        if (i % 15) == 0 do
            print("FizzBuzz");
        elif (i % 3) == 0 do
            print("Fizz");
        elif (i % 5) == 0 do
            print("Buzz");
        else
            print(i);
        end;
        i++;
    end;
end;
```

### Vim Syntax Highlighting
- <a href="https://github.com/ibukiyoshidaa/Tsharp/blob/main/editor/tsharp.vim">Vim</a>


### Contributors

<a href="https://github.com/ibukiyoshidaa/Tsharp/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ibukiyoshidaa/Tsharp" />
</a>
