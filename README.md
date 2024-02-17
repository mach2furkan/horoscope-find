    #include <iostream>
      using namespace std;

    string findHoroscope(int month, int day) {
    string horoscope;

    if ((month == 3 && day >= 21) || (month == 4 && day <= 19))
        horoscope = "Aries";
    else if ((month == 4 && day >= 20) || (month == 5 && day <= 20))
        horoscope = "Taurus";
    else if ((month == 5 && day >= 21) || (month == 6 && day <= 20))
        horoscope = "Gemini";
    else if ((month == 6 && day >= 21) || (month == 7 && day <= 22))
        horoscope = "Cancer";
    else if ((month == 7 && day >= 23) || (month == 8 && day <= 22))
        horoscope = "Leo";
    else if ((month == 8 && day >= 23) || (month == 9 && day <= 22))
        horoscope = "Virgo";
    else if ((month == 9 && day >= 23) || (month == 10 && day <= 22))
        horoscope = "Libra";
    else if ((month == 10 && day >= 23) || (month == 11 && day <= 21))
        horoscope = "Scorpio";
    else if ((month == 11 && day >= 22) || (month == 12 && day <= 21))
        horoscope = "Sagittarius";
    else if ((month == 12 && day >= 22) || (month == 1 && day <= 19))
        horoscope = "Capricorn";
    else if ((month == 1 && day >= 20) || (month == 2 && day <= 18))
        horoscope = "Aquarius";
    else if ((month == 2 && day >= 19) || (month == 3 && day <= 20))
        horoscope = "Pisces";
    else
        horoscope = "Invalid date";

    return horoscope;
       }

    int main() {
    int month, day;
    cout << "Enter your birth month (as a number): ";
    cin >> month;
    cout << "Enter your birth day: ";
    cin >> day;

    string horoscope = findHoroscope(month, day);
    cout << "Your horoscope is: " << horoscope << endl;

    return 0;
     }
