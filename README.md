#include <iostream>

template<typename T>
class Node {
public:
    T data;
    Node* next;

    Node(T item) : data(item), next(nullptr) {}
};

template<typename T>
class SinglyLinkedList {
private:
    Node<T>* head;

public:
    
    SinglyLinkedList() : head(nullptr) {}

    
    ~SinglyLinkedList() {
        clear();
    }
