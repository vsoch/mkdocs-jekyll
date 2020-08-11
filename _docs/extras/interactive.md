---
title: Interactive Code Blocks
tags: 
 - jekyll
 - codefence
 - github
---

<link href="//codefence.io/codefence.css" rel="stylesheet">
<script defer type="text/javascript" src="//codefence.io/codefence.js"></script>

# Interactive Code Blocks

Thanks to <a href="https://codefence.io/" target="_blank">codefence</a> you can easily
embed interactive code snippets in your documentation! Note that we have added
the style and javascript file in <a href="https://github.com/vsoch/mkdocs-jekyll/blob/master/_docs/extras/interface.md" target="_blank">this template</a>,
that way we don't add extra code or styles to pages that don't need it.

# Examples

These are from the main codefence page. The goal is to show all the languages supported!
Heck, I bet there are a lot of new languages here!

## C


<code-fence lang="c" heading="Hello World from C">
<textarea vue-slot="code">
#include &lt;stdio.h&gt;

int main() {
    printf("Hello World from C");
    return 0;
}
</textarea>
</code-fence>

```html
<code-fence lang="c" heading="Hello World from C">
<textarea vue-slot="code">
#include &lt;stdio.h&gt;

int main() {
    printf("Hello World from C");
    return 0;
}
</textarea>
</code-fence>
```

## C++

<code-fence lang="cpp" heading="Hello World from C++">
<textarea vue-slot="code">
#include &lt;iostream&gt;

int main() {
    std::cout &lt;&lt; "Hello World from C++";
    return 0;
}
</textarea>
</code-fence>


```html
<code-fence lang="cpp" heading="Hello World from C++">
<textarea vue-slot="code">
#include &lt;iostream&gt;

int main() {
    std::cout &lt;&lt; "Hello World from C++";
    return 0;
}
</textarea>
</code-fence>
```

## C#


<code-fence lang="cs" heading="Hello World from C#">
<textarea vue-slot="code">
Console.WriteLine("Hello World from C#");
</textarea>
</code-fence>


```html
<code-fence lang="cs" heading="Hello World from C#">
<textarea vue-slot="code">
Console.WriteLine("Hello World from C#");
</textarea>
</code-fence>
```

## Clojure


<code-fence lang="clojure" heading="Hello World from Clojure">
<textarea vue-slot="code">
(ns main)
(defn -main [] (
  println "Hello World from Clojure")
)
</textarea>
</code-fence>

```html
<code-fence lang="clojure" heading="Hello World from Clojure">
<textarea vue-slot="code">
(ns main)
(defn -main [] (
  println "Hello World from Clojure")
)
</textarea>
</code-fence>
```

## Elixir

<code-fence lang="elixir" heading="Hello World from Elixir">
<textarea vue-slot="code">
IO.puts("Hello World from Elixir")
</textarea>
</code-fence>

```html
<code-fence lang="elixir" heading="Hello World from Elixir">
<textarea vue-slot="code">
IO.puts("Hello World from Elixir")
</textarea>
</code-fence>
```

## Crystal

<code-fence lang="crystal" heading="Hello World from Crystal">
<textarea vue-slot="code">
puts "Hello World from Crystal"
</textarea>
</code-fence>

```html
<code-fence lang="crystal" heading="Hello World from Crystal">
<textarea vue-slot="code">
puts "Hello World from Crystal"
</textarea>
</code-fence>
```

## Erlang

<code-fence lang="erlang" heading="Hello World from Erlang">
<textarea vue-slot="code">
-module(main).
-export([start/0]).

start() ->
    io:fwrite("Hello World from Erlang").
</textarea>
</code-fence>

```html
<code-fence lang="erlang" heading="Hello World from Erlang">
<textarea vue-slot="code">
-module(main).
-export([start/0]).

start() ->
    io:fwrite("Hello World from Erlang").
</textarea>
</code-fence>
```

## Asm

<code-fence lang="asm" heading="Hello World from GNU Assembly">
<textarea vue-slot="code">
    .global _start
    .text
_start:
    # write(1, message, 26)
    mov     $1, %rax                # system call 1 is write
    mov     $1, %rdi                # file handle 1 is stdout
    mov     $message, %rsi          # address of string to output
    mov     $26, %rdx               # number of bytes
    syscall                         # invoke operating system to do the write

    # exit(0)
    mov     $60, %rax               # system call 60 is exit
    xor     %rdi, %rdi              # we want return code 0
    syscall                         # invoke operating system to exit
message:
    .ascii  "Hello World from Assembly\n"
</textarea>
</code-fence>

```html
<code-fence lang="asm" heading="Hello World from GNU Assembly">
<textarea vue-slot="code">
    .global _start
    .text
_start:
    # write(1, message, 26)
    mov     $1, %rax                # system call 1 is write
    mov     $1, %rdi                # file handle 1 is stdout
    mov     $message, %rsi          # address of string to output
    mov     $26, %rdx               # number of bytes
    syscall                         # invoke operating system to do the write

    # exit(0)
    mov     $60, %rax               # system call 60 is exit
    xor     %rdi, %rdi              # we want return code 0
    syscall                         # invoke operating system to exit
message:
    .ascii  "Hello World from Assembly\n"
</textarea>
</code-fence>
```


## Go

<code-fence lang="go" heading="Hello World from Go">
<textarea vue-slot="code">
package main
import "fmt"
func main() {
    fmt.Println("Hello World from Go")
}
</textarea>
</code-fence>

```html
<code-fence lang="go" heading="Hello World from Go">
<textarea vue-slot="code">
package main
import "fmt"
func main() {
    fmt.Println("Hello World from Go")
}
</textarea>
</code-fence>
```

## Haskell

<code-fence lang="haskell" heading="Hello World from Haskell">
<textarea vue-slot="code">
main = putStrLn "Hello World from Haskell"
</textarea>
</code-fence>

```html
<code-fence lang="haskell" heading="Hello World from Haskell">
<textarea vue-slot="code">
main = putStrLn "Hello World from Haskell"
</textarea>
</code-fence>
```

## Java

<code-fence lang="java" heading="Hello World from Java">
<textarea vue-slot="code">
class Main {
    public static void main(String args[]) {
        System.out.println("Hello World from Java");
    }
}
</textarea>
</code-fence>

```html
<code-fence lang="java" heading="Hello World from Java">
<textarea vue-slot="code">
class Main {
    public static void main(String args[]) {
        System.out.println("Hello World from Java");
    }
}
</textarea>
</code-fence>
```

## Kotlin

<code-fence lang="kotlin" heading="Hello World from Kotlin">
<textarea vue-slot="code">
fun main() {
    println("Hello World from Kotlin")
}
</textarea>
</code-fence>

```html
<code-fence lang="kotlin" heading="Hello World from Kotlin">
<textarea vue-slot="code">
fun main() {
    println("Hello World from Kotlin")
}
</textarea>
</code-fence>
```

## Lua

<code-fence lang="lua" heading="Hello World from Lua">
<textarea vue-slot="code">
print("Hello World from Lua")
</textarea>
</code-fence>

```html
<code-fence lang="lua" heading="Hello World from Lua">
<textarea vue-slot="code">
print("Hello World from Lua")
</textarea>
</code-fence>
```

## Node

<code-fence lang="node" heading="Hello World from JavaScript">
<textarea vue-slot="code">
console.log("Hello World from JavaScript")
</textarea>
</code-fence>


```html
<code-fence lang="node" heading="Hello World from JavaScript">
<textarea vue-slot="code">
console.log("Hello World from JavaScript")
</textarea>
</code-fence>
```

## Php

<code-fence lang="php" heading="Hello World from PHP">
<textarea vue-slot="code">
&lt;?php echo "Hello World from PHP";
</textarea>
</code-fence>

```html
<code-fence lang="php" heading="Hello World from PHP">
<textarea vue-slot="code">
&lt;?php echo "Hello World from PHP";
</textarea>
</code-fence>
```

## Python

<code-fence lang="python" heading="Hello World from Python">
<textarea vue-slot="code">
print("Hello World from Python")
</textarea>
</code-fence>

```html
<code-fence lang="python" heading="Hello World from Python">
<textarea vue-slot="code">
print("Hello World from Python")
</textarea>
</code-fence>
```

## R

<code-fence lang="r" heading="Hello World from R">
<textarea vue-slot="code">
print("Hello World from R")
</textarea>
</code-fence>

```html
<code-fence lang="r" heading="Hello World from R">
<textarea vue-slot="code">
print("Hello World from R")
</textarea>
</code-fence>
```

## Ruby

<code-fence lang="ruby" heading="Hello World from Ruby">
<textarea vue-slot="code">
puts "Hello World from Ruby"
</textarea>
</code-fence>

```html
<code-fence lang="ruby" heading="Hello World from Ruby">
<textarea vue-slot="code">
puts "Hello World from Ruby"
</textarea>
</code-fence>
```

## Rust

<code-fence lang="rust" heading="Hello World from Rust">
<textarea vue-slot="code">
fn main() {
    println!("Hello World from Rust");
}
</textarea>
</code-fence>

```html
<code-fence lang="rust" heading="Hello World from Rust">
<textarea vue-slot="code">
fn main() {
    println!("Hello World from Rust");
}
</textarea>
</code-fence>
```

## Scala

<code-fence lang="scala" heading="Hello World from Scala">
<textarea vue-slot="code">
object Main {
    def main(args: Array[String]) = {
        println("Hello World from Scala")
    }
}
</textarea>
</code-fence>

```html
<code-fence lang="scala" heading="Hello World from Scala">
<textarea vue-slot="code">
object Main {
    def main(args: Array[String]) = {
        println("Hello World from Scala")
    }
}
</textarea>
</code-fence>
```

## Swift

<code-fence lang="swift" heading="Hello World from Swift">
<textarea vue-slot="code">
print("Hello World from Swift")
</textarea>
</code-fence>

```html
<code-fence lang="swift" heading="Hello World from Swift">
<textarea vue-slot="code">
print("Hello World from Swift")
</textarea>
</code-fence>
```

## TypeScript

<code-fence lang="ts" heading="Hello World from TypeScript">
<textarea vue-slot="code">
console.log("Hello World from TypeScript")
</textarea>
</code-fence>

```html
<code-fence lang="ts" heading="Hello World from TypeScript">
<textarea vue-slot="code">
console.log("Hello World from TypeScript")
</textarea>
</code-fence>
```

## D

<code-fence lang="d" heading="Hello World from D">
<textarea vue-slot="code">
import std.stdio;

void main()
{
    writeln("Hello World from D");
}
</textarea>
</code-fence>

```html
<code-fence lang="d" heading="Hello World from D">
<textarea vue-slot="code">
import std.stdio;

void main()
{
    writeln("Hello World from D");
}
</textarea>
</code-fence>
```

## Perl

<code-fence lang="perl" heading="Hello World from Perl">
<textarea vue-slot="code">
print "Hello World from Perl"
</textarea>
</code-fence>

```html
<code-fence lang="perl" heading="Hello World from Perl">
<textarea vue-slot="code">
print "Hello World from Perl"
</textarea>
</code-fence>
```

## Raku

<code-fence lang="raku" heading="Hello World from Raku">
<textarea vue-slot="code">
say "Hello World from Raku"
</textarea>
</code-fence>

```html
<code-fence lang="raku" heading="Hello World from Raku">
<textarea vue-slot="code">
say "Hello World from Raku"
</textarea>
</code-fence>
```

## Zig

<code-fence lang="zig" heading="Hello World from Zig">
<textarea vue-slot="code">
const std = @import("std");

pub fn main() !void {
    const stdout = std.io.getStdOut().outStream();
    try stdout.print("Hello World from Zig\n", .{});
}
</textarea>
</code-fence>

```html
<code-fence lang="zig" heading="Hello World from Zig">
<textarea vue-slot="code">
const std = @import("std");

pub fn main() !void {
    const stdout = std.io.getStdOut().outStream();
    try stdout.print("Hello World from Zig\n", .{});
}
</textarea>
</code-fence>
```

## Dart

<code-fence lang="dart" heading="Hello World from Dart">
<textarea vue-slot="code">
void main() {
    print('Hello World from Dart');
}
</textarea>
</code-fence>

```html
<code-fence lang="dart" heading="Hello World from Dart">
<textarea vue-slot="code">
void main() {
    print('Hello World from Dart');
}
</textarea>
</code-fence>
```

## Forth

<code-fence lang="forth" heading="Hello World from Forth">
<textarea vue-slot="code">
.( Hello World from Forth) CR
bye
</textarea>
</code-fence>

```html
<code-fence lang="forth" heading="Hello World from Forth">
<textarea vue-slot="code">
.( Hello World from Forth) CR
bye
</textarea>
</code-fence>
```

## Ada

<code-fence lang="ada" heading="Hello World from Ada">
<textarea vue-slot="code">
with Text_IO; use Text_IO;
procedure main is
    begin Put_Line("Hello World from Ada");
end main;
</textarea>
</code-fence>

```html
<code-fence lang="ada" heading="Hello World from Ada">
<textarea vue-slot="code">
with Text_IO; use Text_IO;
procedure main is
    begin Put_Line("Hello World from Ada");
end main;
</textarea>
</code-fence>
```
