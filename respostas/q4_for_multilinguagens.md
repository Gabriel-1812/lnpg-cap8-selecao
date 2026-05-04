PYTHON:

n = 100
sum_val = 0
for i, j in zip(range(n), range(17, 17 - n, -1)):
    sum_val += i * j + 3


JAVASCRIPT:

let n = 100;
let sum = 0;
for (let i = 0, j = 17; i < n; i++, j--) {
    sum += i * j + 3;
}


SWIFT:

var i = 0, j = 17, n = 100, sum = 0
while i < n {
    sum += i * j + 3
    i += 1
    j -= 1
}


GO:

n := 100
sum := 0
for i, j := 0, 17; i < n; i, j = i+1, j-1 {
    sum += i*j + 3
}


RUBY:

n = 100
sum = 0
j = 17
n.times do |i|
  sum += i * j + 3
  j -= 1
end