# Function-Exercise
#include <iostream>
#include <string>
#include <array>

#include <math.h>


using namespace std;

string powValues(double a) {

	for (int i{ 10 }; i > 0; i--) {
		double powValue = (i);
		cout << a << " to the power of " << i << " is " << pow(a, powValue) << endl;
	}
	return "The code had ended";
}


int main() {
	double userInput{};
	cout << "Enter a value to get its power value from 1 to 10: ";
	cin >> userInput;
	while (cin.fail()) {
		cout << "Invalid input.Please enter a another input: ";
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> userInput;
	}
	cout << powValues(userInput);
string rootValues(double a) {

	for (int i{ 10 }; i > 0; i--) {
		double powValue = (1.0 / i);
		cout << a << " to the root of " << i << " is " << pow(a, powValue) << endl;
	}
	return "The code had ended";

}


int main() {

	double userInput{};
	cout << "Enter a value to get its root value from 1 to 10: ";
	cin >> userInput;
	while (cin.fail()) {
		cout << "Invalid input.Please enter a another input: ";
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> userInput;

	}

	cout << rootValues(userInput);
}
