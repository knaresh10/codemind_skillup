#include<bits/stdc++.h>
using namespace std;
bool isprime(int n) {
	if (n == 1) return false;
	for (int i = 2; i * i <= n; i++)
		if (n % i == 0) return false;
	return true;
}
int main() {
	int n; cin >> n;
	int arr[n];
	for (int i = 0; i < n; i++) {
		cin >> arr[i];
	}
	int min = arr[0], max = arr[0];
	int min_index = 0, max_index = 0;
	for (int i = 1; i < n; i++) {
		if (max < arr[i]) {
			max = arr[i];
			max_index = i;
		}
		if (min > arr[i]) {
			min = arr[i];
			min_index = i;
		}
	}
	int count = 0;
	if (min_index < max_index) {
		for (int i = min_index; i <= max_index; i++) {
			if (isprime(arr[i]))
				count++;
		}
	}
	else {
		for (int i = max_index; i <= min_index; i++) {
			if (isprime(arr[i]))
				count++;
		}
	}

	cout << count;
}
