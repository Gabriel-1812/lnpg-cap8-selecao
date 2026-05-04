PYTHON:


j = 10.0
k = (j + 13) / 27

while k <= 10:
    k = k + 1
    i = 3 * k - 1
    print(f"k: {k}, i: {i}")

    

JAVA:

public class Main {
    public static void main(String[] args) {
        double j = 10.0;
        
        double k = (j + 13) / 27.0;
        double i;

        while (k <= 10) {
            k = k + 1;
            i = 3 * k - 1;
            System.out.println("k: " + k + ", i: " + i);
        }
    }
}


HASKELL:


loop :: Double -> IO ()
loop k
    | k > 10    = putStrLn "Loop finalizado."
    | otherwise = do
        let k_novo = k + 1
        let i = 3 * k_novo - 1
        putStrLn ("k: " ++ show k_novo ++ ", i: " ++ show i)
        loop k_novo

main :: IO ()
main = do
    let j = 10.0
    let k_inicial = (j + 13) / 27
    loop k_inicial


SWIFT:

import Foundation

let j = 10.0
var k = (j + 13) / 27.0
var i: Double = 0.0

while k <= 10 {
    k += 1
    i = 3 * k - 1
    print("k: \(k), i: \(i)")
}