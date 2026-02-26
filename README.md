---

# 📘 OOP bo‘yicha 50 ta test savol

---

### 1.

```python
class Car:
    def __init__(self, name):
        self.name = name
```

Bu yerda `__init__` nima vazifani bajaradi?

A) Obyektni o‘chiradi
B) Konstruktor metod
C) Statik metod
D) Inkapsulyatsiya

---

### 2.

```python
class A:
    pass

obj = A()
```

`obj` nima hisoblanadi?

A) Class
B) Funksiya
C) Obyekt
D) Modul

---

### 3.

```python
class Person:
    def speak(self):
        print("Hello")
```

`speak` nima?

A) Konstruktor
B) Obyekt
C) Metod
D) Atribut

---

### 4.

```python
class A:
    x = 10
```

`x` nima?

A) Lokal o‘zgaruvchi
B) Global o‘zgaruvchi
C) Class atributi
D) Metod

---

### 5.

```python
class Test:
    def __init__(self):
        self.a = 5
```

`self.a` nima?

A) Class atribut
B) Obyekt atribut
C) Statik metod
D) Modul

---

### 6.

```python
class Animal:
    def sound(self):
        print("Sound")

class Dog(Animal):
    pass
```

Bu qanday OOP tushunchasi?

A) Polimorfizm
B) Inkapsulyatsiya
C) Vorislik
D) Abstraksiya

---

### 7.

```python
class A:
    def show(self):
        print("A")

class B(A):
    def show(self):
        print("B")
```

Bu qaysi tushunchaga misol?

A) Inkapsulyatsiya
B) Polimorfizm
C) Konstruktor
D) Statik metod

---

### 8.

```python
class A:
    def __private(self):
        print("Hello")
```

`__private` nima?

A) Public metod
B) Protected metod
C) Private metod
D) Statik metod

---

### 9.

```python
class A:
    @staticmethod
    def test():
        print("Hi")
```

Bu qanday metod?

A) Instance metod
B) Constructor
C) Static metod
D) Private metod

---

### 10.

```python
class A:
    @classmethod
    def test(cls):
        print(cls)
```

Bu qanday metod?

A) Static
B) Instance
C) Class metod
D) Private

---

### 11.

```python
class A:
    def __init__(self):
        print("Hello")
```

Obyekt yaratilganda nima sodir bo‘ladi?

A) Hech narsa
B) Xatolik
C) "Hello" chiqadi
D) Class o‘chadi

---

### 12.

```python
class A:
    pass
```

`pass` nima uchun ishlatilgan?

A) Metod chaqirish
B) Bo‘sh blok yaratish
C) Obyekt o‘chirish
D) Vorislik

---

### 13.

```python
class A:
    def __str__(self):
        return "Test"
```

`__str__` nima qiladi?

A) Obyektni o‘chiradi
B) Obyektni stringga aylantiradi
C) Konstruktor
D) Vorislik

---

### 14.

```python
class A:
    def __len__(self):
        return 5
```

Bu qanday metod?

A) Maxsus (magic) metod
B) Static
C) Private
D) Protected

---

### 15.

```python
class A:
    def show(self):
        print(self)
```

`self` nimani bildiradi?

A) Classni
B) Obyektni
C) Modulni
D) Funksiyani

---

### 16.

```python
class Animal:
    def sound(self):
        print("Animal sound")

class Cat(Animal):
    def sound(self):
        print("Meow")
```

Bu qaysi tushunchaga misol?

A) Polimorfizm
B) Inkapsulyatsiya
C) Abstraksiya
D) Static

---

### 17.

```python
class A:
    __x = 10
```

`__x` qanday atribut?

A) Public
B) Protected
C) Private
D) Static

---

### 18.

```python
class A:
    _x = 5
```

`_x` qanday atribut hisoblanadi?

A) Public
B) Protected (konvensiya)
C) Private
D) Magic

---

### 19.

```python
class A:
    def __init__(self, x):
        self.x = x
```

Bu qanday konstruktor?

A) Parametrsiz
B) Parametrli
C) Static
D) Private

---

### 20.

```python
class A:
    def show(self):
        print("Hello")

A.show()
```

Nima sodir bo‘ladi?

A) To‘g‘ri ishlaydi
B) Xatolik
C) Obyekt yaratiladi
D) Hech narsa

---

## 21.

```python
class A:
    def show(self):
        print("A")

class B(A):
    def show(self):
        super().show()
        print("B")

obj = B()
obj.show()
```

Natija qanday bo‘ladi?

A) B
B) A
C) A so‘ng B
D) Xatolik

---

## 22.

```python
class A:
    pass

class B(A):
    pass

class C(B):
    pass
```

Bu qanday vorislik turi?

A) Multiple
B) Multilevel
C) Hybrid
D) Hierarchical

---

## 23.

```python
class A:
    pass

class B:
    pass

class C(A, B):
    pass
```

Bu qanday vorislik turi?

A) Single
B) Multilevel
C) Multiple
D) Hybrid

---

## 24.

```python
class A:
    x = 10

obj1 = A()
obj2 = A()

obj1.x = 20
print(obj2.x)
```

Natija qanday?

A) 20
B) 10
C) None
D) Xatolik

---

## 25.

```python
class A:
    count = 0
    def __init__(self):
        A.count += 1

a1 = A()
a2 = A()
print(A.count)
```

Natija qanday?

A) 0
B) 1
C) 2
D) Xatolik

---

## 26.

```python
class A:
    def __add__(self, other):
        return 100

a = A()
b = A()
print(a + b)
```

Natija qanday?

A) Xatolik
B) 100
C) None
D) 0

---

## 27.

```python
class A:
    def __eq__(self, other):
        return True

a = A()
b = A()
print(a == b)
```

Natija qanday?

A) False
B) True
C) None
D) Xatolik

---

## 28.

```python
class A:
    def __init__(self):
        self.__x = 5

    def get_x(self):
        return self.__x

obj = A()
print(obj.get_x())
```

Bu qaysi tushunchaga misol?

A) Polimorfizm
B) Vorislik
C) Inkapsulyatsiya
D) Abstraksiya

---

## 29.

```python
class A:
    def __init__(self):
        self._x = 10
```

`_x` qanday darajadagi atribut?

A) Public
B) Protected (konvensiya)
C) Private
D) Global

---

## 30.

```python
from abc import ABC, abstractmethod

class A(ABC):
    @abstractmethod
    def test(self):
        pass
```

Bu qanday class?

A) Oddiy class
B) Abstract class
C) Static class
D) Private class

---

## 31.

```python
class A:
    def show(self):
        print("Hello")

class B(A):
    pass

obj = B()
obj.show()
```

Bu qaysi tushunchaga misol?

A) Polimorfizm
B) Vorislik
C) Inkapsulyatsiya
D) Duck typing

---

## 32.

```python
class Engine:
    pass

class Car:
    def __init__(self):
        self.engine = Engine()
```

Bu qanday munosabat?

A) Vorislik
B) Composition
C) Polimorfizm
D) Static

---

## 33.

```python
class A:
    def show(self):
        print("A")

class B:
    def show(self):
        print("B")

def test(obj):
    obj.show()

test(A())
test(B())
```

Bu qaysi tushunchaga misol?

A) Vorislik
B) Inkapsulyatsiya
C) Duck typing
D) Abstraksiya

---

## 34.

```python
class A:
    def show(self):
        print("A")

class B(A):
    pass

print(B.__mro__)
```

`__mro__` nimani bildiradi?

A) Metod soni
B) Obyekt adresi
C) Method Resolution Order
D) Konstruktor

---

## 35.

```python
class A:
    x = 5

a = A()
A.x = 10
print(a.x)
```

Natija qanday?

A) 5
B) 10
C) None
D) Xatolik

---

## 36.

```python
class A:
    def __init__(self):
        print("A")

class B(A):
    def __init__(self):
        print("B")

obj = B()
```

Natija qanday?

A) A
B) B
C) A va B
D) Xatolik

---

## 37.

```python
class A:
    def __init__(self):
        print("A")

class B(A):
    def __init__(self):
        super().__init__()
        print("B")

obj = B()
```

Natija qanday?

A) B
B) A
C) A so‘ng B
D) Xatolik

---

## 38.

```python
class A:
    def __init__(self):
        self.x = 5

a = A()
del a.x
print(a.x)
```

Natija qanday?

A) 5
B) None
C) Xatolik
D) 0

---

## 39.

```python
class A:
    @property
    def x(self):
        return 10

a = A()
print(a.x)
```

`@property` nima qiladi?

A) Metodni atribut kabi ishlatadi
B) Statik qiladi
C) Private qiladi
D) O‘chiradi

---

## 40.

```python
class A:
    def __call__(self):
        print("Called")

a = A()
a()
```

Bu qanday imkoniyat?

A) Obyektni funksiya kabi chaqirish
B) Static metod
C) Abstraksiya
D) Vorislik

---

## 41.

```python
class A:
    pass

a = A()
print(isinstance(a, A))
```

Natija qanday?

A) False
B) True
C) None
D) Xatolik

---

## 42.

```python
class A:
    pass

class B(A):
    pass

print(issubclass(B, A))
```

Natija qanday?

A) False
B) True
C) None
D) Xatolik

---

## 43.

```python
class A:
    def __repr__(self):
        return "Object A"

a = A()
print(a)
```

Qaysi metod ishlaydi?

A) **str**
B) **repr**
C) **init**
D) **call**

---

## 44.

```python
class A:
    def __init__(self, x=5):
        self.x = x

a = A()
print(a.x)
```

Natija qanday?

A) None
B) 0
C) 5
D) Xatolik

---

## 45.

```python
class A:
    pass

print(type(A))
```

Natija qanday?

A) class
B) type
C) object
D) None

---

## 46.

```python
class A:
    def show(self):
        print("A")

a = A
a().show()
```

Natija qanday?

A) Xatolik
B) A
C) None
D) show

---

## 47.

```python
class A:
    def __del__(self):
        print("Deleted")

a = A()
del a
```

`__del__` qachon ishlaydi?

A) Obyekt yaratilganda
B) Obyekt o‘chirilganda
C) Metod chaqirilganda
D) Class e’lon qilinganda

---

## 48.

```python
class A:
    x = 5

a = A()
b = A()

b.x = 10
print(A.x)
```

Natija qanday?

A) 10
B) 5
C) None
D) Xatolik

---

## 49.

```python
class A:
    def __init__(self):
        self.x = 5

a = A()
b = a
b.x = 20
print(a.x)
```

Natija qanday?

A) 5
B) 20
C) None
D) Xatolik

---

## 50.

```python
class A:
    def show(self):
        print("Hello")

obj = A()
method = obj.show
method()
```

Bu nimaga misol?

A) Metod obyekt sifatida saqlanishi
B) Vorislik
C) Inkapsulyatsiya
D) Abstraksiya

---

