#include <iostream>

int foo(int x,int y,int z) {
	if (x < y && x < z) {
		std::cout << "X was the smallest\n";
		return x;
	}
	else if (y < x && y < z) {
		std::cout << "Y was the smallest\n";
		return y;
	}
	else if (z < x && z < y) {
		std::cout << "Z was the smallest\n";
		return z;
	}
	
	std::cout << "No smallest\n";
	return 0;
	
}

int x;
int y; 
int z;

int main()
{
	std::cout << "X: ";
	std::cin >> x;
	std::cout << "Y: ";
	std::cin >> y;
	std::cout << "Z: ";
	std::cin >> z;

	std::cout << "Value: " << foo(x, y, z);
}
