PYTHON:

j = -3
i = 0
continuar = True

while i < 3 and continuar:
    alvo = j + 2
    
    if alvo == 3 or alvo == 2:
        j -= 1
    elif alvo == 0:
        j += 2
    else:
        j = 0
    
    if j > 0:
        continuar = False
    else:
        j = 3 - i
        i += 1


JAVA:

int j = -3;
int i = 0;

while (i < 3 && j <= 0) {

    j = switch (j + 2) {
        case 3, 2 -> j - 1;
        case 0 -> j + 2;
        default -> 0;
    };

    if (j <= 0) {
        j = 3 - i;
        i++;
    }
}


JAVASCRIPT:

let j = -3;
let i = 0;

while (i < 3 && j <= 0) {
    const alvo = j + 2;

    if (alvo === 3 || alvo === 2) {
        j--;
    } else if (alvo === 0) {
        j += 2;
    } else {
        j = 0;
    }

    if (j <= 0) {
        j = 3 - i;
        i++;
    }
}