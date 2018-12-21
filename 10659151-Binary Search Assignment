#include <iostream>

using namespace std;

int binarySearch(int array[], int size, int search_Value)
{
    int down = 0;
    int top = size - 1;

    int mid;

    while (down <= top)
    {
        mid = (down + top) / 2;

        if(search_Value == array[mid])
        {
            return mid;
        }
        else if (search_Value > array[mid])
        {
            down = mid + 1;
        }
        else
        {
            top = mid - 1;
        }
    }

    return -1;

}

int main()
{
    int a[] = {12, 22, 34, 47, 55, 67, 82, 98};

    int user_Value;

    cout << "Enter an integer: " << endl;
    cin >> user_Value;

    int result = binarySearch(a, 8, user_Value);

    if(result >= 0)
    {
        cout << "The number " << a[result] << " was found at the"
                " element with index " << result << endl;
    }
    else
    {
        cout << "The number " << user_Value << " was not found. " << endl;
    }
}

