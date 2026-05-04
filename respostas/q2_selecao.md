C:

switch (k) {
    case 1:
    case 2:
        j = 2 * k - 1;
        break;
    case 3:
    case 5:
        j = 3 * k + 1;
        break;
    case 4:
        j = 4 * k - 1;
        break;
    case 6:
    case 7:
    case 8:
        j = k - 2;
        break;
}


RUBY:

case k
when 1, 2
  j = 2 * k - 1
when 3, 5
  j = 3 * k + 1
when 4
  j = 4 * k - 1
when 6, 7, 8
  j = k - 2
end


ERLANG:

J = case K of
    1 -> 2 * K - 1;
    2 -> 2 * K - 1;
    3 -> 3 * K + 1;
    5 -> 3 * K + 1;
    4 -> 4 * K - 1;
    6 -> K - 2;
    7 -> K - 2;
    8 -> K - 2
end.