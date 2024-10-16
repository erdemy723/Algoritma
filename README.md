# Algoritma
#include <stdio.h>
#include <time.h>
int main() {
clock_t start = clock();
printf("Merhaba MIS, algoritma ve programlama\n");
clock_t end = clock();
double time_spent = (double)(end - start) /
CLOCKS_PER_SEC;
printf("C işlem süresi: %f saniye\n", time_spent);
return 0;} 
C işlem süresi 0.006

#include <iostream>
#include <ctime>
int main() {
clock_t start = clock();
std::cout << "Merhaba MIS, algoritma ve programlama \n";
clock_t end = clock();
double time_spent = (double)(end - start) /
CLOCKS_PER_SEC;
std::cout << "C++ işlem süresi: " << time_spent << "
saniye\n";
return 0;}
C++ işlem süresi 0.002

using System;
using System.Diagnostics;
class Program
{
static void Main()
{
Stopwatch stopwatch = new Stopwatch();
stopwatch.Start();
Console.WriteLine("Merhaba MIS, algoritma ve programlama dersi başladı");
stopwatch.Stop();
Console.WriteLine($"C# işlem süresi: {stopwatch.Elapsed.TotalSeconds} saniye");
}
}
C# işlem süresi 0.036

public class Main {
public static void main(String[] args) {
long startTime = System.nanoTime();
System.out.println("Merhaba MIS, algoritma ve
programlama dersi başladı");
long endTime = System.nanoTime();
double duration = (endTime - startTime) /
1_000_000.0; // milisaniye cinsine çevir
System.out.println("Java işlem süresi: " + duration + "
milisaniye");
}
}
Java işlem süresi 0.028

const startTime = process.hrtime();
console.log("Merhaba MIS, algoritma ve programlama dersi
başladı");
const endTime = process.hrtime(startTime);
const duration = endTime[0] * 1e3 + endTime[1] / 1e6; //
milisaniye cinsine çevir
console.log(`JavaScript işlem süresi: ${duration.toFixed(3)}
milisaniye`);
Javascript işlem süresi 0.055

package main
import (
"fmt"
"time"
)
func main() {
start := time.Now()
fmt.Println("Merhaba MIS, algoritma ve programlama")
elapsed := time.Since(start)
fmt.Printf("Go işlem süresi: %s saniye\n", elapsed)
}
Go işlem süresi 0.025

use std::time::Instant;
fn main() {
let start = Instant::now();
println!("Merhaba MIS, algoritma ve programlama");
let duration = start.elapsed();
println!("Rust işlem süresi: {:?}", duration);
}
Rust işlem süresi 0.021

start = Time.now
puts "Merhaba MIS, algoritma ve programlama"
finish = Time.now
puts "Ruby işlem süresi: #{finish - start} saniye"
Ruby işlem süresi 0.039

use Time::HiRes qw(time);
my $start = time();
print "Merhaba MIS, algoritma ve programlama\n";
my $end = time();
printf "Perl işlem süresi: %f saniye\n", $end - $start;
Perl işlem süresi 0.031

import time
start = time.time()
print("Merhaba MIS, algoritma ve programlama
dersi başladı")
end = time.time()
print(f"Python işlem süresi: {end - start} saniye")
Python işlem süresi 0.001
