# Lecture-14-Arrays-Algorithm-

//EXERCISES

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

    #include <iostream>
    #include <array>
    #include <algorithm>
    #include <string>
    using namespace std;

    int main()
    {
        int i;
        double n = 0, arr[10];
        cout << "\nEnter 10 numbers\n\n";
        for (i = 0; i < 10; i++)
        {
            cout << "Number " << i + 1 << " : ";
            cin >> arr[i];

            while (cin.fail())
            {
                cout << "\nInvalid Input\n";
                cout << "Enter the number again\n\n";
                cin.clear();
                cin.ignore(1000, '\n');

            }
        }

        for (i = 0; i < 10; ++i)
        {

            if (n < arr[i])
                n = arr[i];
        }
        cout << "Largest number = " << n;

        return 0;
    }

Exercise

Write a program that fills an integer array of 10 numbers From the user in an array Then print out the smallest number

    #include <iostream>
    #include <array>
    #include <algorithm>
    #include <string>
    using namespace std;

    int main()
    {
        int i;
        double n = 0, arr[10];
        cout << "\nEnter 10 numbers\n\n";
        for (i = 0; i < 10; ++i)
        {
            cout << "Number " << i + 1 << ": ";
            cin >> arr[i];

            while (cin.fail())
            {
                cout << "\nInvalid Input\n";
                cout << "Enter the number again\n\n";
                cin.clear();
                cin.ignore(1000, '\n');

            }
        }
        n = arr[0];
        for (i = 0; i < 10; ++i)
        {

            if (n > arr[i])
                n = arr[i];
        }
        cout << "smallest number = " << n;

        return 0;
    }


//NOT EXERCISES

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


























