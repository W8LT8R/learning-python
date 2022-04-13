## 1.2.2 Python is expressive

Python is a very expressive language. Expressive in this context means that a single line of Python code can do more than a single line of code in most other languages. The advantages of a more expressive language are obvious: The fewer lines of code you have to write, the faster you can complete the project. The fewer lines of code there are, the easier the program will be to maintain and debug.

To get an idea of how Python’s expressiveness can simplify code, consider swapping the values of two variables, var1 and var2 . In a language like Java, this requires three lines of code and an extra variable:

```java
// Java

int temp = var1;
var1 = var2;
var2 = temp;

```

The variable temp is needed to save the value of var1 when var2 is put into it, and then that saved value is put into var2 . The process isn’t terribly complex, but reading those three lines and understanding that a swap has taken place takes a certain amount of overhead, even for experienced coders.

By contrast, Python lets you make the same swap in one line and in a way that makes it obvious that a swap of values has occurred:

``` Python
# Python

var2, var1 = var1, var2

```

Of course, this is a very simple example, but you find the same advantages throughout the language.

## 1.2.3 Python is readable

Another advantage of Python is that it’s easy to read. You might think that a programming language needs to be read only by a computer, *but humans have to read your code as well: whoever debugs your code (quite possibly you), whoever maintains your code (could be you again), and whoever might want to modify your code in the future. In all of those situations, the easier the code is to read and understand, the better it is.*

The easier code is to understand, the easier it is to debug, maintain, and modify. Python’s main advantage in this department is its use of indentation. Unlike most languages, **Python insists that blocks of code be indented**. Although this strikes some people as odd, it has the benefit that your code is always formatted in a very easy-to-read style.

Following are two short programs, one written in Perl and one in Python. Both take two equal-size lists of numbers and return the pairwise sum of those lists. I think the Python code is more readable than the Perl code; it’s visually cleaner and contains fewer inscrutable symbols:

``` Perl

# Perl version.
sub pairwise_sum {
  my($arg1, $arg2) = @_;
  my @result;
  
  for(0 .. $#$arg1) {
    push(@result, $arg1->[$_] + $arg2->[$_]);
  }
  
  return(\@result);
}

```

``` Python

# Python version.
def pairwise_sum(list1, list2):
  result = []

  for i in range(len(list1)):
    result.append(list1[i] + list2[i])

  return result

```

Both pieces of code do the same thing, but the Python code wins in terms of readability. (There are other ways to do this in Perl, of course, some of which are much more concise but in my opinion harder to read—than the one shown.)