#include <iostream>
#include <string>
using namespace std;

int main()
{
    string frame1, frame2 = "";
    int counter = 0;

    cout << "Enter bits for frame 1: ";
    cin >> frame1;

    for (int i = 0; i < frame1.length(); i++)
    {
        if (frame1[i] == '1')
        {
            counter++;
            frame2 += frame1[i];

            if (counter == 5)
            {
                frame2 += '0';
                counter = 0;
            }
        }
        else
        {
            counter = 0;
            frame2 += frame1[i];
        }
    }

    cout << "Frame 1: " << frame1 << endl;
    cout << "Frame 2 after bit stuffing: " << frame2 << endl;

    return 0;
}
