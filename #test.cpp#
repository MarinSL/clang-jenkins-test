#include <iostream>
#include <memory>

struct Base {
    virtual void func() {
        std::cout << "base" << std::endl;
    }
};

struct Sub : public Base {
    virtual void func() {
        std::cout << "sub" << std::endl;
    }
};

int main() {

    std::unique_ptr<Base> ptrBase{new Base{}};
    std::unique_ptr<Base> ptrSub{new Sub{}};

    ptrBase->func();
    ptrSub->func();
}
