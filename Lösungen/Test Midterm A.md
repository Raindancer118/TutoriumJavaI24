1)
1. public
2. String
3. String
4. String
5. String
6. int
7. void

Aufgabe 2)
57
57
57
12
572
122

Aufgabe 3)
```
public void printLine(String str, int[] zahl) {
	int sum = 0;
	for(int j = 0; j < zahl.length; j++) {
		sum += zahl[j];
	}
	for(int i = 0; i < sum; i++) {
		System.out.print(str);
	}
}
```

```
int[] zahl = {};
```

```
int sum = 0;
for (int x: zahl) {
	sum+=x;
}
```

Aufgabe 4.1)
```
public int countEven (int[] numbers) {
	int total = 0;
	for (int num: numbers) {
		if (num % 2 == 0) total ++;
	}
	return total;
}
```

```
public int countEven (int[] numbers) {
	int total = 0;
	for (int i = 0; i < numbers.length; i++) {
		if (numbers[i] % 2 == 0) total ++;
	}
	return total;
}
```

Aufgabe 4.2)
```
public int[] filterEven (int[] numbers) {
	int[] evens = new int[countEven(numbers)];
	int pos = 0;
	for (int i = 0; i < numbers.length; i++) {
		if (numbers[i] % 2 == 0) {
			evens[pos] = numbers[i];
			pos++;
		}
	}
	return evens;
}
```
