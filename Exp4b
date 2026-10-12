#include <iostream>
#include <string>
using namespace std;

int main()
{
    string frame1, frame2 = "";
    int counter = 0;

    cout << "Enter the stuffed bits: ";
    cin >> frame1;

    for (int i = 0; i < frame1.length(); i++)
    {
        if (frame1[i] == '1')
        {
            counter++;
            frame2 += frame1[i];

            if (counter == 5)
            {
                counter = 0;

                if (i + 1 < frame1.length() && frame1[i + 1] == '0')
                {
                    i++;
                }
            }
        }
        else
        {
            counter = 0;
            frame2 += frame1[i];
        }
    }

    cout << "Received stuffed frame: " << frame1 << endl;
    cout << "Frame after bit destuffing: " << frame2 << endl;

    return 0;
}
