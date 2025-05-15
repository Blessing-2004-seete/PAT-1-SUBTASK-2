#include <iostream>
using namespace std;
int main() {
    int temp1, temp2, temp3;

    // Step 1: Input the first temperature
    cout << "Enter the first temperature reading: ";
    cin >> temp1;

    // Step 2: Input the second temperature
    cout << "Enter the second temperature reading (5 minutes later): ";
    cin >> temp2;

    int increase = temp2 - temp1;

    // Step 3: Check the difference between first and second readings
    if (increase > 50) {
        cout << "Reduce fryer heat before taking the third reading." << endl;
    } else if (increase < 10) {
        cout << "Increase the Fryer heat before taking the third reading." << endl;
    }

    // Step 4: Input the third temperature
    cout << "Enter the third temperature reading (5 minutes later): ";
    cin >> temp3;

    // Step 5: Check if third reading is within the frying range
    if (temp3 >= 150 && temp3 <= 190) {
        cout << "You may start frying the Magwinyas." << endl;
    } else {
        cout << "Oil is not ready for frying!" << endl;
    }

    return 0;
}
