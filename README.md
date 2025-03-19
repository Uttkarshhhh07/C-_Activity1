# C-_Activity1
#include <iostream>
#include <string>
using namespace std;

class Book {
private:
    int bookId;
    string title, author;

public:
    Book(int id, string t, string a) {
        bookId = id;
        title = t;
        author = a;
    }

    void display() {
        cout << "Book ID: " << bookId << ", Title: " << title << ", Author: " << author << endl;
    }
};

int main() {
    Book books[3] = {
        Book(101, "The Alchemist", "Paulo Coelho"),
        Book(102, "1984", "George Orwell"),
        Book(103, "To Kill a Mockingbird", "Harper Lee")
    };

    cout << "Library Books:\n";
    for (int i = 0; i < 3; i++) {
        books[i].display();
    }

    return 0;
}
