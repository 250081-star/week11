#include <iostream>
using namespace std;


// //problem 1
// const int N = 2;
// const int M = 3;
//
// void inputMatrix(int matrix[][M], int N, int M) {
//     cout << "Enter " << N << "x" << M << "matrix elements:\n";
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> matrix[i][j];
//         }
//     }
// }
//
// void printMatrix(int matrix[][M], int N, int M) {
//     cout << "\nMatrix:\n";
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cout << matrix[i][j] << " ";
//         }
//         cout << endl;
//     }
// }
//
// int main() {
//     int matrix[N][M];
//
//     inputMatrix(matrix, N, M);
//     printMatrix(matrix, N, M);
//
//     return 0;
// }

//problem 2

// const int N = 3;
// const int M = 3;
//
// void displayMatrix(int matrix[N][M], int N, int M) {
//     cout << "\nMatrix elements:\n";
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cout << matrix[i][j] << "\t";
//         }
//         cout << endl;
//     }
// }
//
// int main() {
//     int matrix[N][M] = {
//         {1, 2, 3},
//         {4, 5, 6},
//         {7, 8, 9}
//     };
//
//     displayMatrix(matrix, N, M);
//
//     return 0;
// }

//problem 3

// const int N = 3;
// const int M = 3;
//
// int sumMatrix(int matrix[N][M], int N, int M) {
//     int total = 0;
//
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             total += matrix[i][j];
//         }
//     }
//
//     return total;
// }
//
// int main() {
//     int matrix[N][M];
//
//     cout << "Enter elements for a " << N << "x" << M << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> matrix[i][j];
//         }
//     }
//
//     int sum = sumMatrix(matrix, N, M);
//
//     cout << "Sum of all elements = " << sum << endl;
//
//     return 0;
// }
//

//problem 4

// const int N = 3;
// const int M = 3;
//
// void rowWiseMax(int matrix[N][M], int N, int M) {
//     for (int i = 0; i < N; i++) {
//         int maxNum = matrix[i][0];
//
//         for (int j = 1; j < M; j++) {
//             if (matrix[i][j] > maxNum) {
//                 maxNum = matrix[i][j];
//             }
//         }
//
//         cout << "Max in row " << i + 1 << " = " << maxNum << endl;
//     }
// }
//
// int main() {
//     int matrix[N][M];
//
//     cout << "Enter elements for a " << N << "x" << M << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> matrix[i][j];
//         }
//     }
//
//     cout << "\nRow-wise maximum values:" << endl;
//     rowWiseMax(matrix, N, M);
//
//     return 0;
// }
//
//

// problem 5

// const int N = 3;
// const int M = 3;
//
// void columnWiseSum(int matrix[N][M], int N, int M) {
//     for (int j = 0; j < M; j++) {
//         int sum = 0;
//         for (int i = 0; i < N; i++) {
//             sum += matrix[i][j];
//         }
//         cout << "Sum of column " << j + 1 << " = " << sum << endl;
//     }
// }
//
// int main() {
//     int matrix[N][M];
//
//     cout << "Enter elements for a " << N << "x" << M << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> matrix[i][j];
//         }
//     }
//
//     cout << "\nColumn-wise sums:" << endl;
//     columnWiseSum(matrix, N, M);
//
//     return 0;
// }

// problem 6

// const int N = 3;
//
// int diagonalSum(int matrix[N][N], int N) {
//     int sum = 0;
//     for (int i = 0; i < N; i++) {
//         sum += matrix[i][i];
//     }
//     return sum;
// }
//
// int main() {
//     int matrix[N][N];
//
//     cout << "Enter elements for a " << N << "x" << N << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < N; j++) {
//             cin >> matrix[i][j];
//         }
//     }
//
//     cout << "\nSum of main diagonal = " << diagonalSum(matrix, N) << endl;
//     return 0;
// }
//

//problem 7

// const int N = 3;
// const int M = 2;
//
// void transposeMatrix(int A[N][M], int B[M][N]) {
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             B[j][i] = A[i][j];
//         }
//     }
// }
//
// int main() {
//     int A[N][M], B[M][N];
//
//     cout << "Enter elements of " << N << "x" << M << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> A[i][j];
//         }
//     }
//
//     transposeMatrix(A, B);
//
//     cout << "\nTranspose of the matrix:" << endl;
//     for (int i = 0; i < M; i++) {
//         for (int j = 0; j < N; j++) {
//             cout << B[i][j] << " ";
//         }
//         cout << endl;
//     }
//
//     return 0;
// }
//

// problem 8
//
// const int N = 2;
// const int M = 3;
//
// void addMatrices(int A[N][M], int B[N][M], int C[N][M]) {
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             C[i][j] = A[i][j] + B[i][j];
//         }
//     }
// }
//
// int main() {
//     int A[N][M], B[N][M], C[N][M];
//
//     cout << "Enter elements of first " << N << "x" << M << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> A[i][j];
//         }
//     }
//
//     cout << "Enter elements of second " << N << "x" << M << " matrix:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cin >> B[i][j];
//         }
//     }
//
//     addMatrices(A, B, C);
//
//     cout << "\nResult of addition:" << endl;
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < M; j++) {
//             cout << C[i][j] << " ";
//         }
//         cout << endl;
//     }
//
//     return 0;
// }


//problem 9

// int main() {
//     int n, m;
//     cout << "Enter size of matrices (n m): ";
//     cin >> n >> m;
//
//     int A[n][m], B[m][n], C[n][n];
//
//     cout << "Enter elements of first matrix:" << endl;
//     for (int i = 0; i < n; i++) {
//         for (int j = 0; j < m; j++) {
//             cin >> A[i][j];
//         }
//     }
//
//     cout << "Enter elements of second matrix:" << endl;
//     for (int i = 0; i < m; i++) {
//         for (int j = 0; j < n; j++) {
//             cin >> B[i][j];
//         }
//     }
//
//     for (int i = 0; i < n; i++) {
//         for (int j = 0; j < n; j++) {
//             C[i][j] = 0;
//             for (int k = 0; k < m; k++) {
//                 C[i][j] += A[i][k] * B[k][j];
//             }
//         }
//     }
//
//     cout << "\nResultant matrix after multiplication:" << endl;
//     for (int i = 0; i < n; i++) {
//         for (int j = 0; j < n; j++) {
//             cout << C[i][j] << " ";
//         }
//         cout << endl;
//     }
//
//     return 0;
// }
//

//problm 10

// const int N = 3;
//
// void rotateMatrix(int matrix[][N]) {
//
//     for (int i = 0; i < N; i++) {
//         for (int j = i + 1; j < N; j++) {
//             int temp = matrix[i][j];
//             matrix[i][j] = matrix[j][i];
//             matrix[j][i] = temp;
//         }
//     }
//
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < N / 2; j++) {
//             int temp = matrix[i][j];
//             matrix[i][j] = matrix[i][N - j - 1];
//             matrix[i][N - j - 1] = temp;
//         }
//     }
// }
//
// void printMatrix(int matrix[][N]) {
//     for (int i = 0; i < N; i++) {
//         for (int j = 0; j < N; j++) {
//             cout << matrix[i][j] << " ";
//         }
//         cout << endl;
//     }
// }
//
// int main() {
//     int matrix[N][N] = {
//         {1, 2, 3},
//         {4, 5, 6},
//         {7, 8, 9}
//     };
//
//     cout << "Original matrix:\n";
//     printMatrix(matrix);
//
//     rotateMatrix(matrix);
//
//     cout << "\nMatrix after 90 degree rotation:\n";
//     printMatrix(matrix);
//
//     return 0;
// }

