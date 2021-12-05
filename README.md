# Lecture-14-Arrays-Algorithm-


Standard LibraryArray Methods

    #include <iostream>
    #include <array>
    using namespace std;
    int main()
    {
      array<string, 4> arr = { "Mars Bar", "Snickers", "Bounty", "Wispa"};
      cout << arr.at(1) << endl;
      cout << arr[1] << endl;

      cout << arr.front()<< endl;
      cout << arr.back()<< endl;

      for (int i = 0; i < arr.size(); i++) {
        cout << arr.at(i) << ", ";
      }
      cout << endl;
    }


Algorithm Sorting Example

    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      array<int, 5> numbers = { 33, 5, 7, 99, 83 };
      sort(numbers.begin(), numbers.end());
      for (int num : numbers) {
        cout << num << " ";
      }

    }


Algorithm Example Sorting largest to smallest

    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      array<int, 5> numbers = { 33, 5, 7, 99, 83 };
      sort(numbers.begin(), numbers.end());
      reverse(numbers.begin(), numbers.end());
      for (int num : numbers) {
        cout << num << " ";
      }

    }


rand function
  
    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      int randomArray[10];
      for (int i = 0; i < 10; i++) 
      {
        randomArray[i] = rand() % 50;
        cout << randomArray[i] << endl;
      }

    }


Exercise

Write a program that fills an integer array of 1000 random numbers between 1-100. Next count the number 6 appears in the array and output this information to the console.

    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      int randomArray[1000];
      int counter = 0;
      for (int i = 0; i < 1000; i++) 
      {
        randomArray[i] = rand() % 100;
        cout << randomArray[i] << endl;

        if (randomArray[i] == 6)
        {
          counter++;
        }
      }
      cout << "6 appeared " << counter << "x" << endl;

    }


Exercise

Write a program that fills an integer array of 10 numbers From the user in an array Then print out the largest number 



Exercise

Write a program that fills an integer array of 10 numbers From the user in an array Then print out the smallest number



























