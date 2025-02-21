# Mushrooms

__Программа из семинара__

---

**Условие задания**

Дано целое число 1 <= n <= 40, необходимо вычислить *n*-е число Фибоначчи.

```cpp

#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;

    if (n == 0) {
        cout << 0 << endl;
        return 0;
    }
    if (n == 1) {
        cout << 1 << endl;
        return 0;
    }

    int a = 0, b = 1, fib = 0;
    for (int i = 2; i <= n; i++) {
        fib = a + b;
        a = b;
        b = fib;
    }
    cout << fib << endl;
    return 0;
}

```
