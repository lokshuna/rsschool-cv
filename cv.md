# **Liliia Voloshchuk**
### *Student*

## Information:
### My goal is to learn how to program, master the skills of working with website and application development, and raise my level of knowledge to the proper level to get my dream job. My strengths include a fast learning curve, quick perception and processing of information, dedication, and good communication skills. I am eager to learn everything related to website development and programming languages

## Skills:

### *C++
### *C#
### *Python

## Code examples:

 ``` С++
 int main() {

	ifstream fin ("trees.txt");
	size_t n; fin >> n;
	int mostProductiveTree = 0;
	fruitTree* fruits = new fruitTree[n];
	for (size_t i = 0; i < n; ++i) {
		fin >> fruits[i];
	}
	fin.close();
	cout << "All trees: ";
	printArray(fruits, n);
	for (size_t i = 0; i < n; ++i) {
		fruits[i].growing();
	}
	cout << "+1 year"; 
	printArray(fruits, n);

	cout << "Highest tree: " << highestTree(fruits, n);
	cout << "The most productive tree: " << fecundity(fruits, n);
	fruitTree* newTree = treeArray(fruits, n, mostProductiveTree);
	fillFile(newTree, mostProductiveTree, "finalTrees.txt");

return 0;
 }
 ```
