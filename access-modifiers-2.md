Access Modifiers in TypeScript OOP (Public, Private, Protected, and Readonly)

Introduction

In TypeScript, access modifiers control how class properties and methods can be accessed or modified. They are important concepts in Object-Oriented Programming (OOP) because they help protect data and maintain proper code structure. TypeScript provides four commonly used modifiers: public, private, protected, and readonly.

Detailed Body

1. Public

The public modifier allows properties and methods to be accessed from anywhere, both inside and outside the class. It is the default access modifier in TypeScript.

class User {
    public name: string = "Jabir";
}

const user = new User();
console.log(user.name);

2. Private

The private modifier restricts access to a property or method within the class where it is declared.

class BankAccount {
    private balance: number = 5000;

    getBalance() {
        return this.balance;
    }
}

const account = new BankAccount();
console.log(account.getBalance()); 
console.log(account.balance);

3. Protected

The protected modifier allows access within the declaring class and its subclasses, but not from outside the class.

class Person {
    protected age: number = 25;
}

class Student extends Person {
    showAge() {
        console.log(this.age);
    }
}

4. Readonly

The readonly modifier allows a property to be assigned only during initialization or inside the constructor. It cannot be reassigned afterward.

class Employee {
    readonly id: number = 101;
}

const employee = new Employee();
console.log(employee.id);
employee.id = 102; 

Conclusion

Access modifiers help developers control data accessibility and improve code organization. Use public for accessible properties, private for internal data, protected for inheritance, and readonly for values that should not change after initialization. Understanding these modifiers helps you write more secure, readable, and maintainable TypeScript applications.