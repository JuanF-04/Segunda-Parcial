# Segunda-Parcial
Profe Walter

1._ def my_function(my_list=[]):
    my_list.append('???')
    return my_list

    my_function(["a", "b", "c"])

2._ my_function([1, 2, 3, 4, 5])

3._ #Si se llama sin ningún argumento
print(my_function())
print(my_function())
print(my_function())

4._ def f(my_list=None):
    if my_list is None:
        my_list = []
    my_list.append('###')
    return my_list


print(f())
print(f())
print(f())


print(f(['a', 'b', 'c']))


print(f([1, 2, 3, 4, 5]))


5._ def f1():
    print("Hola")
    print("Mundo")
    return

f1()

5.1._ def f2():
    print("Hola")
    print("Mundo")

f2()

6._ def f(x):
    if x < 0:
        return
    if x > 10:
        return
    print(x)

    6.1._ f(-3)

  6.2._ f(15)
  6.3._ f(8)

  7._ def f():
    return


print(f())

8._ def g():
    pass


print(g())


9._ def f():
    return

def g():
    pass


if f() or g():
    print('yes')
else:
    print('no')

9.1._ def f():
    return True

def g():
    pass


if f() or g():
    print('yes')
else:
    print('no')

9.2._ def double(x):
    x *= 2


x = 5
double(x)
x


9.3._ def double(x):
    x *= 2

x = 5
x = double(x)
print(x)

9.4_ def double_list(x):
    i = 0
    while i < len(x):
            x[i] *= 2
            i += 1


a = [1, 2, 3, 4, 5]
double_list(a)
a

9.5._ def double_list(x):
    r = []
    for i in x:
            r.append(i * 2)
    return r


a = [1, 2, 3, 4, 5]
a = double_list(a)
a


10._ def double(x):
    x *= 2
    return x


x = 5
double(x)
x

11. def double(x):
    x *= 2
    return x

x = 5
x = double(x)
x

11.1._ def f():
    return 'Hola'


s = f()
s

11.2._ def f():
    return dict(name_1='Hugo', name_2='Paco', name_3='Luis')


f()

f()['name_1']


11.3._ def f():
    return 'Hola Mundo'


f()[5:]


11.4._ def f():
    return ['a', 'b', 'c', 'd', 'e']


f()


12._ #Opción 1
def avg(a, b, c):
    return (a + b + c) / 3

avg(1, 2, 3)


13._ def avg(a, b=0, c=0):
    match True:
        case True if b==0 and c==0:
            avg = a
        case True if c==0:
            avg = (a + b)/2
        case _:
            avg = (a + b + c)/3
    
    return avg

avg(5)


14._ def f(*args):
    print(f"args: {args}")
    print(f"Tipo: {type(args)}, Longitud: {len(args)}")
    print("Valores")
    for x in args:
            print(f"{x}",end="|")


f(1, 2, 3)

15._ def f(*args):
    l = []
    for i in args:
            l.append(i)
    return l


a = [1, 2, 3]
t = (4, 5, 6)
s = {7, 8, 9}

nums = f(*a, *t, *s)
nums


16._ def f(**kwargs):
    for k, v in kwargs.items():
            print(k, '->', v)


d1 = {'a': 1, 'b': 2}
d2 = {'x': 3, 'y': 4}

f(**d1, **d2)

17._ def oper(x, y, *, op='+'):
    if op == '+':
            return x + y
    elif op == '-':
            return x - y
    elif op == '/':
            return x / y
    else:
            return None

oper(x=5, y=3, op='+')

