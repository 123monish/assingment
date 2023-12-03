#include <iostream>
using namespace std;

const int MAX = 10;

int main() {
    int matrix[MAX][MAX], rows, columns, i, j, sum = 0;

    cout << "Enter the number of rows and columns for the square matrix: ";
    cin >> rows >> columns;

    if (rows != columns) {
        cout << "The matrix should be a square matrix (number of rows should be equal to number of columns)." << endl;
        return 1;
    }

    cout << "Enter the elements of the matrix:" << endl;

    
    for (i = 0; i < rows; ++i) {
        for (j = 0; j < columns; ++j) {
            cout << "Enter element matrix[" << i + 1 << "][" << j + 1 << "]: ";
            cin >> matrix[i][j];
        }
    }

    
    for (i = 0; i < rows; ++i) {
        sum += matrix[i][i];
    }

    cout << "The sum of the main diagonal elements is: " << sum << endl;

    return 0;
}
