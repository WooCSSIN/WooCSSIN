#include <iostream>
#include <vector>
#include <algorithm>

using namespace std;

int main() {
	vector<int> numbers = { 7,3,5,2,6 };
	// khoi tao cac gia tri so nguyen 

	sort(numbers.begin(), numbers.end(), [](int a, int b){
		return a < b; // tra ve va sap xep theo gia tri tang dan va nguoc lai 

		});
	// ham sort nhan vao hai con tro chi den phan tu dau tien va cuoi cung cua vector
	// ham se tra ve true ghi so thu nhat nho hon so thu hai, va tro ve false neu nguoc lai
	// sort se sap xep vector numbers theo thu tu tang dan  

	cout << "sorted numbers: ";
	for (int x : numbers) {
		// su dung for de duyet qua tunng phan tu trong vector va in ra gia tri cua no
		cout << x << " ";
		// moi gia tri duoc pohan cach boi nhung khoang trang
	}
	cout << endl;
	return 0;
}
